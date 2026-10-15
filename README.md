Following an idea by Alex Meiburg on [Zulip](https://leanprover.zulipchat.com/#narrow/channel/583339-AI-authored-projects/topic/OpenAI.20releases.20solutions.20to.20hundreds.20of.20problems/near/630328676)

`Challenge.lean`:

```
def LeanIsInconsistent : Prop := False

theorem iCanProveIt : LeanIsInconsistent := by
  sorry
```

`comparator.json`:

```
{
    "challenge_module": "Challenge",
    "solution_module": "Solution",
    "theorem_names": ["iCanProveIt"],
    "definition_names": ["LeanIsInconsistent"],
    "permitted_axioms": ["propext", "Quot.sound", "Classical.choice"]
}
```
