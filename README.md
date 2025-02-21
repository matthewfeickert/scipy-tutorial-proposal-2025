# [SciPy 2025](https://www.scipy2025.scipy.org/) Submission Instructions

## Information

## Topics

Tutorials should be focused on covering a well-defined topic in a hands-on manner. We want to see attendees coding! We encourage submissions to be designed to allow at least 50% of the time for hands-on exercises even if this means the subject matter needs to be limited. Tutorials will be 4 hours in duration. In your tutorial application, you can indicate what prerequisite skills and knowledge will be needed for your tutorial, and the approximate expected level of knowledge of your students (i.e., beginner, intermediate, advanced).

We are looking for interesting techniques or packages, helping new or advanced Python programmers develop better or faster scientific applications.

## Information for tutorial presenters

### Selection

Accepted tutorials will be announced late March. Final tutorial materials and instructions for attendees will be due on June 11th. This will include final version numbers of required software, detailed and tested installation instructions, and a test script that can be run by attendees to ensure that they have sufficient time to prepare their laptops before the conference. In addition, there will be a pre-tutorial slack channel created before the conference, and tutorial presenters are expected to make themselves available to help with setup instructions.

### Stipend

In recognition of the effort required to plan and prepare a high quality tutorial, we pay a stipend of $1,000 to each instructor (or team of instructors) for each half-day session they lead.

For the submission you will need the following information:
* A short bio of the presenter or team members, containing a description of past experiences as a trainer/teacher/speaker, and (ideally) links to videos of these experiences if available.
* A list of prerequisite skills expected of attendees, so that participants can choose level appropriate tutorials.
* A description of the tutorial, suitable for posting on the SciPy website for attendees to view. It should include the target audience, the expected level of knowledge prior to the class, and the goals of the class.
* A more detailed outline of the tutorial content, including the duration of each part and exercise sessions. Please include a description of how you plan to make the tutorial hands-on.
* Detailed installation instructions for various common Python environments so that attendees can have everything ready for participating before heading to SciPy.
* If available, the tutorial notes, slides, exercise files, and IPython notebooks, even if they are preliminary.

Authors of exemplary submissions from previous years have generously agreed to share their proposals to help new instructors: https://github.com/scipy-conference/scipy-conference/tree/master/data/tutorial_submissions

## Submission

* [Public review preview](https://cfp.scipy.org/scipy2025/talk/review/K9KPCJZNPWMRGDN7RMQLCQGMK37HRY3U)

### Title

Reproducible Machine Learning Workflows for Scientists with pixi

### Session type

Tutorial (4 hours)

### Track

Tutorials

### Abstract

> Your Abstract will appear in the online schedule and give attendees a sense of your talk. This should be around 100 words or less.

Scientific researchers need reproducible software environments for complex applications that can run across heterogeneous computing platforms.
Modern open source tools, like `pixi`, provide automatic reproducibility solutions for all dependencies while providing a high level interface well suited for researchers.

This tutorial will provide a practical introduction to using `pixi` to easily create scientific and AI/ML environments that benefit from hardware acceleration, across multiple machines and platforms.
The focus will be on applications using the PyTorch and JAX Python machine learning libraries with CUDA enabled, as well as deploying these environments to production settings in Linux container images.

### Description

> Your placement in the program will be based on reviews of your description. This should be a roughly 500-word outline of your presentation. This outline should concisely describe software of interest to the SciPy community, tools or techniques for more effective computing, or how scientific Python was applied to solve a research problem. A traditional background/motivation, methods, results, and conclusion structure is encouraged but not required. Links to project websites, source code repositories, figures, full papers, and evidence of public speaking ability are encouraged.

As artificial intelligence (AI) and machine learning (ML) becomes a modern part of the scientific toolkit, the need to have robustly reproducible scientific computing environments that support hardware acceleration, e.g. with CUDA, becomes more important.
However, historically just installing a working CUDA environment on a single machine, let alone on multiple platforms with different requirements, was considered a particularly difficult and painful task.
This lead to many scientific machine learning workflows being reliably runnable on only particular machines, and, even worse, with environments that were not reproducible across time.

With significant recent advancements by the NVIDIA open source team and the conda-forge open source community, the entire CUDA stack &mdash; from compilers to runtime libraries &mdash; is now distributed on conda-forge.
This significantly reduces the overhead to _install_ CUDA dependencies, but packaging and distribution of binaries alone does not solve the problem of reproducibility.
With automatic multi-platform hash-level lock file support for all dependencies that are available on package indexes (like PyPI and conda-forge), highly efficient solving strategies, and high level user interfaces, `pixi` provides a missing piece to the scientific researcher toolkit.
With `pixi`, researchers are able to easily specify the hardware acceleration requirements they have, multiple different computational environments needed for their experiments, and the required software dependencies, and then quickly solve for a multi-platform lock file of all the dependencies required, down to the compiler level.
This makes it possible to have multiple hardware accelerated environments defined that are able to run AI/ML workflows across heterogeneous machines with different GPU types and CUDA compatibility.

This tutorial will be targeted on scientific researchers who use Python for scientific computing and use hardware accelerated workflows in their research, with a particular focus on AI/ML.
No prior expertise with hardware accelerator systems is assumed.
The tutorial structure will begin with an introduction to `pixi` as a computational environment manager, and exploring how it provides features beyond other more common package managers that might be used for Python dependencies.
It will then extend to adding CUDA requirements to `pixi` environments, and provide participants with exercises for solving environments and running simple AI/ML workflows using the PyTorch and JAX machine learning libraries.
The tutorial will then move towards more complex environment requirements in later exercises.
The tutorial will conclude with examples and exercises focusing on deploying `pixi` workflows to production environments by distributing `pixi` environments in Linux container images.

Tutorial participants will code all examples themselves.
Participants will also be given time to explore solutions to their own hardware accelerated Python workflows.
To make the tutorial more practical and interactive, cloud GPU resources will be requested from industry partners, that will allow for participants to have hardware accelerated resources to run their own examples on.

### Notes

* [Matthew Feickert](https://github.com/matthewfeickert) (speaker / instruction team member) has been awarded a [US Research Software Sustainability Institute Early-Career Fellowship](https://urssi.us/blog/2024/11/22/call-for-proposals-for-the-urssi-early-career-fellowship-program/) to research reproducible machine learning workflow standards for scientists.
Part of his work will involve running a workshop in the United States that would cover these topics and more academic research focused problems across multiple days.
If accepted, this tutorial would be a distilled version of the open source workshop resources he will create.

* [Ruben Arts](https://github.com/ruben-arts/)  (speaker / instruction team member) is a core maintainer of `pixi` at [Prefix.dev](https://prefix.dev/).
He regularly speaks and teaches at events like [PyData Eindhoven](https://www.youtube.com/watch?v=P7CO25cx4CI), [PyCon DE](https://youtu.be/sVc0PmeSUNk?si=CmQI34s2rCInerC7&t=444), and various podcasts. More content can be found on the [Prefix.dev YouTube Channel](https://www.youtube.com/@prefix_dev).

### Additional Speaker

* Ruben Arts, ruben.arts[no-spam-please]hotmail.com

#### Bio

[Ruben Arts](https://github.com/ruben-arts/) is a core maintainer of `pixi` at [Prefix.dev](https://prefix.dev/).
Originally a Robotics Engineer, he experienced firsthand the challenges of package management in research and industry.
This led him to join Prefix.dev, where he focuses on building better tools for reproducibility and ease of onboarding, especially in education and research.
He regularly speaks and teaches at events like [PyData Eindhoven](https://www.youtube.com/watch?v=P7CO25cx4CI), [PyCon DE](https://youtu.be/sVc0PmeSUNk?si=CmQI34s2rCInerC7&t=444), and various podcasts. More content can be found on the [Prefix.dev YouTube Channel](https://www.youtube.com/@prefix_dev).

### Session image

> Use this if you want an illustration to go with your proposal.
Please do not upload files larger than 10.0MB!
This content will be shown publicly.

TODO

### Prerequisites

> A list of prerequisite skills expected of attendees, so that participants can chose level appropriate tutorials.
This content will be shown publicly.

Participants should be familiar with Python programming for science, and using external dependencies in their work.
The tutorial will use machine learning workflows as examples, but while familiarly with machine learning may be useful for conceptual understanding of the tasks, no prior machine learning knowledge is required to complete the tutorial.
No prior expertise with CUDA is assumed.

### Confirm

* [x] The author(s) agree(s) to take responsibility and be accountable for the contents of the submission and is/are authorized to present it.

### If you used AI tools and or services to support the preparation of your submission, please state the name and reason for using each of them. If you haven't used any, please enter "No AI."

No AI.

### Installation Instructions

`pixi` is the only tool that needs to be installed prior to the start of the tutorial.
Install instructions for `pixi` are [provided on the `pixi` documentation website](https://pixi.sh/latest/#installation), but can be summarized as

* Linux, macOS:

```
curl -fsSL https://pixi.sh/install.sh | bash
```

* Windows

```
powershell -ExecutionPolicy ByPass -c "irm -useb https://pixi.sh/install.ps1 | iex"
```

### Outline

> A more detailed outline of the tutorial content, including the duration of each part and exercise sessions. Please include a description of how you plan to make the tutorial hands-on.

A general time outline of the tutorial follows:

**0:00 &ndash; 0:20 (20 min):**

* Overview of importance of, and challenges to, reproducible scientific workflows.
* Introduction of `pixi` and `pixi` environment management philosophy.

**0:20 &ndash; 0:40 (20 min):**

* Work through the [`pixi` Python tutorial](https://pixi.sh/latest/tutorials/python/).

**0:40 &ndash; 1:00 (20 min):**

* Exercise 1: Create a multi-platform multi-environment `pixi` project to run a provided "Scientific Python" (e.g., SciPy, NumPy, Matplotlib) example workflow that does not use machine learning.

**1:00 &ndash; 1:15 (15 min):**

* Break

**1:15 &ndash; 1:30 (15 min):**

* Discussion over solutions to Exercise 1.
* Discuss and answer questions participants have.

**1:30 &ndash; 2:50 (20 min):**

* Introduction to the concepts of [conda-forge](https://github.com/conda-forge), the CUDA software stack on conda-forge, and [CUDA `system-requirements` in `pixi`](https://pixi.sh/latest/features/system_requirements/#using-cuda-in-pixi).

**1:50 &ndash; 2:20 (30 min):**

* Exercise 2: Create a `pixi` project to run an example PyTorch machine learning workflow on GPUs with CUDA `v12`.
* Exercise 3: Extend the `pixi` project from Exercise 2 to provide a new environment to run an example JAX machine learning workflow on GPUs with CUDA v11.8.

**2:20 &ndash; 2:35 (15 min):**

* Break

**2:35 &ndash; 2:55 (20 min):**

* Discussion over solutions to Exercises 2 and 3.
* Introduction to environments that install from multiple package indexes (e.g. conda-forge and PyPI).

**2:55 &ndash; 3:15 (20 min):**

* Exercise 4: Create a `pixi` project to run an example machine learning workflow on GPUs with CUDA that installs dependencies from both conda-forge and PyPI.
* Discussion over solutions to Exercise 4.

**3:15 &ndash; 3:25 (10 min):**

* Very brief introduction the concepts of "production environments" and Linux containers.
As Linux containers are their own technology that can be quite complex, all Linux container components of the tutorial will be pre-prepared for participants.

**3:25 &ndash; 3:45 (20 min):**

* Exercise 5: Containerize the `pixi` project environment from Exercise 2 in a Linux container image and run a Pytorch machine learning workflow on GPUs with the deployed container.

**3:45 &ndash; 4:00 (15 min):**

* Discussion over solutions to Exercise 5.
* Time for participants to start exploring their own projects with `pixi`.
* General question and answer time with instructor team.

### Additional Information

> If available, the tutorial notes, slides, exercise files, and IPython notebooks, even if they are preliminary.

The tutorial has not been written yet but will be developed at https://github.com/matthewfeickert-talks/reproducible-ml-for-scientists-with-pixi-scipy-2025.
Example components of what will go into the tutorial exist in the `pixi` documentation:

* [Tutorial: Doing Python development with Pixi](https://pixi.sh/latest/tutorials/python/)
* [Tutorial: How to use Pytorch with Pixi](https://pixi.sh/latest/features/pytorch/)
* [Examples: Directory full of example `pixi` use cases](https://github.com/prefix-dev/pixi/examples/)

and various GitHub repositories:

* https://github.com/matthewfeickert/pytorch-gpu-pixi-example
* https://github.com/UW-Madison-DSI/pixi-docker-chtc

### Prior Python Programming Level of Knowledge Expected

> Please note this reflects the attendees' Python programming level only, not the attendees' level of understanding of the topic.

Basic.
The participants are assumed to have written scientific scripts with Python and installed dependencies for their software from PyPI and/or conda-forge before.

### Paper or Additional Materials

> Upload your paper or additional materials. Please do not upload files larger than 10.0MB!

None.

### Resources

> Resources will be publicly visible. Please try to keep your uploads below 16MB.

TODO
