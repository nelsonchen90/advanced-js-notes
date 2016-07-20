#agile sketchpad
## 
````
**Manifesto**
Individuals and interactions > processes and tools
working software > comprehensive documentation
customer collaboration > contract negotiation
responding to change > following a plan
````
## try to solve small problem at a time

 small design-build-test-deliver
 
3 agile methodologies: SCRUM - KANBAN - **XP**

1. Values: 
  * Courage 
  * Feedback 
  * Communication 
  * Respect 
  * Simplicty

2. Principles: 
  * Improvement - not start to perfect
  * baby steps - stability
  * humanity - 
  * self-similarity - standup is like kickoffs (small things like bigger things)
  * reflection
  * Economics - dev vs customer to have meaningful conversation
  * Quality - fit for purpose (not poor quality code)
  * accepted responsibility: story points-given by dev vs story value-given by customer
  * flow - have continuous progress
  * Redundancy - work in pairs, test is also a redundancy of the code
  * mutual benefit - both working equally, company vs employee
  * diversity - bring perspectives to the problem solving
  * failure - should no be afaird to fail

3. Practicese:
  * Incremental design
  * Whole team
  * stories
  * weekly cycle
  * quarterly cycle
  * pair programming
  * test-first programming
  * Information workspace -> how the project is doing (velocity, values, progress)
  * energized work -> fixed work day to avoiding long hour at the end of projects
  * 10 min build
  * CI
  * sit together
  * Slack - help out when needed, never run out of work

# Each iteration should deliver complete functionality (story should be backend-front)

### User story -> pairing(UI-Server) -> design(small amout, just to make it work) -> write automated test -> build&refactor
User stories: As a *cab driver*, I want to **see my next passenger on a map**, so that __I don't waste time looking for them__

**user**: customer
**want to**: description of the feature
**so that**: why the story is writtern 

#### Story point v.s value point
  * story point: time to finish the story
  * value point: user value- used to negotiate when it's blocked

#### Story: should pass **I.N.V.E.S.T.** test - Bill Wake
  * I.ndependent - **strive for**: stories should be able to be implemented in any order
  * N.egotiable - Summary should remain the same while the acceptance criteria is negotiable
  * V.aluable - Business value-> **so that** of summary
  * E.astimable - customer-> value, dev-> time (trial code=spike)
  * S.mall - no longer than an iteration
  * T.estable: customer should have set of acceptance criteria, otherwise they don't really understand the story

#### Estimate - relative not absolute
 + Story points: Fibonacci sequence -> 1, 1, 2, 3, 5, 8, 13, 21, 34, 55.. F(n+1)/F(n)~= 161.8% => 60%inc
 + Value points: same

=> WIRING: ValuePoint/StoryPoint = BFTB (bang for the buck). Deliver the higher BFTB first


# Technical practices
 * test first programming
  * scope creep: bit by bit, software need to do more -> fix the scope what dev going to code
  * intentions: doc(can get out-of-date), test won't (will break)
  * improves design: reusable
  * progress: force the code to do something useful
  * Type:
   + acceptance: real copy of system
   + unit: 
   
   e.g: 
   unit tests checks the component is using correctly whil acceptance test checks the if we are building the application we need
 * 10 min build
  * BUILD-DEPLOY-TEST
   + avoid overlaps test
   + parallel
   + cloud
   + functional test and performance test separately
   + don't write unit test as acceptance test
 * contiuous intergration
  * working type:
   + async: code code -> build -> code 
   + sync: code code -> wait (build) 

# Pair programming
 * Sharing
 * Start quickly
 * Synergy (1+1>2)
 
#### To avoid bad pair programming (A. wants to do all the work, B. doesn't want to do anything)
 * Rally driving - almost no code review
  + driver - with keyboard
  + navigator - look at acceptance criteria, design test and code
  + switching roles
  + pairs need to be split regularly

# Retrospective - refactoring the team work
 * Simplicity - low tech
  + ticky notes
  + fast
 * feedback
 * courage
 * respect
 * communication
 
#### How it look like
no comments on individuals.
0. any one can host the retro
* what went well
* what went not so well
* what we learned
* any puzzles?

1. pass sticky note - no shout out, more honest, judge by their own
2. grouping similar notes
3. prioritize the groups
4. open for comments for groups
#### to create actions

# Standups
* short time - more time writing code
* stay focused
* easy to schedule
1. lead can be changed: what did, going to do, blockers
2. stop long report
3. ban written notes
4. chicken and pigs

# Story board
 + physical - accessibility
 + BUSISNES ANALYSTS, DEVELOP, TESTERS
  * TODO
  * PLANING
  * DEVELOP
  * TEST
  * DONE
 + LOG JAM 
  * KANBAN
   + pull production
    1. each column should have max story size/number
    2. Planned vs Planning, Developed vs InProgress

# Workspace
 * burn up chart instead of burn down
  1. current scope points
  2. x - time, y - story points
  3. when new points added, the current scope points will go up

# Roles in agile team
 * customers - guide the team to work on highest value work
 * developers - devlier the code
 * business analysts - help with customer to define the stories, *define the vocabulary*
 * tester - pair with BA to generate business scenarios, will know what the software is suppposed to DO. Regression test should be automated. might still do manual testing on new features
 * architects - can pari with tester
  * non-functional requirements - techonology, performance criteria, security, data standards
 * product owner - end the project when no longer economic sense
