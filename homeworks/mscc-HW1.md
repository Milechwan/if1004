###Homework 1###

- _Concepts_
    - _In your own words, explain the difference between continuous integration, continuous delivery, and continuous deployment._
    Answer: Continuous deployment is about automatically testing incremental software integrated with the existing and stable system (regression test). Additionally, it involves frequent deployment in production environments. This makes possible to changes reach customers and clients quickly, in days or even hours.

    Continuous integration is about to make sure the new features are working by their own (unit test), before integrating with the other features, and working with the new parts (integration testing). CI requires code integration into a shared repository, and use of tools that will automatically build and run tests in that repository, guaranting easiness to find bugs and warn the team to correct them as quick as possible.

    Continuous delivery can be considered as an extesion of CI, where each team ensures that every change to the system is releasable, and the release of a new version can be done by pushing a button. CD also involves frequent delivery and get users feedback quickly, being aware of necessary changes, including bug correction or even business/strategy changes.

    - _How does DevOps team model (e.g., site reliability engineer) differ than a NoOps team model (e.g. Netflix team)? What differences in architecture allow for a NoOps model?_
    Answer: Different from DevOps team model, NoOps team model has partial responsability in every task (develop, test, deploy, maintainance). That means that the team is concerned and able to work on every step mentioned, not existing a specific and clear operation team.

    - _Explain the principle of Every Feature is an Expertiment_
    Answer: It's about collecting data (relevant information) and defining metrics to analyze and identify if a feature should be deleted or if it's worth to keep it in the system.

    - _Explain the principle of Be Fast to Deploy, Slow(er) to Release._
    Answer: It's about deploying frequently in production environment and not affect the user experience directly while it is, for example, disabled in the user interface, using strategies such as dark launches. This makes possible to the engineer test and evaluate the new feature "little by little", making sure that it is stable, and then release and enable it to the user interface. 
