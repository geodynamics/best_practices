# Software Training Best Practices for the CIG Community

## Executive Summary

ADD STUFF HERE


## Tutorials
*Structured sessions focused on teaching participants how to use specific modeling tools.*

### Preparation (for instructors)

Each tutorial should begin by defining the goals, topics, and learning objectives of the tutorial. Instructors should consider stating what is in and out of scope. Factors that may influence choices include:

* Scientific background and computational skills of participants.
* Obstacles encountered in progressing along the learning curve.
* Common problems encountered by users.

Make your presentation equal access. Practice Universal design: https://www.washington.edu/doit/equal-access-universal-design-your-presentation

### Preparation (for participants)

Instructors should describe what participants need to know or do in advance of the tutorial (prerequisites). Examples: 

* Be familiar with command line interfaces.
* Install virtual machine on a laptop.
* Install software packages: A (version x), B (version y), and C (version z).
* Useful or recommended skills: e.g., knowledge of Python
* For advanced tutorials: participation in beginner tutorials or use of the software may be a prerequisite.

### Content

* Discuss the history and scientific basis for the software and what scientific problems it can address.
* Outline the tools, software dependencies, and workflow (setup, running, postprocessing).
* Describe the governing equations and the numerical implementation.
* Instructors run end-to-end examples in step-by-step demonstrations.
  * Examples build in complexity and follow the workflow of real research problems.
  * Each example includes a list of the software features discussed.
  * Include “what to do when things go wrong”, such as how to parse error messages and diagnose problems.
* Provide data files of the output or snapshots from visualization of the output so users can verify the have successfully run each example.
* Encourage participation in the user community.
  * Describe how to get answers to questions and what level of support to expect.
  * Provide a list of possible directions and extensions that participants can use as a guide for moving forward.
  * Include how to give credit to developers in presentations, publications, etc.

### Logistics

* Partition the tutorial into discrete chunks with time between sessions for users to run example problems at their own pace.
* Consider separate help sessions to troubleshoot installation problems.
* Maximize accessibility to users.
  * Tutorial content runs on computers used by participants.
    * Installed on own machines (preferred), OR
    * Central resource (cluster or cloud) that is publicly accessible.
    * Examples can be run using free, preferably open-source, software.
    * Version numbers of the software used in the tutorials should be clearly referenced, especially if they are third-party tools (e.g., ParaView visualization software).
    * Any commercial software used should have a free trial so it is accessible to new users during the tutorial.
* Tutorial sessions are archived and available on demand.
  
  Participants can review materials at their own pace afterwards. New and other users can access the tutorial later rather than waiting for the next tutorial. Participants can review materials from previous tutorials.
  
  * Slides and videos from the tutorial are archived and posted on the web.
    * Videos should be of sufficient resolution so that the text is legible and participants can follow what the instructor is going.
    * Videos of each session should be  broken into logical pieces.
  * Include the list of questions asked and corresponding answers.
* In-person versus online tutorials
  * Online
    * Reach a broad audience with minimal cost.
    * Easy to record via tools like Adobe Connect. Recordings can be reused as a prerequisite for more advanced tutorials.
    * May need multiple schedules to reach more time zones.
    * Allows flexibility in scheduling sessions (e.g., similar to class schedules).
  * In person
    * Greatly facilitates interaction between instructors and participants.
    * Promotes interaction among participants.

### Assessment
  * Assess what users have learned via post-tutorial surveys .
  * CIG has a suite of standard questions (see Appendix) that instructors can use as a starting point.

### Examples
  * PyLith: https://wiki.geodynamics.org/software:pylith:start#tutorials
  * Obspy: http://krischer.github.io/seismo_live/
  * ASPECT:
  
## Hackathons
*Unstructured gatherings of principal developers and expert users focused on improving and extending modeling tools.*

* Keep the program largely free of planned activities to give people time to develop code.
* The hackathon should involve 7-10 days of focused coding.
  Five days is usually too short to make significant progress and more than ten days would be physically exhausting.
* Start with everyone introducing themselves and what their goals are for the hackathon.
  Identify experienced developers who can mentor others. This fosters more exchange among the participants by letting them know who to ask (other than the primary developers) in case of questions.
* Provide a brief introduction to git, github, …, how to submit patches, and how the patch review process will work.
* Identify key people who will be responsible for reviewing code and accepting pull requests
* At random times during the hackathon, encourage participants to show images, movies, and other results that they have obtained using the functionality they just implemented.
* Begin each day with a session in which each person has a few minutes to outline what they achieved the previous day and what they intend to work on that day. 
* Produce a hackathon report describing the accomplishments of the hackathon. Each participant would contribute a “one pager” describing their activity and results.
* OPTIMAL PRIMARY DEVELOPER/HACKER RATIO? ??? Optimal experienced: unexperienced hacker
* Add minimum requirements. What level of coding ability and subject matter expertise should the participants have?

# Appendix

## Questions for post-tutorial assessment
(1-5, NA)

### Content and format
* Did you understand the goals of the tutorial?
* Were the lectures clear? 
* Were the materials (slides, handouts) clear?
* Were you able to run the software successfully?
* Were the instructors able to answer your questions?
* Was there sufficient tinker time?
* Do you plan to use this software in your research?
* Did the tutorial meet your expectations overall?
* Did the tutorial adequately prepare you to run the code for your own research? 
* What other topics for future tutorials would be useful? (or what follow-up material would be useful?)
* Other comments?

### Logistics
* Did everything function well at the venue?
* Food? Accommodations?

### Demographics
* What is your area of expertise?
  (Pull down menu)
* Position (Pull down menu)
  * Undergraduate Student
  * Graduate student
  * Postdoc
  * Government scientist
  * University Researcher
  * Pre-tenure faculty
  * Post-tenure faculty
  * Other _______
* How many other tutorials have you participated in for this software?
  * None
  * One
  * Two
  * Three or more
