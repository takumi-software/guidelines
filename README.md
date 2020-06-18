# Guidelines

This projects represent the framework of how we love to work at Takumi software, it is intendended
to work as a reference on how to do work and also to collaborate with us. 

If you are wondering why we are called Takumi software and have sometime to get to know us more please take a look at

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/9EI3aEFANBo/0.jpg)](https://www.youtube.com/watch?v=9EI3aEFANBo)

# General guidelines for collaboration

# Our rules. 

The following rules are our way of tackling collaborative work using world class best practices
and some common sense rules too. Some of them might sound easy, if so please note that this is a compendium
of best practices and it is our framework based on experience on many projects worked over time, having these rule together
and applying them on a consistent way is what will make the best results.


- Program in [English only] Translate and correct into understandable and be thoughtful about the naming in your code.
- [No comments] Commented code is a bad practice, instead have git to store code changes. Also general commentaries are often misused to explain some obscure code or functionality, instead **use Germanic convention**  
- [DRY] Apply DRY principle "Don´t repeat yourself". If when refactoring or creating code you realize you have a duplicity pattern, redo to achieve it without repetition, if you want to learn more about it please read [DRY](https://dzone.com/articles/software-design-principles-dry-kiss-and-yagni)
- [SOLID] SOLID principles will guide our development. For more information, please read [SOLID](https://www.hashbangcode.com/article/solid-principles-php)
- [Pull Request] Any doubts regarding code solutions? Expose it with a Pull request, is better to ask for forgiveness than asking for permission, there is no better way to show your ideas and code changes thant doing through a Pull request.
- [Automate] Having recurrent tasks? Automate it somehow, you have makefile, bash scripts, etc, if you don´t know how to do this, do the Google rule.
- [Google It](www.google.com) having problems? understand the problem, you can also go beyond and post an [stack overflow question](https://stackoverflow.com/), don´t have an account ? what are you waiting for? if after doing so you still have doubts then ask a teammate for help, don´t waste time to find for answer (this means your time, your teammate's time and the project timings.)
- [TEST] Only automatically tested code should be generated (Almost all languages have automatic testing available) don´t know how to do this? go for the google rule.
- [Continuous Integration] CI software shall be added and required to pass in order to approve any pull Request. 
- [DEBUG] Whenever in doubt about why your software does not work, first debug. Debug shows you reality, you can also rely on application logs, but debugging will be almost always faster and easier, you still don´t know how to debug on your current language? you really need to invest time on this!
- [Devil is on the details] Your github activity is important, when commiting do it like if you are sure you will read this messages on a year from today, you probably will! Be explicit and accountant with your work, this means having descriptive commits.
- [Boyscout rule] Leave your code better than you found it. Boy Scouts have a rule regarding camping, that they should leave the campground cleaner than they found it, the same applies for code, if you see something is wrong in the context code where you are working at, fix it [Boyscout rule on code](https://medium.com/@biratkirat/step-8-the-boy-scout-rule-robert-c-martin-uncle-bob-9ac839778385) 

## Contributing to projects.

we work following Issues previously created on the platform. 

Every time you get to work on a new task, you should create a branch with the following structure: 

${ISSUE_ID}-kebab-case-description

Example: 

If you are assigned with the issue 53 then you would need to create your branch with a name like `53-adding-statistics-on-new-accounts`

Still doubts around the kebab case? [Learn more](https://wiki.c2.com/?KebabCase)

- [Create PR´s] create a PR ro your work even if it is partial, is the best way to anticipate possible deviations, don´t hesitate to do it as soon as you start working with an issue an assign the WIP label.
- [Structure] The tiltle of a PR must follow structure: #${ISSUE_NUMBER} clear description. For example if you are working on the issue 53 about registering user endpoint for a certain app, the title shoud be: **#53 User registration endpoint** This way it will be easy to find on the futurre.
- [Tie Issues to PR´s] Don´t forget to tie your issues to the PR you are working on.
 
## General Tricks.

-  I strongly suggest you use a complete IDE such as Intellij or similar.
-  Working on an old application full of comments? Erasing comment is just a requisite but you should not waste time on it, do a "Replace on your IDE" and search the following regular expression and replace with nothing
  `/\*([^*]|[\r\n]|(\*+([^*/]|[\r\n])))*\*+/`
Please always check what it does, it is a powerful tool but use with precaution.
-  Refactor to variables or methods is really easy when you work with intellij, you just have to right click over the variable and select refactor, then change the name and it will do it for you on all the places, [Watch the video](https://www.youtube.com/watch?v=_Fv7Bn9qwkI)

