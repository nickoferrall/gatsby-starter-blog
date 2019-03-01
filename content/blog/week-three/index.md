---
title: 'Labs: Week 3'
date: '2019-03-01'
---

### Accomplishments this week

This week our team worked on SendGrid API, Auth0 Management API, the Refreshr (quizzes) questions and merge conflicts!

Our functionality is largely complete but bringing everything together has been challenging. Merge conflicts have slowed us down but we feel that we're nearly there in terms of functionality.

I personally worked on building the landing page, Auth0 and I've started working on Typeform too.

### Working in a team

Working in a team of 5 has been challenging and highly rewarding.

Most of our Lambda experience has involved us working solo - learning new material and completing a project each day. My main takeaways from working in a team are:

- Working with others drives me to work harder. If you're working on a solo project, you're only letting yourself down if there are weaknesses. With a group, you're letting others down too. That extra pressure has helped me to improve my work.
- Communication is exceptionally important, particularly in development. The best way to avoid merge conflicts and to help each person maximise their time is by being explicitly clear with what everyone is working on. Our group meets up 3 times per day to discuss what we're working on and we regularly use Slack and Trello to stay on top of things. I feel that we're very strong in this area.
- I feel that we were all slightly too positive about our team's accomplishments this week and we didn't realise how much work there was left to do. Often pulling together different features takes more time than expected.

## Tasks Pulled

- Task: Landing Page V1
- Trello: https://trello.com/c/SuGSsJQb/2-landing-page-v1
- Github: https://github.com/Lambda-School-Labs/labs10-student-follow/pull/70

---

- Task: Landing Page Updates
- Trello: https://trello.com/c/JwJ85xfK/81-landing-page-updates
- Github: https://github.com/Lambda-School-Labs/labs10-student-follow/pull/78

---

- Task: Auth0 Management API
- Trello: https://trello.com/c/VC8jxOCO/83-auth0-management-api

---

#### Detailed Analysis on Auth0 Management

The Auth0 Management API provides functionality to add Rules to Auth0. The rules can include restricting access to only certain email address, IP addresses, locations and more.

We want to restrict access to protected routes to only authorised teachers. To do this, we created a rule that whitelists authorised email addresses.

![rules](Rules.png)

Within each rule, you can manually edit the JavaScript provided by Auth0.

![JS](JS-within-rule.png)

Now, only users that login with the whitelisted email addresses are provided access. User that login with a different email address, will get an unauthorized error.

![Login](Login.png)
