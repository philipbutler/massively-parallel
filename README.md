# massively-parallel
A growing list of resources, exercises, and experimentation related to starting parallel processing, ultimately to write fast implementations of large ML/AI models.
These are also my notes for where I'm at on them, and my public journal for my learning process. <br><br>
You *probably* only need a basic understanding of python to start with any of these.

PMPP:
- [Buy the Programming Massively Parallel Processors book](https://www.amazon.com/Programming-Massively-Parallel-Processors-Hands/dp/0323912311) if you have money to spend, or just [download the pdf](https://dokumen.pub/programming-massively-parallel-processors-a-hands-on-approach-4nbsped-9780323912310.html) if you don't.

GPU Puzzles:
- [The original GPU-Puzzles (Numba - Python syntax for CUDA)](https://github.com/philipbutler/GPU-Puzzles/tree/new_tests): My fork of [srush/GPU-Puzzles](https://github.com/srush/GPU-Puzzles): 14 GPU puzzles in a Colab notebook. I altered the first couple tests because a beginner can easily pass several on accident before realizing they're wrong (like myself). When I revisit this I'll continue those tests for more. As of writing, I've worked up to and still am working on Puzzle 13, because I'm too stuborn and only want to use the [walkthrough](https://www.youtube.com/watch?v=K4T-YwsOxrM) to check my answers.
- [CUDA C++ GPU Puzzles](https://github.com/dshah3/GPU-Puzzles): I haven't taken a look at this yet. Maybe as I work through PMPP.
- [Triton Puzzles (another by Sasha Rush, who made the original puzzles)](https://github.com/srush/Triton-Puzzles/): Srush worked with some interpreter folks on a visualizer for Triton debugging. Specifically it tries to make it easier to view the spatial structure of load/stores when implementing complex functions. As if there weren't enough options to learn, here's one if you want to feel like you work at OpenAI.

Selected Resources:
- [Parallelizing Matrix multiplication (Mojo)](https://github.com/modularml/mojo/blob/main/examples/notebooks/Matmul.ipynb):  [From the Mojo site](https://docs.modular.com/mojo/notebooks/Matmul.html). A notebook starting from a sequential matmal I don't think you can currently use Colab (I tried to connect to a local runtime with mojo installed, it didn't work), but you can either [install mojo](https://docs.modular.com/mojo/manual/get-started/#develop-in-the-mojo-playground) and open a jupyter notebook, or even more simply use Modular's hosted Jupyter notebook environment called [Mojo Playground](https://docs.modular.com/mojo/manual/get-started/#develop-in-the-mojo-playground). When I had a session with this, I first read through the document, then I ran the code in it, then started [rewriting it](https://github.com/philipbutler/hello-mojo/blob/main/MojoMatMulRewrite.ipynb) as an exercise. I was trying to keep a daily streak going learning Mojo, so I streamed it [here](https://www.youtube.com/live/raKBN8k80W4?si=K7zs4NL4CR4vmFVo), and left off where I wrote #left off.

- [Getting Started With CUDA for Python Programmers](https://www.youtube.com/watch?v=4sgKnKbR-WE): Jeremy Howard teaching an introductory lesson as a part of the [CUDA MODE](https://github.com/cuda-mode) lecture series. I'm only about 10 minutes in, but I realized that I wanted a better way of keeping track of where I'm at in this parallel processing [eventually large ML models] journey, and paused to make this repo. This lecuture aims to set you up well to work thorough the PMPP book (next).

## Journal:

- 3/20/24: Hoping to watch [Lecture 2](https://www.youtube.com/watch?v=NQ-0D5Ti2dc), and see how far along I can Read & do the exercises of chapter 2. I plan to update this bullet tonight
- 3/19/24: Read parts of the preface and through most of Chapter 1 of PMPP. Thanks to my annotation system I got going on, I see I read 1.1, and skimmed the rest. I'm eager to get to more of the meat, and have indicated where I could go back to read more thoroughly.
Pointing out from "Preface/A two-phased approach":
  - Most chapters designed to be covered in 1 75-min lecture, with 11 14 & 15 might needing 2.
  - (7 weeks) Phase 1: Parts I & II, 12 chapters - fundamentals, basic patterns, guided programming assignments
  - ...
The reason I'm pointing this out is because it looks to me like learning PP is going to be a marathon rather than a sprint, so I'm going to remind myself to stay patient, consistent, & to try and keep a good pace throughout my practice.
- 3/1/24: Watched CUDA MODE [Lecture 1](https://www.youtube.com/watch?v=LuhJEEJQgUM)
