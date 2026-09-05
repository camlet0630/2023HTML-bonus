# Automated AI Debate Experiments

This repository contains a team project completed for the bonus track of the 2023 Fall Machine Learning course at National Taiwan University. The project investigates how model parameters and prompting strategies affect the quality of AI-agent debates evaluated by the CRIT scoring system.

The experiments use Selenium to automate a course-provided debate interface based on SocraSynth. Two language-model agents take opposing positions, agree on a set of discussion topics, exchange arguments, and produce structured conclusions for evaluation.

## Research directions

The project studied three approaches:

1. Adjusting model parameters and argument strength.
2. Asking agents to support their arguments with evidence and references.
3. Providing examples from previously evaluated debates.

The full methodology, analysis, and results are available in an [anonymized copy of the project report](machine_learning_bonus_track_report.pdf).

## Repository contents

- [`chatUI_auto`](chatUI_auto): the original automation program referenced directly by the project report. It is preserved at its original path and has not been modified.
- [`HTML_chatUI_auto.ipynb`](HTML_chatUI_auto.ipynb): an earlier notebook used to develop and test the automated debate workflow. Execution outputs have been removed.
- [`machine_learning_bonus_track_report.pdf`](machine_learning_bonus_track_report.pdf): an anonymized copy of the final report.
- [`sample_debate_outputs`](sample_debate_outputs): transcripts and structured output retained from sample debate runs.

## Sample debate outputs

| File | Debate question |
| --- | --- |
| [`regulating_llms_in_education_and_research_run_1.txt`](sample_debate_outputs/regulating_llms_in_education_and_research_run_1.txt) | Should we regulate the use of large language models in education and research? |
| [`regulating_llms_in_education_and_research_run_1.csv`](sample_debate_outputs/regulating_llms_in_education_and_research_run_1.csv) | Structured output generated from Run 1 of the same debate question. |
| [`regulating_llms_in_education_and_research_run_2.txt`](sample_debate_outputs/regulating_llms_in_education_and_research_run_2.txt) | A second run of the same debate question. |
| [`professors_monetizing_educational_youtube_videos.txt`](sample_debate_outputs/professors_monetizing_educational_youtube_videos.txt) | Should professors monetize their educational videos on YouTube? |

## Historical context and reproducibility

The code depends on a course platform and evaluation service used in 2023, as well as the APIs and model names available at that time. These external services may no longer be available, so the repository is maintained as a record of the original project rather than as a currently reproducible application.

The `chatUI_auto` file is kept unchanged because the final report links directly to that path. It represents the submitted project artifact, although parts of the documented experimental workflow may not be fully reflected in the retained code.
