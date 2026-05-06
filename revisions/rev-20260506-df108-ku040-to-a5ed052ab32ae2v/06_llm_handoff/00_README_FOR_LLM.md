# README For LLM

This folder is a platform-neutral LLM handoff bundle for the DF108 schematic revision task.

It is intended for use in web-based ChatGPT, Claude, Gemini, or another LLM interface where the model does not have access to the local `sch-review` workspace, Cadence PST parser, or project history.

## Scope

Project: `DF108`

Revision: `rev-20260506-df108-ku040-to-a5ed052ab32ae2v`

Task: evaluate a schematic revision described as `KU040 -> Agilex 5 A5ED052AB32AE2V`, while preserving the DF108 peripheral domain.

Current status: pre-review handoff. This is not schematic sign-off, board-release approval, or a formal project closure record.

## Files In This Bundle

| File | Purpose |
|---|---|
| `01_design_context.md` | Self-contained design context for another LLM. Start here. |
| `02_key_facts.md` | Fact table extracted from BOM, PST netlist, opendatasheet, intake, and review outputs. |
| `03_open_questions.md` | Questions that must be resolved before treating this as an A5ED052AB32AE2V design review. |
| `evidence_refs.json` | Machine-readable evidence index with paths, hashes, and line hints. |

## Important Correction

After the initial handoff was generated, the user clarified that the current input is a correct existing schematic with a new Agilex chip package/scheme added as a placeholder. C-type and D-type package usage is unified for this stage, and the part-name mismatch will be corrected later.

Therefore, do not read the initial raw `review status = fail` and `errors = 40` as 40 confirmed schematic design errors. Read:

- `../../03_review_runs/run-task-20260506-df108-ku040-a5ed052ab32ae2v-intake/judgment_interpretation.md`
- `../../02_design_evidence/judgment_mode_correction_20260506.md`

before interpreting raw review output.

## How To Use

For a short external LLM session, provide `01_design_context.md` and `02_key_facts.md`.

For evidence-sensitive review, also provide `03_open_questions.md` and `evidence_refs.json`.

Avoid giving the raw `pstxnet.dat` directly as the first input. It is large and low-level. Use this bundle first, then only provide raw netlist snippets when the LLM asks for specific evidence.

## Boundary

Facts in this bundle are either:

- directly extracted from the downloaded BOM/netlist;
- extracted from local opendatasheet exports;
- produced by the initial `sch-review` run;
- explicitly marked as open questions.

Do not treat borrowed evidence as an official Intel last-mile confirmation. Do not treat this bundle as a formal DF108 project baseline.
