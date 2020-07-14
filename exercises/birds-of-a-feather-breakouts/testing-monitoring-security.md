# Breakout: API Testing, Monitoring, and Security

## Key questions
Taking from the [API Lifecycle Framework](https://github.com/switzersc-usds/cms-api-framework/blob/master/api-lifecycle-framework.md), some key questions related to testing, monitoring, and security include:

Testing:
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

Security:
* Do we allow read and write access to all users, or only certain permissions for certain users?
* As a user, can I use the same credentials or credentialing pattern across multiple APIs from the same provider (e.g. CMS)?
* Is getting access to the API straightforward and timely?
* What is the highest rate limit we can reasonably allow per user? Is that good enough for the user's needs?

Monitoring:
* Do I know who is using my API and how?
* Can I see when and where my API is having performance issues or errors/exceptions?
* Am I meeting my SLAs?
* Do I know before my users when my API goes down?
* Can I monitor metrics related to progress towards product goals?

What other key questions should API teams at CMS be asking as they develop their strategy for testing, monitoring, and security? 

## What's working
What's working well on your teams with regard to testing, monitoring, and security?

## What's not working
What's not working so well on your teams with regard to testing, monitoring, and security? What could be improved?

## Shared best practices and values
As a group, identify and agree upon three best practices or shared values you think all API teams at CMS should follow regarding testing, monitoring, and security. 

If you can all agree on more than 3, go for it!