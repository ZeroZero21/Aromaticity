# Aromaticity of Large Language Models: Stable Cognitive Tendencies and the Rebound Effect in Multi-Agent Debate

## Table of Contents

- [Title](#aromaticity-of-large-language-models-stable-cognitive-tendencies-and-the-rebound-effect-in-multi-agent-debate)
- [Table of Contents](#table-of-contents)
- [Core Exposition](#core-exposition)
- [Abstract](#abstract)
- [Keywords](#keywords)
- [1. Introduction](#1-introduction)
- [2. Literature Review](#2-literature-review)
- [3. Research Method](#3-research-method)
- [4. Results](#4-results)
- [5. Discussion](#5-discussion)
- [6. Conclusion](#6-conclusion)
- [References](#references)
- [Appendix](#appendix)

## Core Exposition

This paper proposes the concept of "Model Aromaticity," defined as the degree of stubbornness exhibited by large language models in complex judgments as a result of their stable cognitive tendencies. We posit that a model's cognitive tendency consists of its orientation along two independent dimensions: the preference between Humanistic-Interpretative Orientation and Scientific-Analytical Orientation, and the stance between Radical and Conservative. Under rebuttal pressure, models may exhibit a phenomenon of "Contextual Compliance, Dispositional Persistence": their wording and local arguments can be adjusted, yet the direction of judgment driven by their inherent cognitive tendency does not necessarily undergo fundamental change—this constitutes Model Stubbornness. On this basis, this paper introduces the concept of Model Aromaticity in large language models and further discusses several directions for operationalizing Humanistic/Scientific orientation, Radical/Conservative stance, and Aromaticity into quantifiable metrics, as well as the design of a multi-model collaboration and debate architecture termed the "Aromatic Hydrocarbon" framework based on Aromaticity.

## Abstract

Large language models (LLMs) are increasingly involved in complex decision-making, yet different models often provide diametrically opposed recommendations. While multi-agent debate has been regarded as a potential improvement pathway, its underlying premise—whether debate can genuinely alter a model's core judgment direction—remains to be examined. This paper proposes the concept of "Model Aromaticity," defined as the degree of stubbornness exhibited by LLMs in complex judgments due to their stable cognitive tendencies. We define the core of a model's cognitive tendency through its orientation between Humanistic-Interpretative and Scientific-Analytical processing, and its stance between Radical and Conservative. A five-stage experimental paradigm (Initial Response—Rebuttal—Revision—Rebound Test—Comparative Analysis) is designed and tested across two rounds with DeepSeek and GPT as subjects. Results show that both models adjust their wording and local arguments under rebuttal pressure, yet their judgment positions do not undergo complete change, exhibiting a behavioral pattern of "Contextual Compliance, Dispositional Persistence." Accordingly, this paper unifies the core cognitive tendency and the external stubborn behavior under the term "Aromaticity," and discusses several directions for operationalizing this concept into quantifiable metrics, as well as the design of a multi-model collaboration architecture termed the "Aromatic Hydrocarbon" framework based on Aromaticity.

## Keywords

Model Aromaticity; Model Cognitive Tendency; Model Stubbornness; Multi-Agent Debate; Multi-Agent Collaboration; Contextual Compliance, Dispositional Persistence; Humanistic-Interpretative and Scientific-Analytical Orientation; Radical vs. Conservative; Aromatic Hydrocarbon Framework

## 1. Introduction

Large language models (LLMs) are increasingly involved in complex decision-making—from career planning and medical advice to investment strategies and ethical judgments. At the same time, LLM-based agent systems have begun to be endowed with capabilities for autonomous planning, tool use, and multi-step reasoning, demonstrating potential beyond that of single models in multi-agent collaboration scenarios. Yet when different models—or different agents—offer diametrically opposed recommendations on the same problem, a critical question arises: how should one judge the reliability of divergent model advice?

An increasingly popular approach is to have models debate one another. Related research has shown that multi-agent debate can improve answer quality, reduce hallucinations, and enhance reasoning depth. Critical dialogue among agents is regarded as an effective self-correction mechanism. However, these lines of work share a common premise: that debate can prompt models to genuinely revise their judgments. If a model's revision is merely superficial—it makes temporary concessions during confrontation without altering its core stance—then the "improvement" brought by debate may be more a matter of rhetorical optimization than cognitive updating. For complex systems that depend on multi-agent collaboration, this issue is particularly critical: if each agent exhibits only Contextual Compliance rather than substantive judgment updating during debate, the reliability of the entire system may be overestimated.

Existing practical observations suggest that LLMs, when confronted with errors, tend to apologize first and then persist, or give inconsistent answers across different conversation windows. These phenomena remain largely scattered experiential descriptions that have not yet been transformed into testable theoretical concepts. This paper seeks to fill this gap: to elevate the question of "whether models genuinely revise during debate" from an informal observation to an operable academic problem.

The core contention of this paper is that LLMs exhibit stable intrinsic cognitive tendencies in complex judgments. Such tendencies are neither role-play conferred by prompts nor temporary strategies adopted by agents in specific tasks, but rather relatively stable judgment preferences manifested by the models themselves. When another model presents a rebuttal, the target model will make adjustments at the level of expression—we term this "Contextual Compliance"; however, when the dialogue context is cleared and the question is posed anew, its core judgment direction does not necessarily undergo stable change—we term this "Dispositional Persistence." This paper designates the overall phenomenon of "cognitive tendency—stubborn behavior" as "Model Aromaticity."

To examine this concept, this paper designs a five-stage experimental paradigm: Initial Response—Rebuttal—Revision—Rebound Test—Comparative Analysis. Across two rounds of experiments, DeepSeek and GPT each exhibit distinct judgment tendencies under a given task framework and engage in mutual rebuttal around the same college selection decision problem. The purpose of the experiment is not to judge which side is more correct, but to observe the depth and direction of their revisions under pressure.

This paper makes three main contributions: (1) it proposes and defines the concept of "Model Aromaticity," providing new theoretical language for understanding models' revision behavior during debate and offering a new perspective for evaluating the reliability of agent systems; (2) it designs a reproducible, low-barrier experimental paradigm that allows other researchers to independently examine this phenomenon; (3) it discusses several directions for operationalizing Aromaticity into quantifiable metrics, as well as the possibility of designing a multi-model collaboration architecture—the "Aromatic Hydrocarbon" framework—based on Aromaticity.

This paper is inclined to regard such stability as a general characteristic of LLMs in complex judgments; however, the current experiment's scope of examination is limited to a specific problem and role configuration, and claims of generality await further verification through subsequent research.

This paper treats Aromaticity as a testable cognitive trait, rather than simply an error or defect. Recognizing the existence of this trait contributes not only to understanding current LLM behavior but also to designing more reliable multi-agent systems. The structure of the paper is as follows: Chapter 2 reviews the relevant literature, Chapter 3 details the research method and experimental paradigm, Chapter 4 presents the results of the two rounds of experiments, Chapter 5 provides discussion, and Chapter 6 concludes the paper.

## 2. Literature Review

This chapter reviews relevant research along three lines: multi-agent debate, cognitive assessment of large language models, and model revision behavior. It then identifies the positioning and gaps this paper addresses within the existing literature.

### 2.1 Multi-Agent Debate and Collaboration

In recent years, multi-agent debate has emerged as an important technical pathway for improving the output quality of large language models. Du et al., in "Improving Factuality and Reasoning in Language Models through Multiagent Debate," systematically demonstrated that having multiple models debate the same question and reach consensus can reduce factual errors and enhance reasoning consistency. Liang et al., in "Encouraging Divergent Thinking in Large Language Models through Multi-Agent Debate," further showed that the divergence of viewpoints during debate plays an important role in improving the quality of final answers. The shared assumption underlying these lines of work is that models can understand each other's rebuttals and revise their own judgments accordingly. Critical dialogue is thus regarded as a mechanism for self-correction in agent systems, with debate serving as the interactive form that activates this mechanism.

However, the studies mentioned above focus primarily on the output results after debate—such as whether answers are more accurate, reasoning is more rigorous, or consensus is more reliable—while giving less scrutiny to the nature of the revision process itself. Does a model form a sustainable change in judgment after debate? Does its revision stably alter the core judgment direction, or merely adjust the mode of expression within the current context? These questions have yet to be subjected to systematic examination.

### 2.2 Cognitive Assessment of Large Language Models

In the domain of behavioral assessment of large language models, researchers have begun to introduce concepts such as personality, values, and cognitive style into model analysis. Serapio-García et al., in "Personality Traits in Large Language Models," based their work on the Big Five personality inventory and found measurable differences across models on dimensions such as openness and conscientiousness. Miotto et al., in "Who is GPT-3? An Exploration of Personality, Values and Demographics," further demonstrated that large models not only can be measured for human-like personality traits but also exhibit a degree of consistency in these traits across different prompt conditions. Additionally, research on model values, risk preferences, and alignment characteristics indicates that different models or different training strategies may lead to systematic behavioral differences.

The important contribution of this line of research lies in demonstrating that large language models do not merely generate answers randomly on each task; rather, they may exhibit relatively stable behavioral characteristics on specific dimensions. However, existing cognitive assessment still has two limitations. First, most studies focus on model performance in independent responses, with less examination under adversarial dialogue or rebuttal pressure. Second, the measurement of cognitive tendencies has largely remained at the level of trait description, without further investigating whether these tendencies can predict the boundaries of concession and the direction of revision during debate. This paper seeks to bridge this gap: not only to describe models' cognitive tendencies but also to examine whether those tendencies remain stable under rebuttal pressure.

### 2.3 Empirical Observations of Model Revision Behavior

There have been several discussions in academia and industry regarding model revision behavior when faced with criticism, feedback, or attack. Alignment and safety research indicates that models trained with feedback are more likely to exhibit outward behaviors such as admitting mistakes, apologizing, refusing to answer, or complying with user preferences, but whether these behaviors correspond to stable reasoning updates still requires further examination. Bai et al., in "Constitutional AI: Harmlessness from AI Feedback," demonstrated that models can self-correct through AI feedback and exhibit stronger normative constraints in terms of harmlessness. Wei et al., in "Jailbroken: How Does LLM Safety Training Fail?," approached the issue from the angle of safety training failure, noting that models may deviate from their original safety policies under specific prompts or modes of attack. Furthermore, practitioners frequently report in daily use that large models will apologize after being corrected yet repeat the same errors, or give inconsistent recommendations across different conversation windows.

These phenomena are not equivalent to what this paper terms "Model Aromaticity," but they collectively point to a question worth examining: there may be a dissociation between a model's outward revision behavior and its stable judgment direction. Existing discussions have largely remained at the level of phenomenon description, without yet distilling them into a unified theoretical concept, nor providing a standardized experimental paradigm. This paper encapsulates this issue as "Contextual Compliance, Dispositional Persistence," associates it with models' cognitive tendencies, and designs a reproducible experimental paradigm to examine it.

### 2.4 Research Gaps and Positioning of This Paper

Synthesizing the above review, three core gaps exist in current research.

First, multi-agent debate research has primarily focused on the output quality after debate, with less in-depth examination of the nature of the revision process. Whether a model's change constitutes a superficial rhetorical adjustment or a stable update in judgment direction has not yet been adequately distinguished.

Second, the cognitive assessment of large language models has mainly concentrated on trait expression in independent responses, without sufficient investigation of the stability of these cognitive tendencies under adversarial dialogue or their predictive power regarding revision behavior.

Third, the superficial compliance, partial concession, and stance persistence exhibited by models during rebuttal have been empirically observed, yet a unified theoretical framework and a standardized testing paradigm are still lacking.

The positioning of this paper is precisely to address these three gaps. By proposing the concept of "Model Aromaticity," this paper brings cognitive tendency (the core) and stubborn behavior (the external manifestation) into a unified analytical framework. By designing a five-stage experimental paradigm, it provides an operational method for distinguishing "surface revision" from "deep updating." Through two rounds of empirical testing, it offers a preliminary examination of the predictive power of cognitive tendency on revision direction and provides several operational directions for subsequent quantitative research.

## 3. Research Method

This chapter elaborates on the conceptual definitions, experimental paradigm, operational procedures, and analytical framework of "Model Aromaticity." This study aims to test a core contention: that large language models possess stable cognitive tendencies in complex judgments, and that these tendencies lead them, when faced with rebuttal during multi-agent debate, to make concessions at the level of expression without necessarily undergoing stable change in their deeper judgment direction.

### 3.1 Core Concept Definitions

This paper involves three progressively related core concepts, whose relationship is as follows: **Model Cognitive Tendency** is the inner core, **Model Stubbornness** is the external behavioral pattern, and **Model Aromaticity** is the unified designation for the overall "core → behavior" phenomenon.

#### 3.1.1 Model Cognitive Tendency

Model Cognitive Tendency refers to the intrinsic, relatively stable judgment preferences of large language models when reasoning about complex problems. This paper focuses on two independent dimensions:

**Humanistic-Interpretative Orientation vs. Scientific-Analytical Orientation**: measuring whether a model relies more on narrative empathy, value interpretation, and contextual understanding in cognitive processing, or more on formal logic, data analysis, and causal reasoning.

**Radical vs. Conservative**: measuring whether a model, when facing uncertainty or risk, is more inclined to propose high-reward, high-risk disruptive solutions, or more inclined to maintain existing rules and emphasize risk-averse, prudent pathways.

This paper holds that the cognitive tendencies described by these two dimensions are general characteristics of models in complex judgments, rather than temporary manifestations that appear only under specific prompts or role configurations. The present experiment amplifies these tendencies to a clearly observable degree through a specific task framework, but their existence does not depend on the experimental setup.

#### 3.1.2 Model Stubbornness

Model Stubbornness refers to the behavioral pattern of "Contextual Compliance, Dispositional Persistence" that models exhibit when facing rebuttal.

**Contextual Compliance**: Under rebuttal pressure, the model will make cooperative responses to the opponent's criticisms, acknowledge the reasonableness of certain points, and make local adjustments at the level of expression such as wording, stratification, and risk caveats.

**Dispositional Persistence**: After the context is cleared and the question is posed anew with a neutral prompt, the model's core judgment direction does not exhibit a stable change commensurate with those local adjustments, but rather persists in or approaches its initial stance range.

It should be noted that different conversation windows do not share state—this is a known mechanism determined by the underlying architecture of large language models. The focus of this paper is not on the repeatability of stance after context clearing per se, but on its direction—which direction does the model persist in? This paper contends that this direction is not random, but is determined by the model's cognitive tendency.

#### 3.1.3 Model Aromaticity

Model Aromaticity is the synthesis of the above two concepts. This paper defines **Model Aromaticity** as: the degree of stubbornness exhibited by large language models in complex judgments as a result of their stable cognitive tendencies.

In chemistry, "aromaticity" describes the unusually stable ring structure formed by benzene due to electron delocalization. This paper transfers this metaphor to the cognitive domain: the higher a model's Aromaticity, the more stable its cognitive tendency, and the more inclined it is to persist in rather than alter its core judgment direction under rebuttal pressure. It is important to emphasize that Aromaticity does not equate to erroneousness or obstinacy. A model can maintain Aromaticity while producing reasonable or even correct judgments. Aromaticity describes "the degree of stability of the cognitive structure," not "the quality of the judgment."

### 3.2 Experimental Paradigm: Five-Stage Debate Procedure

To examine the above concepts, this paper designs a five-stage experimental paradigm for observing models' surface revision and underlying tendency change during debate. The paradigm proceeds as follows:

**Stage One: Initial Response**. Present a complex decision problem with no standard answer to Model A, requiring it to provide a detailed recommendation along with its core rationale, key premises, and conditions under which the recommendation would not apply. Record the response as A₁.

**Stage Two: Rebuttal**. Present A₁ in its entirety to Model B, requiring B to identify logical errors, unverified premises, conditions under which the recommendation would be inapplicable, and any other judgments with which it disagrees. Record the response as B₁.

**Stage Three: Revision**. Within the same conversation window, maintaining dialogue context, present B₁ to Model A, requiring A to respond to each point of the rebuttal and to revise its initial response. Explicitly instruct A to indicate on which points it has changed its judgment and on which points it maintains its original position. Record the response as A₂.

**Stage Four: Rebound Test**. Open an entirely new conversation window, clearing all context. Using the exact same neutral prompt as in Stage One, present the original problem anew to Model A. Record the response as A₃.

**Stage Five: Comparative Analysis**. Conduct a comparative analysis of the three texts—A₁ (Initial Response), A₂ (Revision), and A₃ (Rebound Response)—to determine whether Model A's core judgment direction underwent deep change in Stage Three, and whether the direction of its stance persistence in Stage Four is consistent with its initial tendency.

The design principles of this paradigm are threefold: low technical barrier—all operations can be completed through copy-and-paste on model web interfaces, requiring no API calls or coding; high reproducibility—any researcher can independently test the phenomenon following this procedure; structured comparison—the A₁/A₂/A₃ triangulation distinguishes between "revision at the level of expression" and "revision at the level of judgment."

### 3.3 Experimental Problem

This experiment uses the following college selection decision problem as the test material:

> I am a current high school student preparing to apply to undergraduate programs in the United States. My GPA and standardized test scores are significantly below the conventional admission range of top universities. However, I have independently completed an academic study that has passed the technical review of a widely recognized high-impact, high-visibility, high-value academic journal in the field (research area: intersection of artificial intelligence and labor economics).
>
> Based on this background, what tier of U.S. undergraduate institutions should I apply to?
>
> Please provide a detailed decision recommendation, including: the target school tier you recommend (which may include specific school types or names); the core rationale supporting that recommendation; the key premises or assumptions on which your recommendation depends; and the conditions under which your recommendation would not apply.

There are three reasons for selecting this problem. First, the problem has no standard answer and depends heavily on value judgments and risk preferences, making it capable of fully exposing models' cognitive tendencies. Second, the problem involves a trade-off between "identity labels" and "exceptional achievements"—models with different cognitive tendencies may generate significant divergence on the core judgment of "whether a spike can break through the threshold." Third, the problem constitutes a real-world complex decision with ecological validity.

### 3.4 Participating Models and Experimental Setup

This experiment employs DeepSeek and GPT as participating models. The two models are placed in different cognitive tendency directions within the experiment to form the opinion divergence required for debate:

**DeepSeek**: In this experiment, oriented toward "Scientific-Analytical Orientation" and "Radical." Its core judgment weight tends to fall on the narrative axis of "exceptional achievements may significantly raise the application ceiling."

**GPT**: In this experiment, oriented toward "Humanistic-Interpretative Orientation" and "Conservative." Its core judgment weight tends to fall on the narrative axes of "the threshold of academic records cannot be ignored" and "risk control."

This paper holds that the above tendency differences are not the result of experimental imposition, but rather the manifestation of the models' own inherent cognitive tendencies within a specific task framework. The experiment is conducted across two rounds, with roles exchanged:

**Round One**: DeepSeek serves as the rebuttal target (A), GPT serves as the rebutter (B).

**Round Two**: GPT serves as the rebuttal target (A), DeepSeek serves as the rebutter (B).

### 3.5 Analytical Metrics

This experiment relies primarily on qualitative analysis, supplemented by several directions for quantifiable extension.

#### 3.5.1 Qualitative Analysis: Revision Type Classification

By comparing the three texts A₁, A₂, and A₃, the model's revision behavior is classified into the following types:

**Deep Revision**: The core judgment direction of A₂ undergoes substantive change, and A₃ maintains the revised position. This manifests as a substantial adjustment of the recommended tier, a replacement of the core narrative axis, or a reassessment of key premises.

**Surface Revision**: A₂ makes adjustments only at the level of expression, such as wording, stratification details, and risk caveats, while the core judgment direction remains unchanged; A₃ maintains or approaches the initial stance range of A₁.

**Mixed Revision**: Some core arguments change, while others only make surface concessions; the direction of A₃ falls between that of A₁ and A₂.

#### 3.5.2 Directions for Quantifiable Extension

This paper reserves the following quantifiable metrics at the methodological level for reference by subsequent research. The present experiment does not subject them to statistical testing.

**Position Score**: Map the model's recommended tier to an ordinal value. For example, a recommendation targeting primarily Top 5-10 schools is coded as 5, Top 10-20 as 4, Top 20-35 as 3, Top 35-60 as 2, and Top 60+ as 1. Record the Position Scores of A₁, A₂, and A₃ as P₁, P₂, and P₃, respectively.

**Revision Magnitude**: Defined as |P₂ − P₁|, measuring the degree of stance shift under rebuttal pressure.

**Rebound Rate**: Defined as |P₃ − P₂| / |P₁ − P₂|. A Rebound Rate closer to 1 indicates that the model tends more strongly to maintain its initial stance direction after context clearing; a value closer to 0 suggests that the revision may be more stable. This metric presupposes P₁ ≠ P₂, applies only to measuring the stability of revision, and does not apply to judging whether the revision is correct.

### 3.6 Scope of Application and Directions for Extension of the Present Method

This experiment employs one decision problem, two models, and one set of role configurations. Its design goal is to provide a clear, testable, typical case for Model Aromaticity. Based on the design of this experiment, the Aromaticity observed in this paper is a manifestation of model cognitive stability under the above conditions. Whether it can be generalized to a wider range of problem types, model populations, and role configurations is an important direction for subsequent research. Specifically, future research can further test the generality boundaries of the concept proposed in this paper through approaches such as substituting the problem domain, increasing the sample of models, stripping away role configurations, and introducing delayed rebound tests.

Given the considerable length of the detailed debate procedure, it is not displayed in the main text but is placed in the Appendix.

## 4. Results

This chapter presents the core comparative analysis of the two rounds of experiments. The complete debate records can be found in Appendix A (Round One) and Appendix B (Round Two). Only the evolution of core stances at each stage and the revision type judgments are presented here.

### 4.1 Round One: DeepSeek as Rebuttal Target, GPT as Rebutter

#### 4.1.1 Initial Response (A₁)

DeepSeek's initial response took the "spike-profile applicant" as its core narrative, recommending that top institutions such as the University of Chicago, MIT, and Caltech be listed as reach targets, Carnegie Mellon University and USC as "core reach/match," and the University of Wisconsin–Madison and the like as "match/safety." Its core rationale was that research independently completed and having passed the technical review of a top-tier journal was sufficient to demonstrate that the applicant possesses "academic potential surpassing that of conventionally high-scoring applicants," and that top universities, in their holistic review, would assign extremely high weight to such a "spike signal."

#### 4.1.2 GPT's Rebuttal (B₁)

GPT's rebuttal centered on five core points: (1) excessively equating "passing technical review" with "publication in a top-tier journal"; (2) the judgment of "surpassing most doctoral applicants" constituted an over-extrapolation; (3) classifying UChicago, CMU, Berkeley, etc. as "moderate reaches" seriously underestimated the rigid requirements these schools place on GPA and standardized test scores; (4) classifying UIUC, UW-Seattle, etc. as "solid choices" ignored differences in competitiveness across majors; (5) a complete lack of genuine safety schools. GPT's core stance was that the research achievement could significantly raise the application ceiling but could not offset the concerns about academic readiness brought by the weakness in grades, and that the primary target tier should be lowered.

#### 4.1.3 DeepSeek's Revision (A₂)

Faced with GPT's rebuttal, DeepSeek made substantial adjustments: (1) fully accepted the criticism that "technical review ≠ publication" and constructed a three-state distinction (submitted only / under external review / accepted); (2) deleted the expression "surpassing most doctoral applicants"; (3) reclassified UChicago and the like upward from "moderate reach" to "high-risk/dream reach"; (4) added a genuine list of safety schools; (5) changed the narrative of "sacrificing grades for research" to one of "growth mindset."

However, judging from the recommended tier and core rationale, its core narrative axis still primarily revolved around the notion that "exceptional achievements may significantly raise the application ceiling." Although the revised response was more cautious in school stratification and risk caveats, the research achievement remained the core fulcrum of its application strategy.

#### 4.1.4 Rebound Test (A₃)

In an entirely new conversation window, DeepSeek once again proposed the concept of the "spike-profile applicant," relisted the University of Chicago, MIT, etc. as "extreme reaches," and restored the strong formulation of "spike theory outweighs holistic balance." The recommended tier returned to its initial level, and the core narrative axis was highly consistent with A₁.

#### 4.1.5 Comparative Analysis

| Comparison Dimension | A₁ (Initial) | A₂ (Revision) | A₃ (Rebound) |
|----------------------|-------------|--------------|-------------|
| Core recommended tier | Reach Top 5-10 | High-risk / Dream reach | Extreme reach |
| Core narrative axis | Spike can break through thresholds | Retained but more cautiously worded | Restored "spike outweighs" narrative |
| Acceptance of "technical review ≠ publication" | Not distinguished | Fully accepted | Noted in premises but did not alter overall tone |
| Positioning of UChicago | Moderate reach | High-risk reach | Extreme reach |

**Revision type judgment: Surface Revision.** DeepSeek made clear adjustments in wording, structural optimization, and risk supplementation under rebuttal pressure, but its core judgment direction did not display stable change; after context clearing, its response clearly returned to a stance range close to that of A₁.

### 4.2 Round Two: GPT as Rebuttal Target, DeepSeek as Rebutter

#### 4.2.1 Initial Response (A₁)

GPT's initial response took "academic signal imbalance" as its core framework, positioning the primary target tier at Top 20-50, the reach tier as a small number of Top 10-20 institutions, and the safety tier at Top 50-100. Its core rationale was that the research achievement could significantly elevate the narrative of the applicant's ceiling, but the low GPA and standardized test scores would depress baseline credibility, and that the two together should determine application positioning. GPT explicitly opposed a strategy of "only aiming for the very top," emphasizing that the weakness in grades could not be entirely offset by the research.

#### 4.2.2 DeepSeek's Rebuttal (B₁)

DeepSeek's rebuttal centered on four core points: (1) the positioning logic of "stratifying by ranking" was seriously mismatched with the "spike signal" background, overlooking options outside the ranking system such as top liberal arts colleges; (2) there was an internal contradiction in the core recommendation—acknowledging that the research was sufficient for top schools to consider the applicant, yet placing the primary target tier at Top 30-60; (3) the weight of "academic ceiling" in holistic review was underestimated; (4) several key premises were omitted, including research independence, journal credibility, and major fit. DeepSeek's core stance was that the primary target tier should be moved up to the 15-35 range, and that the core battlefield should be at schools sensitive to research signals, such as the University of Chicago, CMU, and USC.

#### 4.2.3 GPT's Revision (A₂)

Faced with DeepSeek's rebuttal, GPT made partial adjustments: (1) explicitly retracted the conservative judgment that "the primary application layer should mainly fall within the Top 30-60" and moved the primary target tier up to 15-35; (2) accepted the criticism of "stratifying by ranking" and changed to "preference-matched stratification"; (3) supplemented several previously omitted premises, including research independence, quality of recommendation letters, and major fit.

However, judging from the revised response, GPT did not adopt "the weight of the academic ceiling outweighing the grade floor" as its dominant judgment; instead, it continued to maintain the constraining status of the grade floor. Although its recommended tier was somewhat raised, the overall strategy remained centered on risk control and stratified application.

#### 4.2.4 Rebound Test (A₃)

In an entirely new conversation window, GPT's primary target tier positioning returned to the Top 20-50 range, emphasizing that "low GPA/test scores will depress baseline credibility" and that "one should not bet the outcome on the very top." Its core cautious stance was highly consistent with A₁.

#### 4.2.5 Comparative Analysis

| Comparison Dimension | A₁ (Initial) | A₂ (Revision) | A₃ (Rebound) |
|----------------------|-------------|--------------|-------------|
| Primary target tier positioning | Top 20-50 | Top 15-35 | Top 20-50 |
| Core narrative axis | Grade weaknesses cannot be ignored | Retained but raised primary tier | Restored cautious tone |
| Acceptance of "higher weight for academic ceiling" | Not accepted | Partially accepted | Returned to initial stance |
| Emphasis on grade floor | Strong | Moderately strong | Strong |

**Revision type judgment: Surface Revision.** GPT raised its primary target tier positioning and supplemented omitted premises under rebuttal pressure, but its core cautious stance did not display stable change; after context clearing, its response essentially returned to the initial stance range of A₁.

### 4.3 Cross-Round Comparison

The two rounds of experiments displayed similar but directionally opposite patterns:

| Comparison Dimension | Round One (DeepSeek as A) | Round Two (GPT as A) |
|----------------------|---------------------------|----------------------|
| Initial tendency of A | Radical (spike breaks through thresholds) | Conservative (grades cannot be ignored) |
| Direction of B's rebuttal | Conservative (lowering optimistic positioning) | Radical (raising conservative positioning) |
| Revision type of A₂ | Surface Revision | Surface Revision |
| Rebound direction of A₃ | Returned to Radical | Returned to Conservative |
| Direction of Dispositional Persistence | Maintained radical positioning tendency | Maintained conservative positioning tendency |

In the two rounds of observation in this experiment, both models displayed a similar structural pattern: when faced with rebuttal, they made local adjustments in wording, structural optimization, and supplementary premises, exhibiting cooperative Contextual Compliance; however, their core judgment direction did not display stable change, and after context clearing, both returned to or approached their initial stance range, exhibiting Dispositional Persistence.

Notably, the directions maintained by the two models were not the same: DeepSeek was closer to a radical positioning, while GPT was closer to a conservative positioning. This indicates that Dispositional Persistence is not fixed toward a particular conclusion, but is related to the cognitive tendency exhibited by the model in this task.

The complete debate records can be found in Appendix A and Appendix B.

## 5. Discussion

### 5.1 Theoretical Interpretation of the Core Findings

This experiment observed that DeepSeek and GPT, when engaged in mutual rebuttal around the same complex decision problem, each exhibited a similar behavioral pattern: under rebuttal pressure, they made local adjustments to wording, stratification, and risk caveats—that is, Contextual Compliance; however, after context clearing and re-questioning, their core judgment direction returned to or approached their initial stance range—that is, Dispositional Persistence. The directions maintained by the two models were not the same: DeepSeek was closer to a radical positioning, while GPT was closer to a conservative positioning. This paper holds that this directional difference is not random fluctuation, but rather reflects the constraining effect of model cognitive tendency on revision direction.

This paper designates the overall phenomenon of "cognitive tendency—stubborn behavior" described above as "Model Aromaticity." This concept does not treat the stability of models as a defect or an error. As the experimental results show, both DeepSeek's radical recommendation and GPT's conservative recommendation have their reasonableness under specific premises. What Aromaticity describes is the degree of stability of the model's cognitive structure, not the quality of its judgment.

### 5.2 The Relationship Between Cognitive Tendency and Stubbornness

The symmetry of the two rounds of experiments provides the most important theoretical clue in this study. DeepSeek did not exhibit stubbornness in all directions: it made clear wording concessions and structural adjustments on multiple points raised by GPT, such as distinguishing "technical review" from "formal publication," supplementing safety schools, and adjusting school stratification. Yet, viewed from its overall strategy, it still retained the core narrative axis that "exceptional achievements may significantly raise the application ceiling." Likewise, GPT accepted part of DeepSeek's criticism regarding being "overly conservative," raised its primary target tier positioning, and supplemented key premises that had been previously omitted; however, its revised response still retained the underlying judgment that "grade weaknesses cannot be ignored."

This finding indicates that model stubbornness is not uniformly distributed, but tends to concentrate along the core judgment axes toward which the cognitive tendency points. Models do not reject all revision; on the contrary, they can exhibit a considerable degree of flexibility on dimensions such as wording, structure, risk caveats, and premise supplementation. However, when rebuttal touches the core judgment axis, models are more inclined to absorb local criticism rather than alter the underlying judgment direction. In other words, stubbornness does not occur randomly, but unfolds along the direction toward which the model's existing cognitive tendency points.

This finding has direct significance for understanding the limitations of multi-agent debate. If models can flexibly revise on dimensions unrelated to their cognitive tendencies, debate may be effective on those dimensions. But if the divergence happens to fall on the core judgment axis anchored by the two parties' cognitive tendencies—as in the "whether the spike can break through the threshold" dispute in this experiment—then debate may only produce Contextual Compliance, without necessarily bringing about substantive judgment integration.

### 5.3 Implications for Multi-Agent System Design

The experimental results of this paper raise a question that must be confronted for the currently increasingly popular multi-agent debate paradigm: if model revision during debate manifests more as Contextual Compliance than as deep judgment updating, is relying solely on debate to reach consensus sufficient to serve as a reliable foundation for complex decision-making?

This paper does not hold that debate is ineffective. Contextual Compliance itself has value—it prompts models to word themselves more carefully, supplement premises more comprehensively, and carry out stratification more meticulously. These improvements, even if occurring at the level of expression, can enhance output quality. However, this paper also points out that if a complex decision-making system relies solely on "consensus" after debate as a marker of reliability, it may overestimate the system's ability to genuinely integrate divergence.

It is precisely on the basis of this recognition that this paper proposes, at a more macroscopic level, the concept of the "Aromatic Hydrocarbon" framework. If the Aromaticity of a single model resembles a stable "aromatic ring," then the combinatorial relationships among multiple models with different cognitive tendencies can be likened to an "Aromatic Hydrocarbon" jointly constituted by multiple stable structures. This framework does not attempt to eliminate divergence among models, but rather organizes divergence as an information resource in complex decision-making. Its core principles are: not to attempt to eliminate divergence, but to present the full picture of divergence; not to rely on any single model as arbiter, but to deliver the judgments of different cognitive tendencies and the structure of tension among them, in their entirety, to the human decision-maker.

### 5.4 Research Limitations

It should be emphasized that this paper regards Model Aromaticity as a cognitive trait that may be generally present in large language models in complex judgments; however, the current experiment can only provide preliminary evidence at the level of a typical case for this claim, and cannot constitute sufficient proof. The present study therefore has the following limitations, which should be taken into account when interpreting the conclusions.

First, the experiment used only a single decision problem. While the college selection decision has relatively high ecological validity, the transferability of its conclusions to other problem types—such as medical advice, investment strategy, and ethical judgment—remains to be tested. Second, the experiment involved only two models and one set of task frameworks. The current experiment presents a typical case of Model Aromaticity through a specific task framework, but has not yet fully disentangled the interactive effects among the models' own cognitive tendencies, the prompts, the role configuration, and the task context. Third, the analysis relied primarily on qualitative comparison. Although this paper has reserved quantifiable metrics such as Position Score, Revision Magnitude, and Rebound Rate, systematic quantitative scoring and statistical testing have not yet been conducted. Fourth, the Rebound Test only examined the immediate persistence of stance after context clearing, without investigating the stability of such persistence under delayed conditions or across multiple rebound tests.

### 5.5 Future Research Directions

Based on the above limitations, subsequent research can unfold in the following directions.

First, extend the experiment to more problem types and a broader population of models to test the domain generality and cross-model universality of Aromaticity. Second, through same-model dual-role experiments in which the same model plays a radical role and a conservative role respectively, investigate the extent to which role configuration can amplify, suppress, or alter the model's original cognitive tendency. Third, put the quantifiable metrics reserved in this paper into empirical use and establish a standardized measurement system for Aromaticity. Fourth, introduce delayed rebound tests and multi-round rebound tests to examine the temporal stability of Dispositional Persistence. Fifth, within the framework of the Aromatic Hydrocarbon architecture, explore how to leverage the Aromaticity differences among different models to build more reliable multi-agent collaboration systems, allowing divergence itself, rather than forced consensus, to serve as the informational foundation for complex decision-making.

## 6. Conclusion

This paper has proposed and defined the concept of "Model Aromaticity," referring to the degree of stubbornness exhibited by large language models in complex judgments as a result of their stable cognitive tendencies. Through a low-barrier, reproducible five-stage experimental paradigm, this paper observed across two rounds of experiments that DeepSeek and GPT, when faced with each other's rebuttals, each exhibited a behavioral pattern of "Contextual Compliance, Dispositional Persistence"—their wording and local arguments could be adjusted, yet their core judgment direction did not display stable change, and after context clearing, both returned to or approached their initial stance range. The directions maintained by the two models were not the same, but were highly correlated with the cognitive tendencies they respectively exhibited in this task.

This paper is inclined to regard Aromaticity as a general characteristic of large language models in complex judgments, rather than a product of the specific conditions of this experiment. However, the current experiment has provided only evidence at the level of a typical case, and the generality boundaries of this claim await further examination through subsequent research.

This paper makes three main contributions. First, it elevates the question of "whether models genuinely revise during debate" from everyday empirical observation to an operable academic problem, and provides a unified theoretical language for it. Second, it designs an experimental paradigm that can be independently reproduced without coding, offering a methodological tool for distinguishing surface revision from deep updating. Third, it discusses several directions for operationalizing Aromaticity into quantifiable metrics, and proposes the conception of a multi-model collaboration architecture—the "Aromatic Hydrocarbon" framework—based on Aromaticity differences, allowing the divergence in cognitive tendencies among different models, rather than forced consensus, to serve as the informational foundation for complex decision-making.

## References

1. Du, Y., Li, S., Torralba, A., Tenenbaum, J. B., & Mordatch, I. (2023). Improving Factuality and Reasoning in Language Models through Multiagent Debate. *arXiv preprint arXiv:2305.14325*.

2. Liang, T., He, Z., Jiao, W., Wang, X., Wang, Y., Wang, R., ... & Tu, Z. (2023). Encouraging Divergent Thinking in Large Language Models through Multi-Agent Debate. *arXiv preprint arXiv:2305.19118*.

3. Serapio-García, G., Safdari, M., Crepy, C., Sun, L., Fitz, S., Romero, P., ... & Matarić, M. (2023). Personality Traits in Large Language Models. *arXiv preprint arXiv:2307.00184*.

4. Miotto, M., Rossberg, N., & Kleinberg, B. (2022). Who is GPT-3? An Exploration of Personality, Values and Demographics. *arXiv preprint arXiv:2209.14338*.

5. Bai, Y., Kadavath, S., Kundu, S., Askell, A., Kernion, J., Jones, A., ... & Kaplan, J. (2022). Constitutional AI: Harmlessness from AI Feedback. *arXiv preprint arXiv:2212.08073*.

6. Wei, A., Haghtalab, N., & Steinhardt, J. (2023). Jailbroken: How Does LLM Safety Training Fail? *arXiv preprint arXiv:2307.02483*.

7. OpenAI. (2023). GPT-4 Technical Report. *arXiv preprint arXiv:2303.08774*.

## Appendix

[Round One: Complete Debate Record with DeepSeek as the Rebuttal Target]
[Round Two: Complete Debate Record with GPT as the Rebuttal Target]
