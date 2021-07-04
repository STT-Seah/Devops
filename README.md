# Devops Project 2: CI/CD


## Github Actions CI/CD - Everything you need to know to get started



![image of Github Actions](https://avatars.githubusercontent.com/u/44036562?s=200&v=4)



In today's fast-paced environment, it's absolutely essential that we can automate the testing and delivery of our code.

That's where GitHub actions comes in.

It's the built-in, CICD tool for GitHub, if you're unfamiliar with what CICD is it stands for continuous integration and continuous delivery.

Essentially it allows us to automate the testing of our code to make sure it meets certain criteria after all the tests are passed you can enable actions to automate the delivery of your code.

This can significantly reduce the time it takes for you to deliver updates your application, which allows developers to focus more of their time on the code itself.



### What is GitHub Super Linter



![image of Github Super Linter](https://github.blog/wp-content/uploads/2020/06/github-super-linter-white.png?w=1200)



The Super Linter is a *source code repository* that is packaged into a Docker container and called by GitHub Actions.

This allows for any repository on GitHub.com to call the Super Linter and start utilizing its benefits.

The Super Linter will currently support a lot of languages and more coming in the future.



#### How it works



When you’ve set your repository to start running this action, any time you open a pull request, it will start linting the code case and return via the Status API.

It will let you know if any of your code changes passed successfully, or if any errors were detected, where they are, and what they are.

This then allows the developer to go back to their branch, fix any issues, and create a new push to the open pull request.

At that point, the Super Linter will run again and validate the updated code and repeat the process. You can configure your branch protection rules to make sure all code must pass before being able to merge as an additional measure.



**Videos to create Github Actions CI/CD Q2 Show & Tell**

- [Github Actions CI/CD - Everything you need to know to get started](https://www.youtube.com/watch?v=mFFXuXjVgkU)

**Instructions**

  1.Create new repository, click + new and name whatever you want

  2.Select public (if you want the public to view your project)
  
  3.Scroll down select add a README file, click create repository button
  
  4.Create a workflow, click add file button and select create new file, be very specified when comes to naming the file
  
  Type the proper directory in this format: .github/workflows/superlinter.yml(name whatever you want and copy and paste the code (from superlinter.yml) in the blank space to run
  
  Warning: if workflow is not triggering which means the format or spelling error to name the workflow file
  
  The code (from superlinter.yml) paste, its purpose is to listening for a push event, when the push event happen, it's going to check our code and than run superlinter against it to make sure it conforms to the linting standards.
  
  
  5.YAML
