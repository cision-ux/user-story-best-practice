# User Story Best Practice documentation and presentation
[documentation site](http://awkale.me/user-story-best-practice/)

## Version (theme) vs Epic vs user story vs task
Agile development uses four clear delivery methods to bring structure to any project: **versions**, **sprints**, **epics** and **user stories**.
  * A **version** is a set of features and fixes released together as a single update to your product. Assigning issues to versions helps you plan the order in which new features (stories) for your product will be released to your customers. A version can be made up of multiple sprints
  * A **sprint** is a set period of time during which specific work has to be completed and made ready for review
  * An **epic** captures a large body of work. It is essentially a large user story that can be broken down into a number of smaller stories. It may take several sprints to complete an epic.
  * A **user story** (represented as an issue in Jira) captures a description of a feature from an end-user perspective. The user story describes the type of user, what they want and why. A user story helps to create a simplified description of a requirement. User stories are broken up into individual tasks that make up the story (represented as sub-tasks in Jira).

## Why use user stories?
* Keep yourself expressing business value
* Avoid introducing detail too early that would prevent design options and inappropriately lock developers into one solution
* Avoid the appearance of false completeness and clarity
* Get to small enough chunks that invite negotiation and movement in the backlog
* Leave the technical functions to the architect, developers, testers, and so on

## Creating a user story
* The goal is to outline a particular value to the customer that a team can deliver in an iteration using a few short sentences, ideally using non-technical language. While traditional requirements (like use cases) try to be as detailed as possible, a user story is defined incrementally, in three stages:
  * The brief description of the need
  * The conversations that happen during backlog grooming and iteration planning to solidify the details
  * The tests that confirm the story's satisfactory completion

##  What makes a great user story
  * They don't go into detailed requirements.
  * User stories must be written using the following template:
  > As a [type of user], I want [goal] so that I [receive benefit].
  > **End user goal:** _______________________________
  > **End business goal:** _____________________________
  > **Acceptance criteria:**
    * product defines any initial functionality requirements they can think of
    * this is a loose outline that will be finalized through wireframes, flows and discussions
    * acceptance criteria must be finalized before dev starts
  > **Measurement of success:** ___________________________
     * Measurement of success is the way in which we will prove the story was successful in meeting the user and business goal defined above. This will initially be left blank and will be determined through conversations with research, ux and product. This must be finalized before dev starts.

## Example user story
  > As a purchaser on the website I want the ability to pay with a credit card, so that I may immediately confirm my purchase.
  > **End user goal:** Purchase items with a credit card
  > **End business goal:** Increase purchases
  > **Acceptance criteria:**
    * Accept Discover, Visa, MC
    * Validate credit card number
    * Validate expiration data and CVV
    * Validate billing address
    * Generate success/failure messages after processing
  > **Measurement of success:** ___________________________

> “Stories are deliberately not fleshed out in detail until they are ready to be developed, you only need enough understanding to allow prioritization with other stories.” - Kent Beck

* A well-formed user story will follow the INVEST mnemonic.
  * I – Independent
    * Stories are easiest to work with if they are independent. That is, we'd like them to not overlap in concept, and we'd like to be able to schedule and implement them in any order.
  * N – Negotiable
    * A good story is negotiable. It is not an explicit contract for features; rather, details will be co-created by the customer and programmer during development. A good story captures the essence, not the details. Over time, the card may acquire notes, test ideas, and so on, but we don't need these to prioritize or schedule stories.
  * V – Valuable
    * A story needs to be valuable. We don't care about value to just anybody; it needs to be valuable to the customer. Developers may have (legitimate) concerns, but these framed in a way that makes the customer perceive them as important. This is especially an issue when splitting stories.
    * Think of a whole story as a multi-layer cake, e.g., a network layer, a persistence layer, a logic layer, and a presentation layer. When we split a story, we're serving up only part of that cake. We want to give the customer the essence of the whole cake, and the best way is to slice vertically through the layers. Developers often have an inclination to work on only one layer at a time (and get it "right"); but a full database layer (for example) has little value to the customer if there's no presentation layer.
  * E – Estimable
    * A good story can be estimated. We don't need an exact estimate, but just enough to help the customer rank and schedule the story's implementation. Being estimable is partly a function of being negotiated, as it's hard to estimate a story we don't understand. It is also a function of size: bigger stories are harder to estimate.
    * Finally, it's a function of the team: what's easy to estimate will vary depending on the team's experience. (Sometimes a team may have to split a story into a (time-boxed) "spike" that will give the team enough information to make a decent estimate, and the rest of the story that will actually implement the desired feature.)
  * S – Small
    * Good stories tend to be small. Stories typically represent at most a few person-weeks worth of work. (Some teams restrict them to a few person-days of work.) Above this size, and it seems to be too hard to know what's in the story's scope. Saying, "it would take me more than a month" often implicitly adds, "as I don't understand what-all it would entail." Smaller stories tend to get more accurate estimates.
  * T – Testable
    * A good story is testable. Writing a story card carries an implicit promise: "I understand what I want well enough that I could write a test for it." Several teams have reported that by requiring customer tests before implementing a story, the team is more productive.
    * "Testability" has always been a characteristic of good requirements; actually writing the tests early helps us know whether this goal is met. If a customer doesn't know how to test something, this may indicate that the story isn't clear enough, or that it doesn't reflect something valuable to them, or that the customer just needs help in testing. A team can treat non-functional requirements (such as performance and usability) as things that need to be tested. Figure out how to operationalize these tests will help the team learn the true needs.

* User story outline
  * User Story
  * End user goal
  * End business goal
  * Acceptance Criteria /this isn't finalized until the story is ready for development/
  * Measurement of Success /this is added after conversations with product, ux and research/

## User story dos and don’ts
* DO focus on a specific user
  * Avoid the generic role of User when writing user stories. User stories are about all of the role who interact with the system or who realize some value or benefit from the system.
* DO provide acceptance criteria
  * The product owner should list as many acceptance criteria as possible in order to clarify the intent of the story. Acceptance criteria will become QA test cases
* DO have conversations
  * update acceptance criteria and user story details based on your conversations
* DONT go into detailed requirements
* DONT provide the solution
  * User stories must be focused on the user need and benifit not solution


## Advantages of Jira; tips and tricks
  * Type `c` for shortcut to creating an issue
  * Add issue to epic - via backlog agile board or when viewing story
  * take advantage of Jira's text formatting for easy to follow descriptions

## Examples of best in class and ineffective user stories
  * [epic - As a customer of PR Newswire, I would like a new news release template for my thought leadership content](https://prnewswire.jira.com/browse/PRNCOM-4564)
    * [story - As a user I want to be able to see that there is more information below the cropping of an infographic so that it is easier to know that it should be enlarged](https://prnewswire.jira.com/browse/PRNCOM-4869)
  * [UX wireframes](https://prnewswire.jira.com/browse/CNW-58)
  * Agility: [Epic-Display Audience Data Within Agility](https://prnewswire.jira.com/browse/CWP-6196)
   *[story - As a monitoring user, I would like to see mentions with ComScore audience data available within my results, so that I can qualify the message based on reach of the outlet.](https://prnewswire.jira.com/browse/CWP-6297)
   * [story - As an Agility user, I would like to be able to construct a people search using the audience score for the outlets they work for, so I can better isolate influencers.] (https://prnewswire.jira.com/browse/CWP-6207)
  * Visibility Reports: Earned Media, International Release Consolidation
   * (Too technical)[Earned Media Pickup processing and analysis](https://prnewswire.jira.com/browse/VREP-3474)
   * (As a wire customer I want to understand the full value and impact of a PRN distribution so my purchase decision is validated)[https://prnewswire.jira.com/browse/VREP-2674]

## IN-SESSION EXERCISE YOU’LL LEAD:
* Break into groups of 2-3
* Present feature
* As a group write an epic and a few user stories
* Review epic and user stories and dicuss
