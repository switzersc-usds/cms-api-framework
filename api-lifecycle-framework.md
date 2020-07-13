# API Lifecycle Framework

## Strategy
Strategy is all about the *why*. You need to know what problem you're seeking to solve, and for whom, before you can begin designing and building the solution. 

Key questions:
* What is the problem(s) we are trying to solve? 
* Whose problem is it? Are they the same as our user? If not, what is our user's problem?
* Why would someone want to use our API?
* How are users involved in the product roadmapping and development process?
* How do we measure impact and success?
* When does strategy change?

## Design
API design is how users will interact with your API. It includes what data is available, how that data is structured, how API messages are formatted, and what actions an API user can take. It can also include authentication mechanisms, although we address that in the Security section below. 

Key questions:
* What is the learning curve for my users when they onboard to my API?
* Does the API resource model make sense to my users?
* Is my design continuously informed by user feedback?
* Am I using and complying with open standards and conventions such as JSON, FHIR, or HTTP status codes?
*  What kind of architectural approach makes sense for solving the problem identified in my API strategy? E.g. REST, GraphQL, etc.

## Development
API development doesn't look a whole lot different from other software development. 

Key questions:
* Does the dev team follow modern best practices (e.g. code review, version control, automated testing)?
* Is there a continuous integration and delivery pipeline?
* Do developers feel ownership over what they build? Can they scratch their own itches?
* Is the code open source? Does it utilize open source?


## Documentation
Good API documentation isn't just about text-based documentation of available endpoints. API docs should be a living, usable product in their own right, driven by user experience, kept up to date, and tested. 

Key questions:
* Is there a machine readable API definition (e.g. OpenAPI/Swagger)?
* Is my API definition or any part of my documentation auto-generated from code?
* Are the docs up to date and accurate?
* Is my documentation tested during continuous integration?
* As a user, can I consume this API with no intervention from the support or dev team?
* As a user, is it clear why I would want to use this API and how to get started?
* Is any part of the documentation interactive? For example, as a user, can I make a test API call or generate client side code directly from the docs?


## Deployment
Like development, API deployment doesn't look much different than typical software deployment. 

Key questions:
* Can I deploy as needed with zero downtime?
* Who determines when releases should happen?
* How are deployments packaged?
* Am I using a continuous integration and deployment pipeline (CI/CD)?

## Testing
Testing helps you catch bugs and issues before they reach users. Some amount of testing is probably part of your normal software development process, such as automated code tests that are developers write and that get run for every new feature. 

Key questions:
* Do I have or need the following test types:
    * Usability and UX (incl. documentation)
    * Unit 
    * Integration 
    * Performance and load
    * Security
    * Standards compliance
    * Production testing
* Do I have any of the above as part of my CI/CD pipeline?
* How much testing is enough?

## Security
Security can get pretty heavy, especially at CMS! We don't want to get into all the details of compliance and risk mitigation guidelines and requirements here, but rather focus on API-specific security concerns such as access and usage. 

Key questions:
* Do we allow read and write access to all users, or only certain permissions for certain users?
* As a user, can I use the same credentials or credentialing pattern across multiple APIs from the same provider (e.g. CMS)?
* Is getting access to the API straightforward and timely?
* What is the highest rate limit we can reasonably allow per user? Is that good enough for the user's needs?

## Monitoring
We monitor APIs for upholding our SLAs (Service Level Agreements) such as uptime and performance, as well as for better understanding our users and measuring success. 

Key Questions
* Do I know who is using my API and how?
* Can I see when and where my API is having performance issues or errors/exceptions?
* Am I meeting my SLAs?
* Do I know before my users when my API goes down?
* Can I monitor metrics related to progress towards product goals?


## Discovery & Promotion
The attitude "If we build it, they will come," is a pretty dangerous one to have. You can't expect users to use your API just because it's there, or just because it's better than whatever the previous alternative was (or if they feel stuck with using it, they may not be happy about it). Having a plan for how users will discover and onboard to your API is key for adoption and making sure you stay in touch with your target audience. 

Key questions:
* Are my users internal or external?
* How do my users find out about my API?
* What are my usage goals?
* Who owns the discovery experience and how will it be maintained?


## Change Management
Change management is often referred to simply as versioning, but it also encompasses the work done around versioning: deciding what goes in minor or major patches, communicating new versions to users, and offboarding users from deprecated versions.

Key questions: 
* What changes are considered breaking?
* How long do we want to or can we maintain previous versions?
* How do we communicate changes with our users? How do we measure the success of this communimcation?
* What versioning strategy do we want to use and how is this documented?

# References

[Continuous API Management](https://www.oreilly.com/library/view/continuous-api-management/9781492043546/), by Mehdi Medjaoui, Erik Wilde, Ronnie Mitra, Mike Amundsen

