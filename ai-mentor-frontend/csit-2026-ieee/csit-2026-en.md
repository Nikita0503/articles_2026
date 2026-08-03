# Artificial Intelligence as a Personal Mentor in Frontend Development Education: Methodology and Experimental Results

**Authors:**

| | Author 1 (Primary) | Author 2 (Co-author) |
|---|---|---|
| Name | [YOUR FULL NAME] | [CO-AUTHOR FULL NAME] |
| Position | Assistant Lecturer | Student |
| Department | Department of Virtual Reality Systems, Institute of Computer Science and Information Technologies | Department of Virtual Reality Systems, Institute of Computer Science and Information Technologies |
| Affiliation | Lviv Polytechnic National University | Lviv Polytechnic National University |
| City, Country | Lviv, Ukraine | Lviv, Ukraine |
| Email | [your@email.com] | [coauthor@email.com] |
| ORCID (optional) | [0000-0000-0000-0000] | [0000-0000-0000-0000] |

## Abstract

This paper investigates the use of large language models (LLMs) as personal mentors for students learning frontend development in higher education institutions. We propose a methodology based on the cyclical model "theory → practice → reflection" with AI support at each stage, where AI generates personalized learning projects, provides contextual guidance within the student's development environment, and delivers feedback without providing ready-made solutions. An experimental evaluation with a group of 5 students demonstrated high effectiveness of the approach: AI mentor received the highest usefulness rating (4.8 out of 5) among all components of the learning process. The results confirm the feasibility of integrating AI mentorship into computer science education as a scalable, cost-free, and always-available complement to traditional teaching methods.

**Keywords:** artificial intelligence, mentoring, frontend development, programming education, large language models, higher education.

---

## I. Introduction

The modern IT labor market demands that frontend developers possess not only knowledge of programming language syntax but also understanding of architectural patterns, experience with real APIs, version control systems, and the ability to independently solve complex technical problems. According to the Stack Overflow Developer Survey 2025, 44% of developers used AI-enabled tools for learning new technologies, an increase of 7 percentage points from the previous year [1].

Traditional higher education does not always provide the required level of practical preparation. Lecture formats build theoretical foundations but do not develop skills for independent problem-solving in real-world contexts. Laboratory assignments are typically isolated exercises that do not reflect the complexity of commercial development. Online courses offer structured learning but often reduce to passive repetition of instructor actions.

Classical mentorship is recognized as one of the most effective methods for learning programming [2]. An experienced mentor adapts explanations to the student's level, provides personalized feedback, and guides toward correct solutions without providing ready-made answers. However, mentorship is expensive, limited in time, and does not scale — one mentor cannot physically support dozens of students simultaneously.

The development of large language models (LLMs) opens fundamentally new possibilities for addressing this problem. Modern AI systems can perform key mentor functions: explaining concepts, generating learning tasks, analyzing code, and preparing students for technical interviews — while remaining free (within free-tier limits), available 24/7, and capable of adapting to the context of the student's specific project. Research published in Nature (2025) confirms that students learning with AI tutors acquire material faster and demonstrate higher motivation compared to traditional formats [3].

The objective of this paper is to propose and validate a methodology for using AI as a personal mentor in frontend development education.

---

## II. Problem Statement

Analysis of junior frontend developer vacancies reveals typical employer requirements: proficiency in JavaScript/TypeScript, experience with React (hooks, state management, routing), understanding of REST APIs, Git workflow, and ability to work with existing codebases. Comparison of these requirements with typical university curricula reveals a significant gap: academic courses focus on fundamental disciplines (algorithms, data structures) that form a necessary foundation but do not provide practical experience with modern frameworks and tools.

Existing learning formats have notable limitations. Lectures and laboratory work provide structured material delivery but have a fixed pace and do not adapt to individual student levels. Online courses predominantly follow the "repeat after instructor" format — students reproduce code from video but do not develop independent problem-solving skills. Self-directed learning from documentation requires high self-organization and prior experience that beginners typically lack.

Individual mentorship addresses these limitations effectively [2] by adapting explanations, providing code review, guiding without giving direct answers, and supporting motivation. However, it remains financially expensive, time-limited, subjective (dependent on specific mentor competence), and non-reproducible.

These constraints create a demand for an approach that combines the personalization and adaptiveness of mentorship with the scalability and accessibility of digital tools.

---

## III. AI as a Mentor: Capabilities and Limitations

Modern LLMs have demonstrated the capability to effectively perform functions traditionally belonging to mentor competence [4, 5]:

1) **Concept explanation.** AI can explain any frontend development concept adaptively — from basic to advanced level, with analogies, examples, and repeated explanations from different angles. Unlike a human mentor, AI does not tire and is ready to explain the same concept repeatedly without frustration.

2) **Task generation.** AI can create practical tasks of appropriate difficulty: from simple (implement a component by description) to complex (design an authorization module architecture). Tasks are generated with detailed acceptance criteria, enabling students to self-evaluate results.

3) **Code analysis and feedback.** AI analyzes student-written code, identifies potential problems (principle violations, suboptimal solutions, potential bugs) and suggests improvement directions — without providing ready-made code.

4) **Interview preparation.** AI models the format of technical interviews: asks typical questions, analyzes student responses, and identifies gaps in understanding.

5) **Architectural consulting.** When working on projects, AI helps make architectural decisions: file structure, component responsibility distribution, library selection, state management patterns.

**Key advantages** of AI mentorship include: zero cost (free-tier LLM plans are sufficient for learning purposes), 24/7 availability, unlimited patience (willing to explain the same concept indefinitely without judgment), personalization through project context (in smart IDE environments, AI has access to student's code structure and current errors), and development of independence (AI guides rather than provides answers).

**Limitations** include possible generation of incorrect information (hallucinations), risk of dependency formation with insufficient self-discipline, and necessity to verify responses. However, these risks should be evaluated in context: an incorrect AI response costs the student 20–30 minutes of additional debugging, whereas absence of any mentorship costs weeks of stagnation and potential motivation loss. Moreover, the skill of critically evaluating AI output is itself a valuable professional competency for modern developers [1].

**Requirements for the student:** self-direction (AI guides, but the student writes code), desire to understand (ask clarifying questions rather than copying first results), discipline (regular practice), critical thinking (verify AI responses against documentation), and initiative (formulate specific questions with context).

---

## IV. Proposed Methodology

The proposed methodology is based on a cyclical model: **theory → practice → reflection**, where AI provides support at each stage (Table I).

**Table I. Cyclical Learning Model with AI Mentor**

| Stage | Student Activity | AI Mentor Role |
|-------|-----------------|----------------|
| Theory | Studies new concept, asks questions | Explains, provides analogies, adapts complexity, re-explains from different angles |
| Practice | Writes code independently | Consults, gives hints, asks guiding questions, does NOT write code |
| Reflection | Presents result for analysis | Provides feedback, identifies problems, suggests improvements |

The cycle repeats for each new concept or sprint.

### A. AI as Learning Environment Generator

The central element of the methodology is that AI not only mentors but also **generates the personalized learning project** for the student:

1) The student selects a project domain ("task manager," "online store," "blog platform") or asks AI to propose a project of appropriate complexity.
2) AI designs the architecture: defines pages, components, API endpoints, data model.
3) AI divides the project into sprints with progressive complexity and creates structured tasks with detailed acceptance scenarios.
4) The student executes tasks sequentially; AI mentors during execution.
5) After each task completion, AI analyzes the result and provides feedback.

This approach simulates a real IT company workflow: a developer receives a task with requirement description, implements it independently, and undergoes code review.

### B. Contextualization in Smart IDE

The AI mentor operates directly within the student's development environment (smart IDE). It has access to: project structure (files, directories, dependencies), technology stack and configuration, current student code and changes, and current sprint task descriptions.

This enables contextual responses. For example, to the question "How do I implement a protected route?" — AI responds considering the specific structure of the student's router, libraries used, and existing authorization code, rather than providing an abstract documentation example.

### C. Interview Preparation and Pet Projects

AI effectively models technical interview format for frontend developers: theoretical questions, practical coding tasks, and architectural discussions. For pet projects, AI serves as an architectural advisor and reviewer — helping choose technologies, reviewing project structure, analyzing written code, and suggesting new features for expansion.

The key principle throughout: AI explains concepts, indicates direction, asks guiding questions — but does not generate ready-made code for copying. The student writes every line independently.

---

## V. Experimental Evaluation

### A. Experimental Setup

To validate the proposed methodology, a learning platform was developed implementing the described principles. The platform represents a full-featured software project — a task manager built on a modern technology stack (React, TypeScript, Redux Toolkit, REST API).

The project is organized using a sprint model with progressive complexity:
- **Sprint 1** — Authorization: registration, login, JWT tokens, protected routes;
- **Sprint 2** — Data reading: list display, user profile, error handling, loading states;
- **Sprint 3** — Full CRUD: create, edit, delete tasks, file handling, pagination;
- **Sprint 4** — Extended functionality: priorities, redesign, additional filters.

Each sprint contains structured tasks with detailed acceptance scenarios (happy path, error handling, edge cases), simulating the format of commercial development work.

A pilot evaluation was conducted with a group of 5 students. Participant profile: basic knowledge of JavaScript and React, no commercial development experience. Participants completed platform tasks (sprints 1–4) using an AI mentor in a smart IDE over a 4-week period.

### B. Results

Evaluation was performed across four criteria (Table II).

**Table II. Pilot Testing Results (n=5)**

| Criterion | Mean | Min | Max |
|-----------|:----:|:---:|:---:|
| Sprint 1 completion time (days) | 4.2 | 3 | 6 |
| Task clarity (1–5) | 4.4 | 4 | 5 |
| AI mentor usefulness (1–5) | 4.8 | 4 | 5 |
| Work readiness self-assessment (1–5) | 4.0 | 3 | 5 |

The AI mentor received the highest rating among all criteria (4.8/5), indicating its perception by students as the most valuable element of the learning process.

### C. Qualitative Feedback

Participants noted the following aspects of AI mentor interaction:
- ability to receive explanations at any time without waiting;
- contextual responses — AI understood their project structure;
- absence of psychological pressure — ability to ask "basic" questions without embarrassment;
- usefulness in error analysis — AI explained error causes in the context of specific files.

Participant recommendations included: adding more visual examples of expected results, and increasing the number of sprints with more complex topics (WebSocket, real-time updates).

---

## VI. Comparison with Traditional Approaches

**Table III. Comparison of Approaches to Programming Education**

| Criterion | Lectures | Online Courses | Human Mentor | AI Mentor |
|-----------|:--------:|:--------------:|:------------:|:---------:|
| Time availability | Scheduled | 24/7 | By appointment | 24/7 |
| Cost | Included in tuition | Free/paid | Expensive | Free |
| Personalization | Low | Low | High | High |
| Scalability | Medium | High | Low | High |
| Feedback quality | Limited | Absent/auto | High quality | High quality |
| Explanation adaptiveness | Low | None | High | High |
| Patience | Limited | — | Limited | Unlimited |
| Project context awareness | No | No | Yes | Yes |

The comparison demonstrates that AI mentorship combines the key advantages of human mentorship (personalization, high-quality feedback, project context) with the advantages of digital platforms (scalability, availability, zero cost).

---

## VII. Conclusions

This paper investigated the use of LLM-based artificial intelligence as a personal mentor for frontend development students. The main contributions are:

1) We identified the gap between academic preparation and market requirements for frontend developers, as well as limitations of existing learning formats.

2) We theoretically justified the capability of modern LLMs to perform key mentor functions and analyzed advantages, limitations, and requirements for effective use.

3) We proposed a methodology based on the "theory → practice → reflection" cycle with AI support at each stage, including AI generation of personalized learning environments (project, sprints, tasks).

4) We described a practical implementation using a sprint-based learning platform with a contextualized AI mentor in a smart IDE.

5) Experimental evaluation confirmed the approach effectiveness: the AI mentor received the highest usefulness rating (4.8 out of 5) among all learning process components.

**Practical implications.** AI mentorship can be integrated into higher education as a complement to existing formats: students use AI for independent practice between laboratory sessions, exam preparation, and pet project development. The instructor's role transforms from knowledge carrier to learning process curator who monitors progress and verifies results.

**Future work** includes conducting a comparative experiment with a control group (without AI mentor), increasing participant sample size, investigating effectiveness for other development directions (backend, mobile), and developing quality assessment criteria for AI mentorship.

---

## References

[1] "Stack Overflow Developer Survey 2025," Stack Overflow, 2025. [Online]. Available: https://survey.stackoverflow.co/2025/

[2] A. Begel and B. Simon, "Novice software developers, all over again," in *Proc. ICER '08*, 2008, pp. 3–14.

[3] "AI tutoring outperforms in-class active learning: an RCT introducing a novel research-based design in an authentic educational setting," *Nature Scientific Reports*, vol. 15, 17458, 2025.

[4] S. Kazemitabaar et al., "Studying the effect of AI Code Generators on Supporting Novice Learners in Introductory Programming," in *Proc. CHI '23*, 2023.

[5] "A Systematic Review of Chatbots, Generative Tools, and Tutoring Systems in Programming Education," *arXiv preprint*, arXiv:2510.03884, 2025.

[6] "The Influence of Artificial Intelligence Tools on Learning Outcomes in Computer Programming: A Meta-Analysis," *Computers*, vol. 14, no. 5, 185, 2025.

[7] "AI-mediated feedback in gamified programming education: effects on vocational students' achievement and motivation," *Frontiers in Education*, vol. 11, 1846699, 2026.

[8] "What the research shows about generative AI in tutoring," Brookings Institution, 2025. [Online]. Available: https://www.brookings.edu/articles/what-the-research-shows-about-generative-ai-in-tutoring/
