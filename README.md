<!--
# pmph-e2023-pub
--PMPH course 2023-24 public repo
--> 

# Programming Massively Parallel Hardware (PMPH), Block 1 2023

### We are grateful to Nvidia for awarding us a teaching grant (for the PMPH and DPP courses) that consists of two A100 GPUs. These are now accessible on the server futharkhpa03fl.unicph.domain

## Course Structure

PMPH is structured to have four hours of (physical) lectures
and four hours of (physical) labs per week; potentially we
will have no lectures in the last few weeks of the course, so you
can concentrate on project work (to be announced).

[Course Catalog Web Page](https://kurser.ku.dk/course/ndak14008u/2023-2024)

### Lectures (zoom links will be posted on Absalon):

* Monday    13:00 - 15:00 (øv - 4-0-02, Ole Maaløes Vej 5, Biocenter)
* Wednesday 13:00 - 15:00 (øv - 4-0-02, Ole Maaløes Vej 5, Biocenter)

### Labs: 

* Monday    15:00 - 17:00 (øv - 4-0-32, Ole Maaløes Vej 5, Biocenter)
* Wednesday 15:00 - 17:00 (aud - NBB 2.0.G.064/070, Jagtvej 155)

### Flexible Schedule on Wednesday

We have also reserved room "aud - NBB 2.0.G.064/070, Jagtvej 155" 
for Wednesday 10:00 -- 12:00. In case there is a vast majority of
you who prefer starting in the morning, we can re-schedule the
lecture and lab on Wednesday.


### Physical Attendence to Lectures and Labs

The current plan is that everybody will have a physical place
at the lecture and lab. Unless we are forced to move to virtual
teaching, the lectures and labs will not be recorded, so please
plan to attend. If there is strong request, we may stream the
lectures, but without providing any guarantees as to the quality
of streaming.

### Evaluation

Throughout the course, you will hand in four weekly assignments,
which will count for 40\% of the final grade. In the last month
of the course, you will work on a group project (up to three
students per group), and will submit the report and accompanying
code. The group project will be presented orally at the exam together
with the answers to some individual questions, and this will count
for 60\% of your final grade.

The "weekly-assignments" (W-assignments) are tentatively planned to be
published each Wednesday of the first four weeks. They have one week
editing time. If a serious attempt was made but the solution is not
satisfactory (or simply if you want to improve your assignment, hence grade),
an updated solution should be resubmitted one week after the date when
the assignment was graded, i.e., returned to you.  Extensions may be
possible, but your TA will need to agree with it TA.

For the group project no re-submission is possible; the deadline is the
Friday just before the exam week.

The oral examination will be hold in the exam week (Wednesday, Thursday and Friday if necessary). The final evaluation will take up to 20 minutes per student, but probably the whole group will be examined at a time (unless you wish otherwise).

**Weekly and group assignment handin is still on Absalon.**

### Teacher and Teaching Assistants (TAs)

Teacher: **[Cosmin Oancea](mailto:cosmin.oancea@diku.dk)**.

Teaching assistants (TA): 

**[Anders Holst](mailto:anersholst@gmail.com)**

**[Nikolaj Hey Hinnerskov](mailto:nihi@di.ku.dk)**. 

The plan is that the teacher will conduct the lectures and the lab.
The TAs will be mainly in charge of grading and providing good feedback
to the weekly assignments and patrolling the Absalon/Discord discussion
forums.

### Course Tracks and Resources

All lectures and lab sessions will be delivered in English.  The
assignments and projects will be posted in English, and while you can
chose to hand in solutions in either English or Danish, English is
preferred. All course material except for the hardware book is distributed 
via this GitHub page. (Assignment handin is still on Absalon.)

* **The hardware track** of the course covers (lecture) topics related to processor, memory and interconnect design, including cache coherency, which are selected from the book [Parallel Computer Organization and Design, by Michel Dubois, Murali Annavaram and Per Stenstrom,  ISBN 978-521-88675-8. Cambridge University Press, 2012](https://www.cambridge.org/dk/academic/subjects/engineering/computer-engineering/parallel-computer-organization-and-design?format=HB&isbn=9780521886758). The book is available at the local bookstore (biocenter). It is not mandatory to buy it---Cosmin thinks that it is possible to understand the material from the lecture slides, which are detailed enough---but also note that lecture notes are not provided for the hardware track, because of copyright issues.

* **The software track** covers (lecture) topics related to parallel-programming models and recipes to recognize and optimize parallelism and locality of reference.  It demonstrates that compiler optimizations are essential to fully utilizing hardware, and that some optimizations can be implemented both in hardware and software, but with different pro and cons.   [The lecture notes are available here](material/lecture-notes-pmph.pdf), and additional (facultative) reading material (papers) will be linked with individual lectures; see Course Schedule Section below.

* **The lab track** teaches GPGPU hardware specifics and programming in Futhark, CUDA, and OpenMP. The intent is that the lab track applies in practice some of the parallel programming principles and optimizations techniques discussed in the software tracks. It is also intended to provide help for the weekly assignment, project, etc.

## Course Schedule

This course schedule is tentative and will be updated as we go along.

The lab sessions are aimed at providing help for the weeklies and
group project.  Do not assume you can solve them without attending
the lab sessions.

| Date | Time | Topic | Material |
| --- | --- | --- | --- |
| 05/09 | 13:00-15:00 | [Intro, Hardware Trends and List Homomorphisms (SFT)](slides/L1-Intro-Org-LH.pdf), Chapters 1 and 2 in Lecture Notes | [Sergei Gorlatch, "Systematic Extraction and Implementation of Divide-and-Conquer Parallelism"](material/List-Hom/GorlatchDivAndConq.pdf);  [Richard S. Bird, "An Introduction to the Theory of Lists"](material/List-Hom/BirdThofLists.pdf); [Jeremy Gibons, "The third homomorphism theorem"](material/List-Hom/GibonsThirdTheorem.pdf) |
| 05/09 | 13:00-15:00 | [Gentle Intro to CUDA](slides/Lab1-CudaIntro.pdf)](slides/L1-Intro-Org-LH.pdf) |
| 07/09 | 13:00-15:00 | [List Homomorphism & Parallel Basic Blocks (SFT)](slides/L2-Flatenning.pdf), Chapters 2 and 3 in Lecture Notes | [Various papers related to flattening, but which are not very accessible to students](material/Flattening) |
| 07/09 | 15:00-17:00 | Lab: Futhark programming, First Weekly | [Parallel Programming in Futhark](https://futhark-book.readthedocs.io/en/latest/), sections 1-4, [futhark code for the first week (list homs)](futhark-code/L1) |
| 07/09 | some time   | [**Assignment 1 handout**](weeklies/weekly-1/) | |
| 12/09 | 13:00-15:00 | [Parallel Basic Block & Flattening Nested Parallelism (SFT)](slides/L2-Flatenning.pdf) | chapters 3 and 4 in Lecture Notes |
| 12/09 | 15:00-17:00 | Lab: [Fun Quiz](slides/Lab2_presentation.pdf); | help with weekly |
| 14/09 | 13:00-15:00 | [Flattening Nested Parallelism (SFT)](slides/L2-Flatenning.pdf) | , chapter 4 in Lecture Notes |
| 14/09 | 15:00-17:00 | Lab: [Reduce and Scan in Cuda](slides/Lab2-RedScan.pdf) | discussing second weekly, helping with the first |
| 14/09 | some time   | [**Assignment 2 handout**](weeklies/weekly-2/) | |
| 19/09 | 13:00-15:00 | [In-Order Pipelines (HWD)](slides/L3-InOrderPipe.pdf) | Chapter 3 of "Parallel Computer Organization and Design" Book |
| 19/09 | 15:00-17:00 | Lab: helping with weeklies |  |
| 21/09 | 13:00-15:00 | [Optimizing ILP, VLIW Architectures (SFT-HWD)](slides/L4-VLIW.pdf) | Chapter 3 of "Parallel Computer Organization and Design" Book |
| 21/09 | 15:00-17:00 | Lab: [GPU hardware: three important design choices.](slides/Lab2-GPU-HWD.pdf) | helping with the first two weekly assignments.
| 21/09 |  | No new weekly assignment this week; the third will be published next week | |
| 26/09 | 13:00-15:00 | [Dependency Analysis of Imperative Loops](slides/L5-LoopParI.pdf) | Chapter 5 of lecture Notes |
| 26/09 | 15:00-17:00 | Lab: Recognizing Scan and Reduce Patterns in Imperative Code | helping with the weekly assignments. |
| 28/09 | 13:00-15:00 | [Optimizing Locality, Case Study: Nearest Neighbor, Matrix Multiplication and Transposition](slides/L5-LoopParI.pdf) | Chapters 5 and 6 of lecture Notes |
| 28/09 | 15:00-17:00 | Lab: discussing the third assignment | helping with the weekly assignments.
| 28/09 | some time   | [**Assignment 3 handout**](weeklies/weekly-3/) | |
| 03/10 | 13:00-15:00 | [Memory Hierarchy, Bus-Based Coherency Protocols (HWD)](slides/L6-MemIntro.pdf) | Chapter 4 and 5 of "Parallel Computer Organization and Design" Book |
| 03/10 | 15:00-17:00 | Lab: [**Presenting Possible Group Projects**](group-projects/) | discussing group projects, helping with weekly assignments |
| 05/10 | 13:00-15:00 | HWD: [Scalable Coherence Protocols](slides/L7-Interconnect.pdf) | Chapters 5 and 6 of "Parallel Computer Organization and Design" Book |
| 05/10 | 15:00-17:00 | Lab: [**Presenting Possible Group Projects**](group-projects/), [Assignment 4 handout](weeklies/weekly-4/) | helping with weekly assignments, discussing group projects.
| 05/10 | some time | [Assignment 4 handout](weeklies/weekly-4/) | |
| 10/10 | 13:00-15:00 | HWD: [Scalable Coherence Protocols, Scalable Interconect (HWD)](slides/L7-Interconnect.pdf) | Chapters 5 and 6 of "Parallel Computer Organization and Design" Book |
| 10/10 | 15:00-17:00 | Lab: helping with weekly assignments and project |  |
| 12/10 | 13:00-15:00 | [Inspector-Executor Techniques for Locality Optimizations (SFT)](slides/L8-LocOfRef.pdf) | [Various scientific papers](material/Opt-Loc-Ref) |
| 12/10 | 15:00-17:00 | Lab: Working on the 4th Weekly Assignment | helping with project and anything else.
| 17/10 | 13:00-15:00 | Autumn break (no lecture) | |
| 17/10 | 15:00-17:00 | Autumn break (no lab) | |
| 19/10 | 13:00-15:00 | Autumn break (no lecture) | |
| 19/10 | 15:00-17:00 | Autumn break (no lab) |
| 24/10 | 13:00-15:00 | No lecture |  |
| 24/10 | 15:00-17:00 | Lab: Helping with group-project, weekly assignments | |
| 26/10 | 13:00-15:00 | [Modern CPU Design: Tomasulo Algorithm (HWD)](slides/L9-OoOproc.pdf)| Chapter 3 of "Parallel Computer Organization and Design" Book |
| 26/10 | 15:00-17:00 | Lab: help with group project, weeklies |
| 31/10 | 13:00-15:00 | Invited Talk: Prof. Pedro Trancoso (Chalmers University) | either in this slot or we switch with the slot from 15:00-17:00; to be updated later |
| 31/10 | 15:00-17:00 | Lab: Helping with group project, weeklies | |
| 02/11 | 13:00-15:00 | No Lecture unless you ask for one | |
| 02/11 | 15:00-17:00 | Lab: help with group project |
| 09/11 | whole day | Oral exam | one three-person group will be examined in about 1 hour, but all of you will take two full days.|
| 10/11 | whole day | Oral exam | |
 



## Weekly assignments

The weekly assignments are **mandatory**, must be solved
**individually**, and make up 40% of your final grade.  Submission is
on Absalon.

Hopefully, you will receive feedback a week after the handin deadline
(at the latest).  You then have another week to prepare a re-submission.
That is, **the re-submission deadline is two weeks after the original
handin deadline, given that you receive the feedback in time**.

### Weekly 1 (due September 15th)

* [Assignment text](weeklies/weekly-1/assignment1.asciidoc)
* [Code handin](weeklies/weekly-1/w1-code-handin.tar.gz)

### Weekly 2 (due September 28th)

* [Assignment text](weeklies/weekly-2/assignment2.asciidoc)
* [Code handout](weeklies/weekly-2/w2-code-handin.tar.gz)

### Weekly 3 (due October 7th)

* [Assignment text](weeklies/weekly-3/assignment3.asciidoc)
* [Code handout](weeklies/weekly-3/w3-code-handin.tar.gz)

### Weekly 4 (due October 14th)

* [Assignment text](weeklies/weekly-4/Assignment4.pdf)

## Group projects (due Friday just before the exam week starts)

Several potential choices for group project may be found in folder `group-projects`, namely

* **You are free to propose your own project, for example from the machine learning field, but please discuss it first with Cosmin, to make sure it is a relevant project, i.e., on which you can apply some of the techniques/reasoning that we have studied in PMPH.**
* [Single Pass Scan in Cuda (basic block of parallel programming)](group-projects/single-pass-scan)
* [GPU Implementation of Linear Recurrences](group-projects/linear-rec)
* [Futhark or Cuda implementation for the Rank-K Search Problem](group-projects/rank-search-k)
* [Fast Sorting Algorithm(s) for GPUs](group-projects/sorting-on-gpu)
* [Bfast: a landscape change detection algorithm (Remote Sensing)](group-projects/bfast)
* [Local Volatility Calibration  (Finance)](group-projects/loc-vol-calib)
* [HP Implementation for Fusing Tensor Contractions (Deep Learning)](group-projects/tensor-contraction): read the paper, implement the technique (some initial code is provided), and try to replicate the results of the paper. Or you can also try to implement a matrix multiplication for 16-bit floats that uses the tensor-core support. 

[Here you can find the CUB library and a simple program that utilizes CUB to sort](group-projects/cub-code)

## GPU + MultiCore Machines

All students will be provided individual accounts on a multi-core and GPGPU machine that supports multi-core programming via C++/OpenMP and CUDA programming.

Login to GPU & 16 multicore machines will become operational after 6th of September:

You log in by first SSHing to the bastion server
`ssh-diku-apl.science.ku.dk` using your KU license plate (`abc123`) as
the user name, and then SSHing on to one of the GPU machines.

```bash
$ ssh -l <ku_id> ssh-diku-apl.science.ku.dk
$ ssh gpu04-diku-apl
````
(or gpu02-diku-apl or gpu03-diku-apl).
 
Despite their names, they each have 16 cores with 2-way hyperthreading CPUs and plenty of RAM as well. The GPUs are:
  * `gpu02-diku-apl`, `gpu03-diku-apl` have dual GTX780 Ti GPUs.

  * `gpu04-diku-apl` has a GTX 2080 Ti GPU (by far the fastest).

For CUDA to work, you may need to add the following to your `$HOME/.bash_profile` or `$HOME/.bashrc` file (on one of the gpu02..4-diku-apl machines):

```bash
CUDA_DIR=/usr/local/cuda
export PATH=$CUDA_DIR/bin:$PATH
export LD_LIBRARY_PATH=$CUDA_DIR/lib64:$LD_LIBRARY_PATH
export LIBRARY_PATH=$LD_LIBRARY_PATH:$LIBRARY_PATH
export CPLUS_INCLUDE_PATH=$CUDA_DIR/include:$CPLUS_INCLUDE_PATH
export C_INCLUDE_PATH=$CUDA_DIR/include:$C_INCLUDE_PATH
```

*New accounts have also been created on sever futharkhpa03fl.unicph.domain, which contains two top-of-the-line A100 Nvidia GPUs.* You may ssh directly to `futharkhpa03fl.unicph.domain` with your ku-id and corresponding password, and then similarly add the above to your `.bashrc` file. More hardware documentation is available [here](https://github.com/diku-dk/howto/blob/main/servers.md)

## Other resources

### Futhark and CUDA

* We will use a basic subset of Futhark during the course. Futhark related documentation can be found at [Futhark's webpage](https://futhark-lang.org), in particular a [tutorial](https://futhark-book.readthedocs.io/en/latest/) and [user guide](https://futhark.readthedocs.io/en/stable/)

* [CUDA C Best Practices Guide](https://docs.nvidia.com/cuda/cuda-c-best-practices-guide/index.html) you may want to browse through this guide to see what offers. No need to read all of it closely.


### Other Related Books

* Some of the compiler transformations taught in the software track can be found
in this book [Optimizing Compilers for Modern Architectures. Randy Allen and Ken Kennedy, Morgan Kaufmann, 2001](https://www.elsevier.com/books/optimizing-compilers-for-modern-architectures/allen/978-0-08-051324-9), but you are not expected to buy it or read for the purpose of PMPH.

* Similarly, some course topics are further developed in this book [High-Performance Computing Paradigm and Infrastructure](https://www.wiley.com/en-dk/High+Performance+Computing%3A+Paradigm+and+Infrastructure-p-9780471732709), e.g., Chapters 3, 8 and 11, but again, you are not expected to buy it or read for the purpose of PMPH.

