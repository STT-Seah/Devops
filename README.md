# Devops Project 2: CI/CD


## Welcome to Fintech Learners Pages For Non Tech


In today's fast-paced environment, it's absolutely essential that we can automate the testing and delivery of our code. 

That's where GitHub actions comes in. 

It's the built-in,  CICD tool for GitHub, if you're unfamiliar with what CICD is it stands for continuous integration and continuous delivery. 

Essentially it allows us to automate the testing of our code to make sure it meets certain criteria after all the tests are passed you can enable actions to automate the delivery of your code. 

This can significantly reduce the time it takes for you to deliver updates your application, which allows developers to focus more of their time on the code itself. 

In this video, I'm going to go over all the theory you need to know to understand the GitHub action workflow.

In the lab portion of this video will go over how to implement our own GitHub action and implements a linter that will run checks against our code, to make sure that it meets specific criteria. 

So to start us off, let's go over the terminology, you need to know to understand a GitHub actions workflow file. 

So we have a workflow Yaml file which specifies events jobs Runners steps and actions. 

So an event is a trigger for a workflow. 

A common event that occurs in a repository. 

It's when someone pushes new code, you can see that in this configuration file. 

We specify the workflow to trigger when someone pushes new code. 

When the event occurs, it's going to run all the jobs within the workflow. 

In this workflow we have a single job named Super lint, that specify multiple steps and actions. 

You can see underneath the steps. 

There's two actions that are being run. 

First, it's going to check out our code and then it's going to run the super linter against it up here. 

You can see the runs on parameter and this is where we specify our runner. 

Basically, this is a container environment that will run our code by default GitHub runs, this container for you, but you can host your own Runner if you would like to.

The default containers to choose from are Ubuntu Linux, Microsoft Windows and Mac OS. So to put it all together on the event that someone It pushes new code, it's going to run the job. Super lint that job is going to run on Ubuntu, container hosted on github.com, and then it's going to go through two steps. The first step is to check out the code and the next step is to run the linter. By the way, if you don't know what a linter is, it's just something that we use to check to make sure that our code is conforming to certain standards, super linter is made up of multiple linters, so it doesn't matter which code you use in your repository. Super lindtr is going to understand it and make sure you can conform to the standards of that language.

  
