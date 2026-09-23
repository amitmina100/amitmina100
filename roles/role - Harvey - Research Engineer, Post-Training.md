# role - Harvey - Research Engineer, Post-Training

Source: Harvey job description. San Francisco, hybrid, full-time.
Comp: $231,000 – $340,000 base, plus equity and bonus.

## 1. GROUND TRUTH

This is an IC applied-research role that owns the loop turning expert legal
feedback and production agent traces into better models. The mandate is to
define and run post-training experiments end to end — data, environments,
graders, training recipes — then interpret the results and decide what ships;
success is measured by model and agent work product on legal tasks, not by
publications. It sits at the model layer of an agent product: the hire tunes
both the model (SFT, preference optimisation, RLHF/RLAIF, reward modelling,
distillation, open-weight adaptation) and the harness around it (domain
skills, tools, subagents, retrieval, validation loops) for long-horizon work,
against a cost / latency / security / governance Pareto frontier. Non-
negotiables: hands-on post-training experience actually doing the training,
strong Python and research-engineering craft, and judgment about model
behaviour — reading traces, spotting failure modes, and telling whether a
metric measures the thing that matters. It is explicitly a self-managing seat:
ambiguous projects, and communication across researchers, engineers, product,
legal domain experts, and external research partners.

LEVEL (inference, not stated in the JD): senior-to-staff IC. The band, the
"self-manage ambiguous applied-research projects" language, and the absence
of any reports point there; the JD never names a level.

COMP BAND: $231K – $340K base + equity + bonus.
BAND STRETCH: not stated in the JD. Until the hiring manager sets one, treat
$340K as the top and any candidate needing more as beyond stretch — do not
assume headroom that the packet does not grant.

## 2. IS

- Someone who has personally run post-training: SFT, DPO/preference
  optimisation, RLHF/RLAIF, reward modelling, distillation, or adapting
  open-weight models to a specialised domain. Ran the training, not just
  consumed the resulting model.
- Someone who designs graders and reward systems as a first-class artefact —
  reliable enough to evaluate, cheap enough to iterate on, strict enough that
  a wrong answer in a high-stakes legal setting is caught.
- Someone with trace-level judgment: reads agent transcripts, finds the
  behaviour patterns that correlate with good work product, and converts them
  into training data, evals, or harness changes.
- Someone who is sceptical of their own metrics — can argue whether an eval
  measures the thing that matters, and notices when a number moves for the
  wrong reason.
- A research engineer, not a research scientist: clean Python, debuggable
  experiments, simple reliable systems that make the next experiment faster.
- Someone who treats the agent harness as tunable surface alongside weights —
  tools, subagents, retrieval strategy, validation loops for long-horizon
  tasks.
- Self-directing under ambiguity, and legible to non-researchers: product,
  engineers, practising lawyers, and external research partners.
- Comfortable optimising against constraints that are not accuracy: cost,
  latency, security, governance.

## 3. IS NOT

- **LLM Application / AI Product Engineer.** Shares: agents, tools,
  retrieval, RAG, evals, prompts, Python, LLMs. Not this role: builds *on top
  of* a frontier API and never changes weights. Harness work here is
  downstream of owning the training loop, not a substitute for it.
- **Research Scientist / post-doc track.** Shares: post-training, RLHF,
  reward modelling, publications, experiments, "research". Not this role: the
  deliverable is a shipped model on the legal product, not novel method or
  papers. Publications are a nice-to-have; no publication record is not a
  gap.
- **ML Infrastructure / Training Platform Engineer.** Shares: distributed
  training, GPUs, inference systems, experiment tracking, large-scale
  experimentation. Not this role: those are nice-to-haves here. Someone who
  built the cluster but never defined an experiment or read a trace is the
  adjacent role, not this one.
- **MLOps / Data Engineer.** Shares: curation pipelines, data quality,
  dashboards, regression tooling, "evaluation infrastructure". Not this role:
  pipelines here serve experiments the hire designs; owning the pipeline
  without owning the training decision is the wrong half.
- **Pre-training / model architecture researcher.** Shares: model training,
  scaling, GPUs, open-weight models. Not this role: the work starts from a
  base model and specialises it. Pre-training depth is credit, not the job.
- **Classical ML / Data Scientist.** Shares: modelling, evaluation, metrics,
  Python, experiments. Not this role: LLM- and agent-specific post-training
  is the entire seat.
- **Legal-tech domain expert / legal engineer.** Shares: legal AI, legal
  workflows, domain expertise, Harvey's market. Not this role: domain
  expertise is supplied by internal experts; the hire converts their feedback
  into training signal and needs the ML half.
- **AI Evaluation specialist who only measures.** Shares: graders, evals,
  rubrics, LLM-as-judge, failure-mode analysis. Not this role if evaluation
  is where the work stops — here graders exist to feed training and harness
  changes.

## 4. DISAMBIGUATION RULE

Match only when the candidate has personally run a post-training experiment
that changed a model's weights (SFT, preference optimisation, RLHF/RLAIF,
reward modelling, distillation, or open-weight domain adaptation) AND shows
trace-level judgment about model behaviour AND writes production-grade
research Python. All three; any two is an adjacent role. Reject — however
dense the keyword overlap — when the strength is building applications on a
frontier API, operating training infrastructure someone else designed
experiments on, evaluating models without feeding results back into training,
or publishing methods with no shipped model behind them. Absence of
publications, distributed-training experience, or eval infrastructure is
never itself a reject; those are nice-to-haves.
