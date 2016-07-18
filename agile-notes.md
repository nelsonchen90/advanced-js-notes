#agile sketchpad

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
