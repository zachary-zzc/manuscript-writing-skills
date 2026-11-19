# Conditional Results guidance

Use this reference only for study types actually present in the manuscript. Read the prerequisite before each section and skip sections that do not match. These are reporting rules for existing evidence, not instructions to add experiments, models, datasets, human participants, scoring instruments or supplementary tables. The user's Easy/Normal/Expert writing mode is unrelated to whether the research includes experts.

| Guidance | Prerequisite | Does not follow merely from |
|---|---|---|
| Quantitative evidence | The reported finding makes a quantitative claim | A descriptive sample count turning an entire qualitative study or proof into a quantitative evaluation |
| Rubric-based evaluation | An assessment actually assigns scores through criteria or anchors | A standard numerical metric or ordinary peer review |
| Predictive evaluation | The study evaluates predictions, classifications or forecasts | Computational analysis, simulation or statistical testing alone |
| Biological interpretation | The claim concerns biological systems, objects or functions | An interdisciplinary manuscript with no biological claim in the relevant passage |
| Autonomous-agent evaluation | Autonomous planning, directed actions or workflow execution by a research agent is actually evaluated | An ordinary software tool, script or computational pipeline |
| Human intervention | Human assistance or expert guidance is an actual study condition | Authors, advisers, participants, peer reviewers or Expert writing mode |
| Human assessment | Human judgments or ratings are actually collected as assessment outcomes | Human intervention or an automated evaluator alone |

## Measured quantities and scored outcomes

**Prerequisite:** the reported claim is quantitative. Use the relevant quantities, units, denominators, direction, aggregation and comparison conditions. This section does not require numerical support for qualitative themes, theoretical arguments or proofs; support those with the appropriate observations, sources or reasoning.

For data-based comparisons, state whether inputs were supplied or independently selected when that distinction affects interpretation. Distinguish retrieved, eligible, retained and analysed records and attach each result to the subset that produced it. Keep measurements, annotation assignments, unique objects and grouped objects separate. Shared research outlines do not establish matched datasets. In a study without datasets or cohorts, do not introduce those concepts.

Define the quantity needed to interpret a score before discussing its value. Preserve arithmetic versus geometric averages, weighting, spread, per-class versus aggregate measures and repeated versus independent observations as relevant. Keep comparison groups, eligibility thresholds, resampling/permutation units and the full multiple-testing family consistent when those procedures were actually used; do not invent such procedures.

For inferential comparisons or claims based on statistical tests, apply the shared [statistical reporting checks](../../manuscript-audit/references/statistical-reporting.md), especially direct comparison of effects and evidence for exclusions. A descriptive count alone does not require that review.

For accuracy or reconstruction claims, foreground achieved outcomes and the appropriate reference values. Avoid arbitrary tolerance summaries that displace the finding or imply acceptance criteria absent from the protocol. Preserve exact versus approximate agreement and material discrepancies. A larger dataset or broader analysis does not itself establish greater accuracy or validity.

**Rubric-based assessment only:** identify the rated object, evaluator type and actual instrument. Provide or cite the detailed criteria and score anchors in Methods or supplementary material, and cite detailed score tables where applicable. Define scale, direction and aggregation before interpretation. Later mentions may name and cite the established assessment without repeating every criterion. Avoid remote references such as 'the dimensions above' without a clear local referent or named rubric. Do not invent a scoring rubric for an evaluation that did not use one. Automated ratings are not human-expert ratings.

## Predictive methods, including machine learning

**Prerequisite:** predictive performance is actually evaluated, whether the predictor is statistical, machine-learning-based or otherwise. Ordinary computation, association testing or the word 'model' in a theoretical paper does not activate these requirements.

Identify the prediction target, evaluated population or target range, and relevant input and output. Preserve cohort construction, preprocessing, partitioning/grouping and validation distinctions that materially affect the reported prediction result. Do not infer model training, feature selection, held-out testing or cross-validation where they did not occur.

Compare the dimension actually supported: number of observations, target/class coverage, predictive accuracy, calibration or interpretive specificity. More observations can coexist with fewer target classes or a different validation design. Scores from different cohorts and protocols do not establish superior accuracy. Describe feature ranks as ranks within their fitted model and evaluated collection, not automatically as mechanisms or complete shares of total importance. Keep interpretation-changing validation details with the affected estimate; place additional procedure in Methods or SI.

## Biological findings

**Prerequisite:** the passage interprets biological observations or functions. In other disciplines, use the corresponding scientific objects and evidence distinctions; do not require a biological discovery, molecular explanation or functional validation.

Name the supported biological relationship, process or candidate and explain what the observations mean. Keep the inference at the measured level, for example an organism, cell, molecule, genome, protein, family, cluster or recorded host/source group only when those objects occur in the study. Distinguish annotation, observed association, prediction, candidate prioritisation, experimentally demonstrated function and mechanism. Describe a useful supported hypothesis positively at its actual evidential strength without adding generic defensive wording.

**Sequence/profile annotation studies only:** distinguish unique sequences or families from annotation assignments and overlapping functional categories. Absence of a match to the screened database or profiles supports a candidate unassigned by that screen, not a newly demonstrated protein function, biochemical novelty or mechanism. Recorded host or ecological labels are not automatically experimental infection or interaction measurements. Do not impose these sequence-specific checks on unrelated biological studies.

## Autonomous research agents

**Prerequisite:** the manuscript evaluates a system as an autonomous research agent that plans or directs actions or executes a research workflow. An ordinary tool, script, pipeline or simulation is not automatically an agent. An agent study need not involve machine learning or human assistance; activate those other sections independently.

Distinguish the underlying model when present, generated roadmap, interaction, completed execution, end result and rated output. Name what the experiment actually tests; do not attribute a bare-model result to the whole agent or treat a planned task as a completed analysis. Explain scientifically consequential workflow coverage without listing every tool call.

If agents choose their own data or analytical procedures, state that freedom and distinguish retrieval counts from the analysed cohorts. Compare the supported dimensions, such as dataset coverage, completed scientific analyses or output specificity. A full-workflow comparison does not isolate one component's causal effect. Delivered analyses are not necessarily correct or equally validated. If conversational state is studied, a successful next response does not alone prove restoration of accumulated state.

## Human contributions and assessments

**Prerequisite:** human assistance/intervention or human assessment is an actual component of the research design. Treat these as independent conditions: assistance does not imply ratings, and ratings do not imply assistance. Authors, advisers, ordinary peer review, human participation in general and Expert writing mode do not by themselves activate an expert-collaboration experiment. Do not invent experts, independent raters, blinding or qualifications.

**Intervention present:** report the actual role, decisions changed, work subsequently performed and outcomes under that condition. For studies specifically comparing autonomous agent findings with optional expert-guided extensions, present the initial findings coherently before the extensions when that follows the scientific question. Explain what experts revised, what the agent executed and which discoveries arose in the guided runs. Do not interrupt each initial finding with expert contributions from a different condition. In non-agent studies, follow the actual intervention design rather than importing roadmaps or agent terminology.

Quantify interaction or plan changes only if recorded and informative. Identify the unit, comparison condition and relevant trajectory length; categories may overlap. More turns or revisions alone do not establish efficiency, collaboration quality or improved scientific outcomes. If coverage combines initial and revised outputs, label it as a union and do not present it as autonomous performance or as the increment caused by intervention.

**Human assessment present:** distinguish the assessment role from the intervention role without assuming the people are different. Describe the actual rated material, scale and independent/blinded procedure only as supported by the study records. Apply the rubric guidance only if a rubric was used. Expert ratings assess the rated outputs; they do not independently verify every factual claim. Preserve mixed quality results. Within Results, avoid repeating shared qualifications or full established criterion lists; retain enough local context and cite the named assessment or supplementary rubric.
