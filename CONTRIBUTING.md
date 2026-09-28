# Contributing to Unfloat AI

Unfloat AI is currently a private research and engineering organization.

Our research and source code are maintained privately while the project is being developed.

These guidelines describe the principles we use when developing and researching internally. They may evolve as the organization grows.

---

# Research First

Unfloat is a research project as well as a software project.

Our objective is to investigate whether fundamentally discrete numerical approaches can provide useful advantages for machine learning.

We should distinguish between:

### Hypothesis

Something we think might be true.

### Experiment

Something we test.

### Result

What actually happened.

### Interpretation

What we think the result means.

### Conclusion

What the available evidence supports.

These should not be treated as interchangeable.

A promising prototype is evidence that something is worth investigating, not proof that the underlying approach is superior.

---

# Evidence Over Assumptions

Technical claims should be supported by experiments whenever practical.

When evaluating an approach, relevant measurements may include:

* Accuracy
* Training time
* Inference time
* Memory usage
* Model size
* Computational requirements
* Convergence behaviour
* Numerical error
* Hardware requirements
* Energy consumption where measurable

The exact measurements depend on the experiment.

An approach should not be considered successful merely because it works on a small demonstration.

---

# Reproducibility

Important experiments should record enough information for another member of the team to understand and reproduce the result.

Depending on the experiment, this may include:

* Model architecture
* Dataset
* Numerical representation
* Training configuration
* Hardware
* Software environment
* Runtime
* Relevant parameters
* Baseline results
* Limitations
* Conclusions

Reproducibility is particularly important when making claims about efficiency or performance.

---

# Failed Experiments

Failed experiments are valuable.

We should document important failures rather than hiding them simply because the result was disappointing.

A useful record should explain:

* What we expected
* What we tested
* What happened
* Possible reasons
* What we learned
* What should be investigated next

Research is a process, not a collection of screenshots of successful demos.

---

# Development Standards

Code should be:

* Understandable
* Tested
* Documented where necessary
* Deliberate
* Maintainable
* Appropriate for its purpose

Numerical code should receive particular attention to correctness and edge cases.

Changes should be tested before being considered complete.

---

# Version Control

Internal projects use Git for version control.

General expectations are:

* Keep commits meaningful
* Use descriptive branch names
* Test changes before committing
* Keep unrelated changes separate
* Review important changes
* Avoid committing generated files
* Never commit credentials or secrets

The stable branch of a project should represent a reasonably reliable version of that project.

Individual repositories may define more specific workflows.

---

# Code Review

Code review exists to improve the project.

Reviewers should examine:

* Correctness
* Design
* Maintainability
* Testing
* Performance where relevant
* Security where relevant
* Research implications

Technical disagreement is normal.

A reviewer identifying a problem is not a criticism of the person who wrote the code.

The goal is to make the resulting system better.

---

# AI-Assisted Development

AI tools may be used for:

* Learning
* Research assistance
* Debugging
* Code generation
* Code translation
* Documentation
* Brainstorming
* Code review
* Exploring implementation approaches

However:

> **Anyone contributing code is responsible for understanding that code.**

AI-generated code should not be treated as automatically correct.

Contributors should be able to explain, test and debug code they commit.

AI should accelerate learning and development rather than replace understanding.

---

# Research Integrity

We should be precise about what has actually been demonstrated.

Avoid turning:

> "This might work."

into:

> "This works."

or:

> "This is more efficient."

without evidence supporting the stronger claim.

When discussing results, clearly distinguish:

* Measured results
* Interpretation
* Hypotheses
* Existing research
* Personal opinions

If new evidence contradicts an earlier assumption, the evidence takes priority.

---

# Intellectual Property and Confidentiality

Unfloat's internal implementation and research are currently private.

Contributors should not publicly disclose:

* Private source code
* Internal repositories
* Unreleased implementations
* Private experiment results
* Internal architecture
* Credentials or secrets
* Confidential research material
* Unreleased product or business plans

Do not upload private project material to public repositories or services without permission.

When in doubt about whether something is intended to be public, treat it as private until the team has agreed otherwise.

Public descriptions should communicate the general research direction without revealing confidential implementation details.

---

# Repository Boundaries

Internal repositories may have different purposes.

For example, a repository may contain:

* Core infrastructure
* Research experiments
* A specific model or architecture
* Benchmarking systems
* Applications
* Supporting tools

Each repository should have a clearly defined purpose.

Experimental projects should not unnecessarily destabilize foundational infrastructure.

The exact repository structure is intentionally kept internal.

---

# Collaboration

We are a small team.

The goal is to avoid unnecessary bureaucracy while maintaining enough structure to prevent confusion.

Contributors should:

* Communicate major technical changes
* Avoid silently overwriting another person's work
* Share useful research
* Ask questions when something is unclear
* Challenge assumptions constructively
* Document important decisions
* Help other contributors understand the systems they work on

Everyone should understand the broad direction of the project even when individual contributors specialize in different areas.

---

# Security

Security-sensitive information must remain private.

Never commit:

* Passwords
* API keys
* Access tokens
* Private credentials
* Personal authentication information
* Other secrets

If a secret is accidentally committed, deleting it from the latest version is not necessarily enough because Git history may retain it.

Report accidental exposure immediately so the appropriate credentials can be revoked or replaced.

---

# Scope

Not every interesting technical idea belongs in Unfloat.

Research should have a meaningful relationship to the organization's research direction or to technology developed from that research.

Unrelated projects should remain separate rather than being forced into the organization.

---

# The Standard

Our standard is simple:

**Build things. Measure them. Understand them. Document them.**

We should be ambitious about the problems we investigate while remaining honest about what we have actually demonstrated.

The goal is not to convince people that Unfloat works.

The goal is to determine what works, understand why it works, understand where it fails, and build useful technology from what we learn.
