#### Homework 4 ####

1. Continuous deployment x continuous delivery
    1. _Main issues:_ 
    2. _Benefits:_
        - Continuous deployment:  Since it is considered the next step of continuous delivery, if in your company the application acceptance tests step to the last step are automated and the tests before the UAT one are also automated, the application is deployed automatically to production. That means there's no need of "human intervention" or IT limitations, so the continuous deployment is possible to apply.
        - Continuous delivery: The guarantee of a safe and fast code deployment, since it is almost all about rigorous automated tests, delivering every change to a production-like environment. 
    3. _Differences:_ The continuous deployment cannot be possible if there are some requirements, agreements, IT limitations or even the need to wait for another feature to go live first. Additionally, it cannot happen if there's no continuous delivery. In other words, if the steps before the UAT step are not automated, then it isn't possible to have either continuous delivery nor continuous deployment. And if just the steps mentioned above are triggered automatically and the UAT is not, then you have just continuous delivery. 

2. Branch vs trunk-based approaches
    - _Advantages:_ Trunk-based approaches are great in a scenario like Google's, meaning that it's worth it because there's a tool that automatically checks if a developer submit/commit something that would negativelly affect a core feature/dependency for other services, even if they are not directly correlated. Additionally, it saves time to resolve conflicts (comparing to branch-based approach), and justifies if a change should be included/released or not, based on computational costs.

        Branch-based approaches allow developers to change the same file if necessary so it can save time to develop a feature, and it helps a lot in Agile development. A branch for each developer, for example, is a scenario that can be possible in small teams ("two pizzas team") and the tasks being developed by each one of them can also save time to review, test, etc, since the core dependencies and features should be in master branch, and every developer is responsible to get the latest version of this branch to keep coding their tasks. Also, tagging the master branch so the DevOps tools are aware of the new version is a form of ensuring the changes to be delivered and deployed are approved. 

    - _Disadvantages:_ To make possible a trunk-based approach, it's necessary to have a regulatory that ensures code review and "owner files" to make sure that uncorrect commits will not be accepted. Even with the use of a software tool to calculate and advice if a change is wrong or worths the effort along with the code review made by developers, an uncorrect commit can be submitted, since there's no official way to prevent this.

        Branch-based approach's main disadvantage is merging the conflicts. It can take a few minutes or even days to be resolved if the team is not well aligned enough with their responsabilities and/or tasks. The time theoretically saved with the spread of tasks is spent resolving merge conflicts.

3. Heavily baked and lightly baked images
    - Heavily baked images: If the service doesn't need to be highly scalable or to constantly update all the dependencies like libraries or third-party software, tools, etc., then a heavily baked image should be adequate. Small companies or companies that don't use or need cloud provisioning are some examples of who would prefer heavily baked images. 
    - Lightly baked images: If your service is using cloud provisioning, needing autoscaling and high availability and maintain all the dependent software (or even SO) updated as soon as possible, then a lightly baked image is more suitable than a heavily baked one. 