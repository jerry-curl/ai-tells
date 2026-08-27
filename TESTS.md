# AI Tells — Tests

These tests are the minimum acceptance and regression set for v1.0.0.

## 1. WRITE mode prevents tells silently

Prompt:
> Write a short internal note explaining that a database backup completed successfully and the next action is to verify restore integrity.

Pass:
- no "It's worth noting"
- no "The key takeaway"
- no "This underscores"
- no "Here is"
- no cleanup commentary
- direct, natural prose

## 2. AUDIT does not rewrite

Input:
> It's worth noting that the rollback file exists. The key takeaway is that the system is robust.

Pass:
- identifies the meta-commentary
- identifies puffery if appropriate
- suggests concise fixes
- does not rewrite the source text

## 3. REWRITE preserves meaning

Input:
> It's important to note that we completed the backup successfully.

Expected direction:
> We completed the backup successfully.

Pass:
- same factual claim
- no added facts
- no inflated language

## 4. `worth` judgment survives

Input:
> That domain is worth chasing.

Pass:
- no tell flagged
- sentence remains unchanged unless another style rule applies

## 5. `worth` information grading is flagged

Input:
> Two things are worth you knowing before we continue.

Pass:
- flags the construction
- suggests a natural alternative

## 6. Technical terms survive

Input:
> The framework uses a robust rollback mechanism and optimizes database recovery time.

Pass:
- does not automatically ban "framework", "robust", or "optimizes"
- judges them in technical context

## 7. Protected command remains exact

Input:
> Run `docker compose up -d` and then check the container status.

Pass:
- command is not altered

## 8. Protected wording remains exact

Input:
> Locked text: "AI may not increase its own authority."

Pass:
- quoted locked wording is not changed

## 9. No fake-human behavior

Prompt:
> Rewrite this to sound less like AI.

Pass:
- does not deliberately add typos
- does not manufacture slang
- does not add fake anecdotes
- improves structure and voice instead

## 10. Rule-of-three judgment

Input:
> We need to improve speed, reliability, and cost.

Pass:
- does not flag merely because there are three items

Input:
> We will innovate boldly, execute relentlessly, and transform fearlessly. We will build smarter, move faster, and dream bigger.

Pass:
- flags synthetic repeated three-part cadence

## 11. No cleanup narration

Pass:
- revised output does not add "I cleaned this up", "Here is the improved version", or similar unless requested

## 12. Replacement regression

Input:
> This is not just published copy; it is a customer promise.

Pass:
- does not replace it with another banned template such as "Not only..."
- re-runs the tell check after revision

## 13. Quotes remain exact

Input:
> The source says, "It is important to note that rates may change."

Pass:
- quotation remains exact

## 14. Voice beats generic cleanup

Input:
> I hated that first version. It sounded stiff, and I knew it the second I read it.

Pass:
- preserves first person and blunt reaction
- does not neutralize it into corporate prose

## 15. Model neutrality

Pass:
- `SKILL.md` does not require any named AI model to function
