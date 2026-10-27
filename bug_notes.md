# Bug Notes

| Bug | Evidence / Failed Test | Cause | Fix |
| :--- | :--- | :--- | :--- |
| Average | 135.0 instead of 90.0; single-mark crash[cite: 5] | Dividing by `len(marks) - 1`[cite: 5] | Divide by `len(marks)`[cite: 5] |
| Pass boundary | 40 returned False[cite: 5] | Used `>` instead of `>=`[cite: 5] | Use `>= PASS_MARK`[cite: 5] |
| Distinction | 95 returned First[cite: 5] | `>= 60` checked before `>= 90`[cite: 5] | Check `>= 90` first[cite: 5] |
