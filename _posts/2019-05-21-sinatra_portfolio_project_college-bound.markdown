---
layout: post
title:      "Sinatra Portfolio Project: College-Bound"
date:       2019-05-21 17:55:55 +0000
permalink:  sinatra_portfolio_project_college-bound
---




My Sinatra portfolio project centered around a sophomore or junior in high school who is approaching her college application process. Specifically, the student (User) would create her colleges, interact with them in terms of editing and deleting, and be able to access them throughout the process via registration and then subsequent logins as she returned to the application. 

In approaching this second portfolio project, I knew to establish strict organization.  My organizational strategy included the following: 
a. Using Corneal gem to create the file structure
b. Mapping out the idea on paper with associations, control flow, models
c. Determining the flow of the app that the User would be experiencing
d. Creating a boilerplate template of the seven RESTful routes in both of the controllers

I met with my Sinatra portfolio project section lead to discuss my laid-out plans. That was instrumental in that my initial idea had logic holes and unwarranted complexity.  For example, I had a join table (there would be three controllers- Students, Colleges, and Guardians/Parents), unnecessary college attributes like selectivity, tuition, academic concentrations, and bells and whistles that I’d wanted to learn like how to employ testing (ie TDD) into this application.   I’d  grappled with the association(s), whether Colleges belonged to Students or if Students had many Colleges.  I resolved that either association could work and be coded well. 

After installing Corneal,  I used previous lessons and labs and coded the basic 7 RESTful routes in the Student and College Controllers.  While doing so, I tried to think through what each route needed to accomplish. I thought of the 'where' (the action) as well as the 'how' (the method) that I would need in my Views.  Some things that  were problematic: 
a. The difference between rendering and re-directing
b. Singularity versus plurality of words like ‘college’ to ‘colleges’
c. Conditional Use- when to use then, when to stop the elsif 
d. What made sense for redirecting ---where would the User want to go?

The hardest problem and the most crucial element to fix was how to disallow other users from editing and deleting others’ resources.   That was key to this entire operation and one thing that I had missed over the four weeks.  This major omission was only unearthed as I tried to register and to login with a different user name than “Jane Doe” and was immediately sent to Jane Doe’s entire index display of colleges.  That wasn't too problematic but the fact that another User could edit and then delete Jane's resources was alarming.  That would be synonymous to a User signing in to her bank account and being able to see the previous account holder’s bank balance.   

Another difficult part  was seemingly the simplest-sounding one-figuring out the flow of the work.  That flow of what the User would experience as she went through the Sinatra application was grounded in my College Controller were I needed to code  redirects, renders and routes.  It was profoundly crippling for  me.

