# Detailed Plan: SLT

## Overall Goal

To conduct an initial exploration into the field of Singular Learning Theory (SLT) by personally following Roma's introductory program. The aim is to master the fundamentals and key ideas of SLT and its associated mathematics (as much as possible) within a 3-month internship. The outcome will be a structured understanding of the covered area, documentation of the practical skills acquired, and a report with recommendations for improving the original curriculum.

## Areas of Development and Their Metrics

### Theory
- **Objective (Why):** To learn a certain number of (mathematical) concepts around SLT (e.g., the Bayesian approach to generalization, the concept of singular models, RLCT, etc.) and related fields (elements of algebraic geometry?). To be able to explain them.
- **Metric (What to look at):** The number of new models, concepts, and connections between them.
- **Expected Outcome (How to measure):**
    - A research log on GitHub tracking work progress.
    - Presentations (and their slides) on the topics studied.

### Practice
- **Objectives:**
    - To be able to solve a number of exercises on SLT.
    - To be able to write code relevant to an SLT task.
    - To be able to replicate existing research.
- **Metric:**
    - The number of exercises solved.
    - The number of Timaeus notebooks completed.
    - Progress on research tasks (how many studies were reproduced and/or extended, developed from an idea, etc.).
- **Expected Outcome (How to measure):** The research log on GitHub will document: completed exercises (or documented failures), replications, and research ideas.

### Research Taste
- **Objective:** To be able to formulate a hypothesis that seems meaningful and interesting to test within the SLT/DevInterp agenda.
- **Metric:** The number of generated research ideas that are reasonably meaningful.
- **Expected Outcome (How to measure):** The research log on GitHub will document: ideas for pet projects and feedback on their meaningfulness from the mentor and a focus group.

## Outcomes and Reporting
- A completed research log on GitHub for 80 hours of work (filled out as the individual development plan progresses).
- Mini-presentations on the topics studied (intermediate results).
- A brief report with feedback on the time spent, results achieved, and suggestions for improving the SLT introductory plan (to be provided to the curriculum's author).
- A final presentation to the Monoid group on what was learned, with a reflection on the experience of being both a mentor and mentee in the program.

---

## Work Plan by Stages

### Stage 1: Foundation and Intuition

#### Module 1.1: Introduction to Singular Learning Theory and Basic Preparation

**Task: Read introductory articles and share them with the world. Part 1**
- **Deadline:** Week 1
- **Description:** Read and take notes on "One Weird Trick" and "Dialogue introduction".
- **Resources:**
    - ["One Weird Trick"](https://www.lesswrong.com/posts/fovfuFdpuEwQzJu2w/neural-networks-generalize-because-of-this-one-weird-trick)
    - ["Dialogue introduction"](https://www.lesswrong.com/posts/CmcarN6fGgTGwGuFp/dialogue-introduction-to-singular-learning-theory)
    - My GitHub project: https://github.com/meriton-s/slt_intro
- **Expected Outcome:** I can explain what the articles are about, what high-level problem they are trying to solve, and the main ideas of the solution and related concepts.
- **Hours:** 3 + 3 hours
- **Deliverables:**
    - A summary with the main points of the articles.
    - A concept map/diagram (e.g., in Miro) with key ideas and their connections.
    - A presentation for a talk at Monoid or Minimizers.
- **Checkpoint:** Explain my understanding of the articles (to the mentor, at Monoid, or Minimizers). Gather feedback to ensure key ideas are correctly understood before moving on.

**Task: Build grounded intuitions (code)**
- **Deadline:** Week 2
- **Description:**
    - Write simple code to visualize the loss landscape for a simple neural network on a simple dataset.
    - Experiment with different initializations and see how the landscape changes.
- **Resources:**
    - My GitHub project: https://github.com/meriton-s/slt_intro
    - Inspiration links:
        - [Loss Landscape Library](https://github.com/tomgoldstein/loss-landscape)
        - [Visualizing the Loss Landscape of Neural Nets (Paper)](https://arxiv.org/abs/1712.09913)
- **Expected Outcome:** I can write a script that generates 2D/3D plots illustrating the main ideas from the articles.
- **Hours:** 6 hours
- **Deliverables:**
    - The script's code on GitHub.
    - A progress entry in the research log.

#### Module 1.2: Further Reading and Thinking in SLT Models

**Task: Read introductory articles and share them with the world. Part 2**
- **Deadline:** Week 2
- **Description:** Read and take notes.
- **Resources:**
    - ["You're measuring model complexity wrong"](https://www.lesswrong.com/posts/6g8cAftfQufLmFDYT/you-re-measuring-model-complexity-wrong)
    - ["Distilling Singular Learning Theory"](https://www.lesswrong.com/s/czrXjvCLsqGepybHC)
    - My GitHub project: https://github.com/meriton-s/slt_intro
- **Expected Outcome:** I can explain what the articles are about, what high-level problem they are trying to solve, and the main ideas of the solution and related concepts.
- **Hours:** 6 hours
- **Deliverables:**
    - A summary with the main points of the articles.
    - A concept map/diagram (e.g., in Miro) with key ideas and their connections.
    - A presentation for a talk at Monoid.

**Task: Work through non-educational articles**
- **Deadline:** Week 3
- **Description:** Read and take notes.
- **Resources:**
    - [Liam Carroll’s MSc thesis, "Phase transitions in neural networks"](http://therisingsea.org/notes/MSc-Carroll.pdf)
    - [S. Wei, et al. “Deep learning is singular, and that’s good”](https://arxiv.org/abs/2208.06283)
    - My GitHub project: https://github.com/meriton-s/slt_intro
- **Expected Outcome:** I can explain what the articles are about, what high-level problem they are trying to solve, and the main ideas of the solution and related concepts.
- **Hours:** 10 hours
- **Deliverables:**
    - A summary with the main points of the articles.
    - A concept map/diagram (e.g., in Miro) with key ideas and their connections.
    - A presentation for a talk at Monoid or Minimizers.
- **Checkpoint:** Explain my understanding of the articles (to the mentor, at Monoid, or Minimizers). Gather feedback to ensure key ideas are correctly understood before moving on.

---

### Stage 2: Practice and Extended Theory

#### Module 2.1: Theory
*(Note: Maybe these tasks can be done in parallel: read a few chapters, work through some seminars, then more chapters?)*

**Task: Build the mathematical foundation – Watanabe**
- **Deadline:** Weeks 5-8
- **Description:**
    - Do a surface reading of S. Watanabe’s “Algebraic geometry and statistical learning theory”.
    - Focus on the first chapters to understand the basic apparatus.
- **Resources:**
    - [Book link (Anna's Archive)](https://annas-archive.org/md5/2967fdaab00856c4b5573a816f5a4f25)
    - My GitHub project: https://github.com/meriton-s/slt_intro
- **Expected Outcome:** I don't understand anything, but it's very interesting.
- **Hours:** 10
- **Deliverables:** TO DO

**Task: Work through the Metauni seminars**
- **Deadline:** Weeks 5-8
- **Description:**
    - After reading the book, watch the seminar recordings to reinforce and deepen understanding OR watch the seminar after reading a chapter OR read the chapter after watching the seminar.
    - Focus on topics that were difficult during the reading.
- **Resources:**
    - [Metauni seminars](https://metauni.org/slt/)
- **Expected Outcome:** I don't understand anything, but it's very interesting.
- **Hours:** 10
- **Deliverables:**
    - A summary with the main points of the seminars.
    - A concept map/diagram (e.g., in Miro) with key ideas and their connections.
    - A presentation for a talk at Monoid or Minimizers.
- **Checkpoint:** Explain my understanding (to the mentor, at Monoid, or Minimizers). Gather feedback.

#### Module 2.2: Exercises

**Task: Read the distilled version of Watanabe's book on SLT**
- **Deadline:** Weeks 5-8
- **Resources:** ["Distilling Singular Learning Theory"](https://www.lesswrong.com/s/czrXjvCLsqGepybHC)
- **Expected Outcome:** I don't understand anything, but it's very interesting.
- **Hours:** 10
- **Deliverables:**
    - A presentation for a talk at Monoid titled "Mathematical Foundations of SLT".
    - A final report (2-3 pages) on "My Understanding of SLT" (updated after the Monoid presentation).

**Task: Solve exercises**
- **Deadline:** Week 9
- **Description:**
    - Solve exercises on SLT.
    - *Comment from Oleg:* 19 exercises, most with 2-3 parts. 40 minutes per exercise. This seems about right assuming general knowledge of the theory (i.e., assuming one might need to reread sections, but not that one learns of these sections from the problem statement).
    - *Recommendation:* Track time. If exercises take longer, skip those not marked with asterisks.
- **Resources:**
    - ["Singular learning theory: exercises"](https://www.lesswrong.com/posts/3HYqTAi4kD35G3BzQ/singular-learning-theory-exercises)
    - My GitHub project: https://github.com/meriton-s/slt_intro
- **Expected Outcome:** I don't understand anything, but it's very interesting.
- **Hours:** 10
- **Deliverables:**
    - A document with solutions and notes for each exercise.

**Task: Work through the video lecture from Timaeus**
- **Deadline:** Week 10
- **Description:** Watch and take notes.
- **Resources:**
    - ["DevInterp Conference 2023 - The Plan / Open Problems"](https://www.youtube.com/watch?v=Otv_FODM-hE)
- **Expected Outcome:** I don't understand anything, but it's very interesting.
- **Hours:** 2
- **Deliverables:**
    - A summary with the main points of the lecture.
    - A concept map/diagram (e.g., in Miro) with key ideas and their connections.
    - A presentation for a talk at Monoid or Minimizers.
- **Checkpoint:** Discuss the solution with Anton.

#### Module 2.3: Code

**Task: Go through the Colab notebooks on SLT**
- **Deadline:** Week 11
- **Description:** Go through all notebooks from Timaeus (from [timaeus.co/projects](https://timaeus.co/projects)) up to and including "Toy Landscapes".
- **Resources:**
    - [Introduction](https://colab.research.google.com/github/timaeus-research/devinterp/blob/main/examples/introduction.ipynb)
    - [Calibration](https://colab.research.google.com/github/timaeus-research/devinterp/blob/main/examples/sgld_calibration.ipynb)
    - [Diagnostics](https://colab.research.google.com/github/timaeus-research/devinterp/blob/main/examples/diagnostics.ipynb)
    - [Toy Landscapes (normal crossing singularities)](https://colab.research.google.com/github/timaeus-research/devinterp/blob/main/examples/normal_crossing.ipynb)
- **Expected Outcome:** TO DO
- **Hours:** 8
- **Deliverables:**
    - Code on GitHub.
    - A progress entry in the research log.

***Task: Conduct some kind of learning event based on notebooks 1-4 (?)***
- **Deadline:** TO DO
- **Description:** TO DO
- **Resources:** TO DO
- **Expected Outcome:** TO DO
- **Hours:** TO DO
- **Deliverables:** TO DO

---

### Stage 3: Research

#### Module 3.1: Educational Code

**Task: Complete the notebook on investigating the MNIST landscape**
- **Deadline:** Week 12
- **Description:** Go through the notebook.
- **Resources:**
    - [mnist.ipynb - Colab](https://colab.research.google.com/github/timaeus-research/devinterp/blob/main/examples/mnist.ipynb)
- **Expected Outcome:** I don't understand anything, but it's very interesting.
- **Hours:** 4
- **Deliverables:**
    - Code on GitHub.
    - A progress entry in the research log.

#### Module 3.2: Replication

**Task: Replicate the results of the "Easy" project from Timaeus**
- **Deadline:** Week 12
- **Description:** Set a deadline of 8 total hours for the "Easy" project. If not completed within this time, set it aside and at least start the "Medium" project.
- **Resources:**
    - My GitHub project: https://github.com/meriton-s/slt_intro
    - Project descriptions: [https://timaeus.co/projects](https://timaeus.co/projects)
- **Expected Outcome:**
    - Code and data that fully reproduce the results of the "Easy" project.
    - OR: some code and a detailed report on the problems encountered and the work done.
- **Hours:** 8 hours
- **Deliverables:**
    - Code on GitHub.
    - A progress entry in the research log.

**Task: Replicate the results of the "Medium" project from Timaeus**
- **Deadline:** Week 12
- **Description:** Set a deadline of 12 total hours for the project. If not completed, set it aside and try to come up with my own project.
- **Resources:**
    - Project descriptions: [https://timaeus.co/projects](https://timaeus.co/projects)
- **Expected Outcome:**
    - Environment is set up, data is loaded, first steps toward replication are taken.
    - A detailed report on the problems encountered and the work done.
- **Hours:** 12 hours
- **Deliverables:**
    - Code on GitHub.
    - A progress entry in the research log.

#### Module 3.3: Pet Project

***Task: Formulate my own small research question and create a research plan for it.***
- **Deadline:** TO DO
- **Description:**
    - Brainstorm project ideas.
    - Discuss the weak points of the proposed ideas (take notes, trace the sources of bad ideas, write a reflection on this).
    - Select/refine the top 3 ideas.
    - Choose 1 and write a research plan for it.
- **Resources:**
    - My GitHub project: https://github.com/meriton-s/slt_intro
- **Expected Outcome:** I can generate somewhat interesting project ideas and create a research plan for them.
- **Hours:** TO DO
- **Deliverables:**
    - A list of project ideas.
    - Reflection after feedback on the projects (from Oleg and maybe others if needed).
    - A research plan.

***Task: Implement the pet project.***
- **Deadline:** TO DO
- **Description:** Choose an unfinished project from Timaeus or a small idea of my own and implement it, either alone or in a team.
- **Resources:**
    - [https://timaeus.co/projects](https://timaeus.co/projects)
    - My GitHub project: https://github.com/meriton-s/slt_intro
- **Expected Outcome:** I can complete a pet project on SLT.
- **Hours:** 21 hours (4 days: 4+7+7+3 hours)
- **Deliverables:**
    - Code on GitHub.
    - A report in the research log: hypothesis, methodology, intermediate results, and a plan for next steps.

***Task: Conduct a hackathon***
- **Deadline:** TO DO
- **Description:** TO DO
- **Resources:** TO DO
- **Expected Outcome:** TO DO
- **Hours:** TO DO
- **Deliverables:** TO DO

---

### Stage 4: Summarizing

- **Task:** Show the results to Oleg and discuss them.
  - **Deadline:** Week 13

- **Task:** Prepare feedback for Roma on his educational program.
  - **Deadline:** Week 13

- **Task:** Prepare a final presentation for the Monoid group on the results of the individual development plan.
  - **Deadline:** November 1