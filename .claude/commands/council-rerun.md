Rerun a hiring council sitting with new evidence.
Arguments: $ARGUMENTS = <previous sitting folder> <answers file path>

1. Read `<previous sitting>/ruling.json` and `<previous sitting>/state.json`
   to get the role and candidate paths.
2. Create a new SITTING folder under the same candidate slug. Copy the
   previous `ruling.json` into it as `prior_ruling.json`. Copy the answers
   file into it as `answers.md`.
3. The answers file must tag each item with a provenance tier:
   `[public_artefact]`, `[self_reported]`, or `[interviewer_observed]`. If
   any item is untagged, stop and ask the user to tag it.
4. Run the full `/council` procedure with the same role and candidate paths,
   with these changes:
   - Every seat prompt additionally includes:
     `PRIOR_RULING: SITTING/prior_ruling.json` and `ANSWERS: SITTING/answers.md`
     and the line "This is a rerun. Do not re-litigate settled findings.
     Treat [interviewer_observed] opinions as opinions and
     [interviewer_observed] specifics as evidence."
   - Chair MODE=open must state which prior open_questions the answers
     address.
   - Chair MODE=rule must fill `diff_from_prior`.
5. Finish as in /council, and additionally print `diff_from_prior`.
