# STA 523 :: Exam 1

## Introduction

The Tour de France is a multi-stage bike race held annually in July. The race
has riders primarily cycle throughout French cities, countrysides, and 
mountains. It is considered one of the toughest endurance events in the world.
Participants will cover over 3,300 kilometers in a 23-day span.

Cycling is both a team and individual sport. Riders are members of teams, but
there are individual accolades up for grabs. Riders in first with regards
to these individual award categories wear special colored / patterned jerseys.


- Overall winner (by time): yellow jersey
- Best sprinter (by points): green jersey
- King of the mountains / best climber (by points): polka dot jersey
- Best young rider (by time): white jersey 

<center>
<img src="jerseys.jpg" width="350" height="300">
</center>


## Data

Data in your repository is from the 2019 Tour de France. To get started, read in 
`tdf_2019.rds` and create an object `tdf` with

```r
tdf <- readRDS(file = "tdf_2019.rds")
```

Most of the variables are self-explanatory. The data should be clean and
organized; maybe not in the form you want, but I did not add any issues as 
I did in Homework 4. Below are a few details on the data.

1. Time is expressed in hours:minutes.seconds.
2. Only the winning rider (team) in a stage has a real time, the time
   for others are relative to the winner's and formatted as "+hh:mm.ss".
3. `sprint` and `climber` are the number of points a rider earned in the stage.

## Tasks

You may use any R package. Include code to load your package with 
`library(package_name)`. If I do not have the package, I will install it.

#### Task 1

Use object `tdf` to create a tidy data frame that contains the following
variables. Each variable should be of the specified type given in parentheses.

* `rider_name` - full name of the cyclist, no need to change the format **(character)**
* `rider_nat` - cyclist's nationality **(character)**
* `team_name` - cyclist's team name **(character)**
* `team_nat` - cyclist's team nationality **(character)**
* `stage` - stage of the Tour **(integer)**
* `dep_city` - departure city for given stage **(character)**
* `arr_city` - arrival city for given stage **(character)**
* `classification` - stage's classification **(character)**
* `distance` - stage's distance that cyclists will ride **(double)**
* `start_date` - stage's start date, not the time **(date)**
* `time` - cyclist's time on a given stage **(character)**
* `time_rank` - rank of cyclists based on time within stage **(integer)**
* `sprint_pts` - sprint points earned by cyclist on given stage **(double)**
* `sprint_rank` - rank of cyclists based on sprint points within stage **(integer)**
* `climb_pts` - climb points earned by cyclist on given stage **(double)**
* `climb_rank` - rank of cyclists based on climb points within stage **(integer)**
* `young_rider_time` - young rider time on a given stage **(character)**
* `young_rider_rank` - rank of cyclists based on young rider time within stage **(integer)**

If a variable's value is missing, code it as `NA`. For example, some cyclists 
may have values `dns`, `dnf`, or `dq` if they did not start,
did not finish, or were disqualified, respectively. 
Similarly, most riders will not have climb points and a climb 
rank since only a few points are up for grabs in a given stage; riders missing 
these values should also have `NA` for the respective variable's value. 

<br/>

#### Task 2

1. Fix the time variables (`time`, `young_rider_time`) so each cyclist's 
   stage time is given rather 
   than just the winner's time and time back from the winner. 
   For example, rather than
   `"04:22.47", "+00:00.00", "+00:00.00", "+00:00.00", ...` in stage 1, it
   should be changed to
   `"04:22.47", "04:22.47", "04:22.47", "04:22.47", ...`. You may keep the
   result as type character or a date/time data type.
   
2. Use the data frame (either from Task 1 or after you fixed the times above)
   to create a data frame that showcases the King of the Mountains competition
   across the 21 stages. To give you an idea of what it should like in a 
   tabular form see below.
   <br/><br/>
![](task2_table.jpg)
   <br/><br/>
Only include the top 30 climbers sorted by `total_climb_points` in your final 
data frame. If a cyclist did not accumulate any points in a given stage, 
set the value to 0. Variable `rider_name` should be of type character. All
other variables should be of type integer.

<br/>

#### Task 3

Use any of the three data frames to construct a single visualization that 
depicts something about the 2019 Tour de France. A single visualization can
include subplots, but I do not want, for example, 10 unrelated graphics. Your
visualization should be well-polished with aesthetics, font size, and style
chosen appropriately. You may construct this visualization with the mindset
that it would appear in a presentation. Thus, animations are okay to utilize.

<br/>

## Essential details

#### Deadline and submission

**The deadline to submit Exam 1 is 11:59am on Friday, October 11.** 
Only the code in the master branch will be graded.

#### Rules

- This is an individual assignment. 

- Everything in your repository is for your eyes only except for the instructor
  and TAs.

- You may not communicate anything about this exam to anyone.

- You may use any online, book, and note resources. As always, you must
  cite any code you use as inspiration.

- Questions to the instructor and TAs should only be about understanding
  the data or the exam's instructions.

#### git / GitHub

You will only have one branch to start with in your repository - master. 
You may create other branches as needed, but only your work in the master 
branch will be graded. Be sure to push your work before the deadline.

#### Help

- The instructor and TAs will only answer questions about directions that may
  seem unclear and about the meaning of data variables. 

#### Academic integrity

>Duke University is a community dedicated to scholarship, leadership, and 
service and to the principles of honesty, fairness, respect, and accountability.
Citizens of this community commit to reflect upon and uphold these principles 
in all academic and non-academic endeavors, and to protect and promote a culture
of integrity. Cheating on exams and quizzes, plagiarism on homework assignments 
and projects, lying about an illness or absence and other forms of academic 
dishonesty are a breach of trust with classmates and faculty, violate the [Duke 
Community Standard](https://gradschool.duke.edu/academics/academic-policies-and-forms/standards-conduct/duke-community-standard),
and will not be tolerated. Such incidences will result in a 
0 grade for all parties involved as well as being reported to the [University 
Judicial Board](https://gradschool.duke.edu/academics/academic-policies-and-forms/standards-conduct/judicial-code-and-procedures). 
Additionally, there may be penalties to your final class grade. 
Please review [Duke's Standards of Conduct](https://gradschool.duke.edu/academics/academic-policies-and-forms/standards-conduct).

#### Grading

**Topic**|**Points**
---------|----------:|
Task 1   |  20
Task 2.1 |   5
Task 2.2 |  15
Task 3   |  20
**Total**|**60**

- *Documents that fail to knit will receive a 0*.
# STA 523 Exam 1
# ????????? powcoder

# [????????????CS???????????????????????????](https://powcoder.com/)

# Programming Help Add Wechat powcoder

[????????????](https://powcoder.com/tag/????????????/)

[java??????](https://powcoder.com/tag/java/) [c/c++??????](https://powcoder.com/tag/c/) [python??????](https://powcoder.com/tag/python/) [drracket??????](https://powcoder.com/tag/drracket/) [MIPS????????????](https://powcoder.com/tag/MIPS/) [matlab??????](https://powcoder.com/tag/matlab/) [R????????????](https://powcoder.com/tag/r/) [javascript??????](https://powcoder.com/tag/javascript/)

[prolog??????](https://powcoder.com/tag/prolog/) [haskell??????](https://powcoder.com/tag/haskell/) [processing??????](https://powcoder.com/tag/processing/) [ruby??????](https://powcoder.com/tag/ruby/) [scheme??????](https://powcoder.com/tag/drracket/) [ocaml??????](https://powcoder.com/tag/ocaml/) [lisp??????](https://powcoder.com/tag/lisp/)

- [?????????????????? data structure algorithm ??????](https://powcoder.com/category/data-structure-algorithm/)
- [??????????????? ??????????????? computer network socket programming ??????](https://powcoder.com/category/network-socket/)
- [????????? DB Database SQL ??????](https://powcoder.com/category/database-db-sql/)
- [???????????? machine learning ??????](https://powcoder.com/category/machine-learning/)
- [??????????????? Compiler ??????](https://powcoder.com/category/compiler/)
- [????????????OS(Operating System) ??????](https://powcoder.com/category/????????????osoperating-system/)
- [?????????????????? Computer Graphics opengl webgl ??????](https://powcoder.com/category/computer-graphics-opengl-webgl/)
- [???????????? AI Artificial Intelligence ??????](https://powcoder.com/category/????????????-ai-artificial-intelligence/)
- [????????? Hadoop Map Reduce Spark HBase ??????](https://powcoder.com/category/hadoop-map-reduce-spark-hbase/)
- [???????????? System programming ??????](https://powcoder.com/category/sys-programming/)
- [???????????? Web Application ??????](https://powcoder.com/category/web/)
- [?????????????????? NLP natural language processing ??????](https://powcoder.com/category/nlp/)
- [????????????????????? Computer Architecture ??????](https://powcoder.com/category/computer-architecture/)
- [????????????????????????computer security cryptography ??????](https://powcoder.com/category/computer-security/)
- [??????????????? Computation Theory ??????](https://powcoder.com/category/computation-theory/)
- [???????????????(Compute Vision) ??????](https://powcoder.com/category/???????????????compute-vision/)

