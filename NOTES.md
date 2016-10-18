# Notes on DPhil Seminar

---

## Problem Definition
- Convey a comprehensive, yet accessible overview of the work I conducted in the course of my thesis.
- Make the story flow well.
- Provide sufficient but not exhaustive background (also to show off graphs)
- Frame interesting questions

## Fundamental Questions
- How can temporal order arise in self-organised molecular systems?
- How can models help to understand molecular feedback control mechanisms?
- How can we map this decision-making space?
- What are these maps useful for?

---

## Script

### Slide 1.1 - Staging the story
*All cells come from cells* - If you step back for a second and consider this statement, it is remarkable how much weight this statement has:

As adults, our body consists of several trillion cells, yet we start out from a single fertilised egg.

For you to sit here today, innumerable cell divisions have to be executed virtually without errors.

**PAUSE**

Over the last three years, I've been working in Bela Novak's group on a set of projects in this context aimed at shedding more light on a problem, which could be stated in colloquial terms as follows:

*30s*

#### Slide 1.2 - Question in plain words

How do cells make sure that they put on their socks before they put on their shoes?

**PAUSE**

*10s*

### Slide 2.1 - Cell Cycle Overview

Let me elaborate a bit more:

The cell cycle is the process whereby, cells grow, replicate their genetic material and divide.

For metazoans, we divide it into four stages: the gap phases G1 and G2 - when the cell primarily grow; S-phase - when the DNA is replicated and mitosis - when the nucleus is divided.

In my work I focus on the regulation of mitosis, where it is absolutely crucial that things happen in order:

1. In cells undergoing open mitosis first the DNA becomes condensed. At this stage, sister chromatids, that is to say corresponding copies of chromosomes are held together by the ring-shaped cohesin complex. An apparatus of microtubules motor proteins begins to organise around centrosomes. Finally, the nuclear envelope is disassembled, and **Prophase** has ended.

2. Next - in **Prometaphase** the mircotubules begin to invade the centre of the cell capture pairs of sister chromatids by binding to large protein complexes called kinetochores that assemble in the centromeric region of each chromatid.

3. Once corresponding sisters have become attachced to opposite poles of the spindle, the chromatids are said to have become bi-oriented; the hallmark of **Metaphase**.

4. In **Anaphase**, the cohesin is cleaved and sister chromatids are separated towards opposite poles of the spindle, by pole-ward pulling forces within the spindle, as well as pushing forces from bundles of microtubules that nucleate between the separating sisters.

5. This so-called central spindle also serves the purpose of determining the position of the equator of the cell in **Telophase**, when the cell membrane begins to gradually invade the equatorial plane, while the cell elongates.
Moreover, **Telophase** can be understood as prophase in reverse: The nuclear envelope is reassembled on the chromatin, which in turn becomes decondensed.

*90s*
*total: 2:10*

#### Slide 2.2 - Reframe question

Do you spot the issue with this all too smooth description of this process?
Cells encode the identity of chromatids topologically, by tying corresponding sisters together, and breaks these ties only if the mitotic spindle can pull them apart correctly.

If sister chromatid cohesion were lost prematurely - before biorientation - the information of "belonging-ness" of chromatids would be lost, with potentially grave consequences for the cell.

This is only one prominent example! Likewise, reassembling the nuclear envelope before separation of the sister chromatids would be problematic.

SO: How can temporal order and control arise in self-organised molecular systems?

*40s*

#### Slide 2.3 - Extra Slide for Dramatic Effect

A very general answer to this question is **Feedback Control**

*10s*

*total: 3:00*

### Slide 3.1 - Mitotic Checkpoint

Cells have evolved an intricate feedback control system, which I shall call the Mitotic Checkpoint. It delays progression into anaphase until all pairs of sisters have become bioriented.

This checkpoint consists of two sub-modules: a surveillance and error correction system, and a checkpoint enforcement mechanism.

The error corretion module monitors the attachment state of each chromatid pair and destabilises incorrect attachments. The checkpoint enforcement mechanism produces a soluble inhibitor that prevents premature initiation of anaphase.

The field on this topic is quite big, and thanks to momentuous effort, we know a lot about the molecular basis of the mitotic checkpoint...

*30s*

#### Slide 3.2 - Error Correction
To destabilise incorrect attachment configuration, such as
- monotelic
- syntelic
- merotelic
Error Correction must integrate the attachment state of the kinetochore on each of the two sisters. This is achieved through a tension-sensitive mechanism:

Aurora B kinase, which is part of the chromosomal passenger complex, phosphorylates the binding interface between kinetochores and microtubules.
It thus abolishes the electrostatic interaction between kinetochore and microtubule and destabilises the attachment.

Only correct, amphitelic attachment configuration will experience equal drag from the two poles of the mitotic spindle. This results in a sufficiently strong deformation of the kinetochore, that the phosphorylation targets are displaced out of reach of the sharp aurora b activity gradient.

This provides a mechanism that biases the attachment process towards the formation of correct attachment.

*40s*

#### Slide 3.3 - Checkpoint effector 1

To be effective at delaying anaphase until error correction the checkpoint requires a mechanism to signal incomplete biorientation to the molecular machinery that drives anaphase.

*10s*

#### Slide 3.4 - Checkpoint effector 2

Anaphase is initiated by the activation of the E3 ubiquitin ligase anaphase promoting complex/cyclosome (APC/C) by its co-activator Cdc20. This confers it with susbtrate specificity towards it's early anaphase substrates cyclin B and securin and allows it to target them for proteasomal degradation.
Securin acts as chaperone and stoichiometric inhibitor of separase, which promotes the segragation of sister chromatids as specific protease to cohesin.
Cyclin B is the crucial activator of the mitotic cyclin-dependent kinase, CDK1, whose activity high in mitosis and crucial in maintaining the mitotic state.

*30s*

#### Slide 3.5 - Checkpoint effector 3

To delay the singular event of APC/C:Cdc20 activation that drives the cell into anaphase in a manner that gives the error correction time to promote amphitelic attachments, cells produce a soluble inhibitor called mitotic checkpoint complex (MCC).

If unattached kinetochores are present, the checkpoint is active.
They serve as catalytic platforms in the assembly of MCC, which - once assembled - binds very tightly to APC/C, and acts as a stoichiometric inhibitor.

In prometaphase the rate of production of MCC by unattached kinetochores is sufficiently high that a single unattached kinetochore is sufficient to delay the onset of anaphase.

Once all chromosomes have become attached, the checkpoint is satisfied, the  assembly of MCC from its components ceases, and a set of processes directing the disassembly of MCC remove the APC/C-inhibitor in metaphase, and lead to timely activation of APC/C.
Noteably, the checkpoint retains the capacity to become re-engaged when it is satisfied. Only after the onset of anaphase does it become irreversibly inactivated.

*45s*

*total: 5:35*

### Slide 4.1 - Systems-Level Perspective

As with any description of a biological system that suggests an all to neat and clean picture, this description should give you reason for scepticism!

There are plenty of conceptual problems associated with this description:

*10s*

#### Slide 4.2 - Scale

The first problem has to do with scale: It is easy to show two pictures side-by-side: One, representing the cell say in anaphase, and another one showing how APC/C degrades cyclin B. This may implicitly imply a connection, but it is not spelled out.

How can we connect the molecular state with the cellular state? - What do prometphase, metaphase and anaphase correspond to in terms of molecular signalling?

*25s*

#### Slide 4.3 - State

The second problem has to do with the state of a system.

What does it mean on molecular level, if we say checkpoint is on or off, signalling or satisfied?

*20s*

#### Slide 4.4 - Identity

Despite having presented them as entirely distinct entities, error correction and checkpoint effector are intimately interconnected.
Error correction produces the unattached kinetochores and thereby generates the very signal the checkpoint effector responds to.
In turn, the checkpoint effector stabilises the activity of many upstream kinases such as Cdk1, Aurora B and Mps1 that are required for the activity of both error correction and checkpoint effector modules.

If we talk about error correction and checkpoint effector module, are these really two different things? Where does error correction end and the checkpoint effector module begin?
And is this question even relevant?

*40s*

#### Slide 4.5 - Dissemination

In the diagram I showed you before, anaphase is represented merely by degradation of cyclin B and securin and the consecutive cleavage of cohesin. Yet many processes have to be executed in well-timed manner for a cell to successfully exit from mitosis.

How is the decision to exit mitosis broadcast?
...and how is correct timing ensured beyond the control of the mitotic checkpoint?

*20s*
*total: 7:30*

### Slide 5.1 - Models, Maps and Iteration
Again, I would claim the answer to these questions lies in a feedback system. Now it is composed of  data-driven modelling and model-driven experimentation. This was the approach I employed in three projects aimed at deepening our understanding of the mitotic checkpoint.

*20s*

#### Slide 5.2 - Experiments and Simulation
- experimental data-driven
- formulate hypothesis
- simulate, and bring into agreement
- show model that displays bistability

#### Slide 5.3 - Mapping
- construct maps model that allow us to understand the abstract decision-making space in terms of steady states of the molecular regulators

#### Slide 5.4 - Interpretation

### Slide 6.1 - Crosstalk

#### Slide 6.2 - Question

#### Slide 6.3 - Timing

#### Slide 6.4 - Imaging

#### Slide 6.5 - Tracking

#### Slide 6.6 - Model

#### Slide 6.7 - Simulation

#### Slide 6.5 - Testing

#### Slide 6.6 - Summary

### Slide 7.1 Mapping Metaphase

### Slide 8.1 Heuristic
