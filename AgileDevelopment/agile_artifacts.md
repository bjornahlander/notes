## Agile Artifacts
There are virtual and concrete artifacts defined by agile approaches
### Virtual artifacts
 * Code
 * Tests
 * User Stories
 * Story Points
 * Velocity
 * Definition of Done
 * Working Space
 * Product Backlog, Iterantion backlog
#### Code
Code (working code) is center in the agile universe
Focus on code to shift attention to concrete results
#### Tests
Unit tests in xUnit style
 * Method executes test
 * Set up conotext and reset context
 * Assertion

Maybe use them as specification och class invariants, preconditions and
postconditions, Design by Contract.
Regression test suite is a colleciton of unit tests and has the purpose of
preventing old bugs to reappear due to versioning problems, incomplete bug fixes
etc.
Incremental by nature
#### User Stories
A description of a fine-grain functionality as seen by its users
Described by the triple `{ category of user, goal, benefit }`.
> **As a** staff member, **I want to** cancel a bookin **so that** reasonable
> requests for policy exceptions can be accomodated.

We need to define a refactor or a stack change as a user story otherwise it's
not customer driven.
Problems can occur with user stories not them selves taking effort into account
and that one might end up with complex systems since individual systems might be
built with respect to individual user stories. "See the whole" is a lean
principle and a user story doesn't see the whole by design.
User stories is not a replacemnt for writing genereal requirements.
One could sequentially work on domain model in first phase and then shift some
of the focus to user-visible functionality.
One could also work on them both in parallel, but the important thing is that
there needs to be a balance between them.
#### Story Points
Important for project control is estimation of effort and measurement of
progress. Story points are used to estimate effort for user stories and to
measure progress. Previous alternatives inlude:
 * SLOCs (lines of code), but are we 90% or 40% done with 85k lines?
 * person-months (-days), nice for HR and IT cost estimate but hard to tell
   effetiveness.
 * Function points, estimates #functions of the system. What about OOP?

Story points are **relative** indicators, only counted for **implemented** user
stories (no waste!) and **non-delivered artifacts will not count towards
progress** (like docs, plans, requirements). Story points can be used to compare
progress between iterations. Fibonacci sequencce is one way of assigning story
point values.

#### Velocity
How many story points have been (will be) achieved in the current (next)
iteration? Nice for estimation and measurement. Useful for adjusting story point
assignment in coming iterations (convergence).

#### Definition of done
Really important to have a strict definition of when we're done since it
minimizes waste. Example defintions are releasable, unit- and
integration-tested, acceptance test, deployed to demo server etc

#### Working Space
XP argues for working spaces with no physical separation (bullpens) aswell as
offerings of more private spaces (cubbicles). This is based on assumptions about
everbody being in the same office. Distributed development model is also
possible. When applicable go with everyone-under-one-roof.

#### Product backlog, iteration backlog
Instead of comprehensive requirements documentation replacements can consist of a 
collection of user stories as a whole (product backlog) and a collection of user stories
for a particular iteration (iteration backlog). Categories Remain, in progress,
done.

### Tangible artifacts
 * Story card, task card
 * Task and Story Boards
 * Burndown and Burnup charts
 * Impediment

#### Story Card, Task Card
In order to standardize the form in which user stories are written, one could
use simple hand-written notes. 

#### Task and Story Boards
It is important to keep the team constatly aware of don, in progress and
remains, when focusing on delivering the best customer value in the least
possible time. Advantages include
 * Keeping track of velocity
 * Boosting team morale (GTD)
 * Discouraging waste (some work not shown)

#### Burndown and Burnup charts
Burndown chart is remaining units of work plotted against time. (Derivative is
velocity). Linear line can be added to serve as a reference for the ideal
project. Burnup chart shows progress, rather than remaining work, in a cumulative
way. For both charts work is counted if it is deliverable and finished. 

#### Impediment
Impediment is any matter that damages the progress of the project: hardware no
there, delay in producing a module needed by the project. 

#### Waste, technical debt, dependency, dependency charts
These belong in the agile discussion in a negative way, obstacles to be avoided.
**Waste** avoidance is a concern in all agile aproaches. It includes all the
products, material/virtual, not delivered. Design documents, unfocused meetings
etc. Waste takes many forms due to the insistence on code and tests as the only
products worthy of consideration.

**Techincal debt** builds during a proejct and consist of code with unsatisfactory 
quality. This is fought with refactoring.

**Dependencies** are constraints between development elements. Story B needs
story a to be finished. Goal is to minimize dependencies but this is hard. 

**Dependency charts** (Gantt charts) can be used as a tangible artifact to
visualize and manage the tasks and their dependencies in order to schedule work. 


