# Guidelines

This project represents the framework of how we love to work at Takumi software, it is intendended
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
- [Eat your dog´s food] Never ever deliver work if it is not tested, you will lose credit and time.
- [A video is worth 1000 images] Literally! If you have a problem with an application try recording it on video to show it to your teammates and ask for help after applying the **Google rule**, then send it over Slack or the team chat, also videos are a good way to explain or make evidence of behaviors. 
- The master branch MUST always be able to compile, this means that we need to protect the master branch by having pipelines. Protection comes from automation instead of mothod implementation.
- If there is a none clear syntax on the code either if it is coming from the framework or the mathod/variable naming either refactor the code to apply the German convention or use sugar syntax to make it clearer.


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

### Refactoring Insane Code Blocks
Always strive to simplify code! Here's a simple recipe to decrease code complexity:

- [ ] search for an `if`, `for`, `while` statement or a method that is just simply insanely huge
- [ ] cut it using your IDE csapabilities.
- [ ] paste it into a new private (private or protected always better, let it be exposed by the parent method where you cut the code block) method called `refactor()`
- [ ] look for variables needed as parameters - they'll scream red at you by your IDE
- [ ] create needed parameters and inject them to your `refactor()` method
- [ ] read code, search for a descriptive name for the code block and change the dummy name
- [ ] read the code searching for possible implementations of early returns, code removal, etc.
- [ ] repeat the process inside the recently create method.

This is a simple, but effective way of decreasing the [cyclomatic complexity](https://en.wikipedia.org/wiki/Cyclomatic_complexity) of the codebase.

## How to track your work.

In order to track your work either you are working on several projects for the organization or just one, you will find there are several url´s that can help you keep your eye on the work you are on.

- See all the issues assigned to you that are open, [issues assigned and open](https://github.com/issues?q=user%3Atakumi-software+is%3Aopen)
- See all the pull requests that open on the organization, [pull requests open](https://github.com/pulls?q=user%3Atakumi-software+is%3Aopen)
- Simply get all the notifications, [Github Notifications](https://github.com/notifications)
      
