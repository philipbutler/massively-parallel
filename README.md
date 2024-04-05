# massively-parallel
A growing list of resources, exercises, and experimentation related to starting parallel processing, ultimately to write fast implementations of large ML/AI models.
These are also my notes for where I'm at on them, and my public journal for my learning process. <br><br>

PMPP:
- [Buy the Programming Massively Parallel Processors book](https://www.amazon.com/Programming-Massively-Parallel-Processors-Hands/dp/0323912311) if you have money to spend, or just [download the pdf](https://dokumen.pub/programming-massively-parallel-processors-a-hands-on-approach-4nbsped-9780323912310.html) if you don't.

GPU Puzzles:
- [The original GPU-Puzzles (Numba - Python syntax for CUDA)](https://github.com/philipbutler/GPU-Puzzles/tree/new_tests): My fork of [srush/GPU-Puzzles](https://github.com/srush/GPU-Puzzles): 14 GPU puzzles in a Colab notebook. I altered the first couple tests because a beginner can easily pass several on accident before realizing they're wrong (like myself). When I revisit this I'll continue those tests for more. As of writing, I've worked up to and still am working on Puzzle 13, because I'm too stuborn and only want to use the [walkthrough](https://www.youtube.com/watch?v=K4T-YwsOxrM) to check my answers.
- [CUDA C++ GPU Puzzles](https://github.com/dshah3/GPU-Puzzles): I haven't taken a look at this yet. Maybe as I work through PMPP.
- [Triton Puzzles (another by Sasha Rush, who made the original puzzles)](https://github.com/srush/Triton-Puzzles/): Srush worked with some interpreter folks on a visualizer for Triton debugging. Specifically it tries to make it easier to view the spatial structure of load/stores when implementing complex functions. As if there weren't enough options to learn, here's one if you want to feel like you work at OpenAI.

Selected [CUDA MODE](https://github.com/cuda-mode/lectures) Lectures:
- [Getting Started With CUDA for Python Programmers](https://www.youtube.com/watch?v=4sgKnKbR-WE): Jeremy Howard teaching an introductory lesson as a part of the [CUDA MODE](https://github.com/cuda-mode) lecture series. This lecuture aims to set you up well to work thorough the PMPP book, and explains an awesome hack to write CUDA code to run on Colab GPUs. No longer do we need our own NVIDA GPU! One can learn on a chromebook, or what I plan on doing, is learning CUDA & also to help learn PP concepts in general, to then apply to Metal, Triton, & Mojo.
- [Starter code only](https://colab.research.google.com/drive/15mWl0pvuyrriqFEnf1py7TlI9suRsesS?usp=sharing): I stripped down the notebook from Lecture 3 to be the barebones of what one needs to write a kernel on Colab. The compile time is rough, so I attempted and still would like to add the optimizations discussed [here](https://discord.com/channels/1189498204333543425/1189607750876008468/1211605910464495627) and put into a minimal repo [here](https://github.com/pbridger/cuda-experiments/blob/main/main.py).

Selected Resources:
- [Parallelizing Matrix multiplication (Mojo)](https://github.com/modularml/mojo/blob/main/examples/notebooks/Matmul.ipynb):  [From the Mojo site](https://docs.modular.com/mojo/notebooks/Matmul.html). A notebook starting from a sequential matmal I don't think you can currently use Colab (I tried to connect to a local runtime with mojo installed, it didn't work), but you can either [install mojo](https://docs.modular.com/mojo/manual/get-started/#develop-in-the-mojo-playground) and open a jupyter notebook, or even more simply use Modular's hosted Jupyter notebook environment called [Mojo Playground](https://docs.modular.com/mojo/manual/get-started/#develop-in-the-mojo-playground).

More:
- [Awesome GPU Resources](https://github.com/Jokeren/Awesome-GPU): Resources, mostly papers, on [GPU] architecture, algorithms, applications, tools, runtime, & code generation.

## Journal:
- 4/5/24: Finally finished Ch3 exercise 1. a & b 🥳. I was hesitant to draw a picture, thinking I shouldn't need to, but honestly not only did it make it so much easier, but I think my understanding is better after having drawn it. I have a 12" iPad Pro, but straight up nothing beats a pencil and sketch notebook. I truly wonder if I'll ever get as comfortable on a tablet. It's noon now, going on a last training run with my brother (we're running in a 10K in 2 days), and going go-karting with the homies around 6:30pm. That gives me between maybe 1:30pm-6pm to finish 2 & 5, no problem😼
- 4/4/24: I stripped down Lecture 3 starter code [(here)](https://colab.research.google.com/drive/15mWl0pvuyrriqFEnf1py7TlI9suRsesS?usp=sharing), going to now use this as a starting point for all the PMPP exercises
- 3/27 - 4/2: BS interview, recovered from cold & frustration, continued training for 10k, bowled with the homies, funeral & lecture 12 on flash attention, work all day Sunday-Tuesday.
- 3/26/24: Wife and I were sick, she went to work, I slept through my alarm which I never do, and my supervisior suggested I take the day off, which I gladly took, but my wife was not glad. Anyways I finished reading Chapter 3, and did problems 3 & 4, but my sick-ass brain was not working, and I had an interview the next morning, so I decided to rest with my wife the rest of the day.
- 3/23/24: Out of frustruation I [brazenly set a goal](https://discord.com/channels/1189498204333543425/1194427148656721970/1221116804030795896) that I wasn't able to reach, basically that I was going to study/practice every night after a 10 hour shift. I had a good session the first night at the cost of my wife being pissed at me. So this struggle between finding the balance between life and the grind is still really difficult for me to find, I feel like I lose either way. However, I think it's a good signal that throughout my delivery shifts, I have this deep yearning, wishing I was instead spending my time progressing my engineering skills - it reminds me of how I used to feel when I would be in school and couldn't wait to get out to go skateboard, being in love with the feeling of progressing.
- 3/22/24: In the morning finished chapter 2 and working on the exercises now. Will finish chapter 3 and probably skim/skip Lecture 2, and today I at least want to upload a CUDA C++ vector addition program whether in the Colab notebook format like in JH's lecture, or if I'm really ambitious, get CUDA set up on my PC and run it locally. I think I set it up but never actually wrote/ran anything so idk. Update: I did neither that day.
- 3/21/24: Started Lecture 2 then realized it's a recap of chapters 1-3. Read most of chapter 2 before bed.
- 3/20/24: Hoping to watch [Lecture 2](https://www.youtube.com/watch?v=NQ-0D5Ti2dc), and see how far along I can Read & do the exercises of chapter 2.
- 3/19/24: Read parts of the preface and through most of Chapter 1 of PMPP. Thanks to my annotation system I got going on, I see I read 1.1, and skimmed the rest. I'm eager to get to more of the meat, and have indicated where I could go back to read more thoroughly.
Pointing out from "Preface/A two-phased approach":
  - Most chapters designed to be covered in 1 75-min lecture, with 11 14 & 15 might needing 2.
  - (7 weeks) Phase 1: Parts I & II, 12 chapters - fundamentals, basic patterns, guided programming assignments
  - ...
The reason I'm pointing this out is because it looks to me like learning PP is going to be a marathon rather than a sprint, so I'm going to remind myself to stay patient, consistent, & to try and keep a good pace throughout my practice.
- 3/1/24: Watched CUDA MODE [Lecture 1](https://www.youtube.com/watch?v=LuhJEEJQgUM)
