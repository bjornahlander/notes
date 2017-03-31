## Meyer Ch. 8 Agile Artifacts
There are virtual and concrete artifacts defined by agile approaches
### Virtual artifacts
 * Code
 * Tests
 * User Stories
 * Story Points
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
> requests for policy exceptions can be accomodatedi.

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


