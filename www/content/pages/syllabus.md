Title: UC Berkeley's Statistics 159/259 (Fall 2015)
Slug: syllabus

## Reproducible and Collaborative Statistical Data Science

[TOC]

### Overview and Longer Course Description

This is a project-based course that introduces you to reproducible and
collaborative statistical research, applied to real scientific questions.  You
will gain experience acquiring, cleaning, and curating data; formulating
scientific questions statistically; developing appropriate statistical methods
to analyze the data to answer the scientific questions; implementing those
methods in robust, testable, reusable, extensible software; applying the
methods; visualizing the results; interpreting the results; and communicating
the results to others. And you will learn to do this in a way that is
computationally reproducible, which is increasingly recognized as key to
scientific progress.

As if you were working in a scientific research group or in industry, you will
be given a set of tools (a “software stack”) and practices you are required to
master and use. As if you were working in a scientific research group or in
industry, you will be pointed to resources to help you learn the tools, and it
is your responsibility to ensure that you have mastered them, which will
require a substantial amount of time outside class. And, as if you were working
in a scientific research group or in industry, you will be required to
collaborate and to take responsibility for your role in the collaboration. 

But the point is not merely to master the tools or to learn to collaborate
effectively.  Rather, the point is to do sound computational science, and to do
it in a way that others can verify the data and statistical techniques behind
your analysis, can verify that your code does what it’s supposed to do, can run
the code using the data and parameters you used, can verify that they get the
same results you do, and can build on what you have done. 

### Format

Three hours of class per week in two 90-minute sessions, plus two hours of labwork.
Class sessions are divided between lecture and collaborative work. To a large
extent, the class is “flipped,” meaning that you are responsible for watching
video lectures and working through online tutorial materials—outside class—as
well as collaborating with your team outside class, so that a substantial
amount of class time can be devoted to group work on the project, including
frequent in-class presentations by students, code reviews, brainstorming, etc.
Students are expected to work at least eight hours per week outside class, making
this a 4-unit course (thirteen hours of effort per week).


### Grading

10% quizzes, 20% labs, 30% individual projects, and 40% group project

All work will be done using the version control system Git. The Git repository
is not merely a mechanism for submitting work, but the way you will work with
code and text throughout the course. You will be expected to be a Git
expert by the end of the course.

There will be periodic, short quizzes in class.

The weekly [labs](|filename|/pages/labs.md) will focus on the analysis of
functional Magnetic Resonance Imaging (MRI).  Functional MRI (fMRI) allows
scientists to localize which parts of the brain are associated with specific
cognitive tasks.  There is no expectation that you will have a background in
neuroscience. You will learn everything you need to know about the method in
the course. The intention of focusing on fMRI data is merely to provide a
concrete problem domain that exemplifies the types of programming and
statistical challenges present in many statistical applications.  Additionally,
the weekly labs will prepare you---through a series of graded exercises---with
the skills and background you will need for the Stat 159 final project.

For the first half of the course, there will be a number of individual projects
to develop the basic computational skills and development habits the students
will need for their final group projects.  The group projects will be the
primary focus for the last half of the semester.  There will be regular
milestones that will involve code submissions, code review, and short
presentations.

For students registered in Stat 159, the final group project will involve fMRI
and will build on the material covered in the weekly labs.  While there will be
a number of regular milestones, the final deliverable for the group project
will involve a poster session and project report.

For students registered in Stat 259, you will need to determine the scientific
question and identify the data sources for your group projects.  You are
welcome to choose something from your own scientific field; you are also
welcome to pursue something in fMRI, but will need to do something different
than the Stat 159 project.  The final deliverable for the group project will
involve an oral presentation and project report.  You will also be assigned to
help one of the Stat 159 final project groups.

### Textbook

Readings will be assigned weekly and will mostly consist of articles and
tutorials.  Examples of the assigned articles are listed below.  Assigned
tutorials will vary per semester, but there will be an emphasis on using
official project documentation.

## Syllabus

### Week 1

Introduction and course overview. What is the difference between
reproducibility, replicability, verifiability, and auditability? Why is
reproducibility important to the scientific method?

Overview of toolstack for the course.  Introduction to the command line
interface, the filesystem hierarchy, and working with text files. Introduce
version control with Git focusing on conceptual model and basic objects. 

**Reading** 

* Buckheit, Jonathan B., and David L. Donoho. Wavelab and reproducible research.
  Springer New York, 1995.
* Preeyanon, Likit, Alexis Black Pyrkosz, and C. Titus Brown. "Reproducible
  bioinformatics research for biologists." Implementing Reproducible Research
  (2014): 185.

### Week 2

Introduction to Python and the scientific Python software stack.  Python data
structures and control flow.  Basic NumPy, SciPy, and matplotlib.

Introduce the Duke/Potti cancer genomics scandal.  Basic exploratory data
analysis of the microarray data from the Duke/Potti scandal.

**Reading**

* Perez, Fernando, Brian E. Granger, and John D. Hunter. "Python: an ecosystem
  for scientific computing." Computing in Science & Engineering 13.2 (2011):
  13-21.
* Baggerly, Keith A., and Kevin R. Coombes. "Deriving chemosensitivity from
  cell lines: Forensic bioinformatics and reproducible research in
  high-throughput biology." The Annals of Applied Statistics (2009): 1309-1334.

### Week 3

Introduction to functional programming in Python including iterators, generators,
list comprehension, zip, map, enumerate, etc.  Unit testing in Python.  More advanced
Git. Continue working with the Duke/Potti cancer genomics data.

**Reading**

* Millman, K. Jarrod, and Fernando Pérez. "Developing Open-Source Scientific
  Practice." Implementing Reproducible Research (2014): 149.

### Week 4

Additional Python packages for scientific programming including for example
statsmodels, scikit learn, and scikit image.

**Reading**

* [Python Scientific Lecture Notes](https://scipy-lectures.github.io/)

### Week 5

Refresher on the scientific problems and the statistical issues. Estimation,
prediction, hypothesis testing, confidence sets, robustness, nonparametrics,
abstract permutation tests, Monte Carlo, pseudo-random number generation.
Framing the scientific question as a quantitative statistical question. All
theoretical topics will be explored from a practical perspective using Python.

**Reading**

* Lecture notes

### Week 6

Introduction to the scientific problem for the semester (the substantive
scientific question the class will address will vary by semester) and the data
sources for the project. Example topics: recidivism in Federal prisons,
earthquake prediction, effect of packstock use on the Yosemite Toad population.
(Note: Graduate students will be expected to come up with their own scientific
questions for the final project. But they will also be required to understand
the problem that the undergraduates are assigned as it will serve as a
case study for future lectures.)

**Reading**

* Reading will vary every semester depending on scientific question

### Week 7

Introduction to project organization and process automation including: Python
packages and setuptools; makefiles; markdown, reStructuredText, and LaTeX; and
automated testing and continuous integration. Collaborative workflows with Git.

**Reading**

* [The Hitchhiker’s Guide to Packaging](https://the-hitchhikers-guide-to-packaging.readthedocs.org/en/latest/) 

### Week 8

Discussion of bottlenecks. Refine scientific and statistical vision. Outline
analysis strategy. Mini-lectures on statistical and computational tools needed
to complete the project.

**Reading**

* Reading will vary every semester depending on scientific question

### Week 9

Introduction to software architectures and design patterns.  What is software
architecture? What are design patterns? Overview of key principles of software
architecture. Review several architectural patterns and styles including
streams and filters, clients and servers, split-apply-combine, and map-reduce.

**Reading**

* Garlan, David, and Mary Shaw. "An introduction to software architecture." (1994).

### Week 10

Discussion of bottlenecks. Refine scientific and statistical vision. Outline
analysis strategy. Mini-lectures on statistical and computational tools needed
to complete the project.

### Week 11

Parallel and cloud computing.  Brief overview of computer and network
architectures.

Tuesday--present progress.
Thursday--code review and reproducibility review.

**Reading**

* Lecture notes

### Week 12

How to give good talks and posters; examples of bad talks and posters.
The good, the bad, and the ugly of data visualization.

### Week 13

Tuesday--present progress.
Thursday--code review and reproducibility review.

### Week 14

Tuesday--Lightning talks in class.
Thursday--feedback on the talks.

### Week 15

Tuesday--polish poster presentations.
Thursday-- 3-hour session of public poster presentations.
