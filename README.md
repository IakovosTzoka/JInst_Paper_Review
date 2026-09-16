# JINST Paper Reviewer

A standalone skill for critically reviewing instrumentation manuscripts before submission to the Journal of Instrumentation (JINST). Combines Aaron Storey's general paper-review workflow with JINST guidance and technical instrumentation checks.

## Use

Point a skill-capable assistant at [SKILL.md](SKILL.md) and provide an author-owned draft or a public paper for ordinary scientific critique:

```text
Use $jinst-paper-reviewer to review my detector manuscript before submission
to JINST as a research article. Focus on calibration, timing resolution,
systematic uncertainties, and whether the main claims are supported.
```

The result is an assessment with located findings, supporting evidence, and prioritized revisions. The skill covers detectors, electronics, DAQ, simulations, reconstruction methods, and other instrumentation as applicable. It does not require the original skill's companion tools.

For an assigned journal referee review, the skill supports policy-compatible language editing of the referee's own report. It does not automate the scientific referee assessment. See [journal guidance and sources](references/jinst-guidance.md).

## Package

- `SKILL.md`: combined workflow and mode selection.
- `references/jinst-guidance.md`: journal criteria, review policy, and official sources.
- `references/instrumentation-checks.md`: technical review prompts.
- `assets/review-report.md`: full review output template.
- `agents/openai.yaml`: Codex display metadata.

This repository is the complete skill package, not an MCP server. To obtain a copy with the skill's directory name:

```sh
git clone https://github.com/IakovosTzoka/JInst_Paper_Review.git jinst-paper-reviewer
```

Place the complete `jinst-paper-reviewer` folder in the skills directory supported by your assistant, keeping relative paths intact. Cloning alone does not install it into an assistant.

Keep manuscript inputs and review outputs outside this repository. The repository should contain only reusable skill files.

## Attribution

Adapted from [paper-reviewer by Aaron Storey](https://github.com/astoreyai/claude-skills/blob/b6c399b095322fd65bca61ec5f045985493243ab/paper-reviewer/SKILL.md), version 1.0.0, discovered through [MCP Market](https://mcpmarket.com/tools/skills/paper-reviewer). Upstream revision checked: `b6c399b095322fd65bca61ec5f045985493243ab`, on 2026-09-16. The upstream MIT notice is preserved alongside the repository author's notice in [LICENSE](LICENSE).

The adaptation adds JINST categories and instrumentation checks, removes fixed AI-authorship and checklist pass thresholds, and replaces external skill dependencies with a self-contained workflow. Journal documents are linked and summarized rather than bundled. This is an independent tool, not an official JINST, SISSA Medialab, or IOP Publishing product.
