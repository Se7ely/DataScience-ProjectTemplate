## Structure Expaination
- data: A folder that should contain all data files
    - external: Sub-folder for data from external sources 
    - interem: Sub-folder for data that has undergone interemediate but not full processing
    - processed: Sub-folder for data that has undergone full processing and ready to be used
    - raw: Sub-folder for raw data generating or gathered internally
- docs: A folder containing documentation files
    - data: Sub-folder for data documentation
        - data_definition.md: A file provding an overview of all the data included in the project (example included)
        - data_report.md: A file specific for a single dataset provding statistics about the data and variables in it, a seperate file should be included for each dataset in the project (example included)
    - models: Sub-folder for model documentation
        - v#.#
            - model_report.md: A file specific to a certain model defining the algorithm used, data used, features, and performance (example included)
    - project: Sub-folder for project documentation
        - charter​.​md: A file that should be compiled before starting the project to define business goals, evaluations metrics, etc. (example included)
        - exit_report.md: A file that should be compiled at the end of the project containing different findings, perfermance, technical details, etc. (example included)
- models: A folder that should contain all saved model files
    - v#.#
- notebooks: A folder containing notebooks for experiments, presentations, visualizations, etc. (but not final code)
- src: A folder containing the main source code of the preoject
    - data: Sub-folder for all data-related code
    - features: Sub-folder for all features-related code
    - model: Sub-folder for main model processes: definition, training, inference
        - architecture: Sub-folder for files defining model(s) architecture
        - training: Sub-folder for training scripts/notebooks
        - inference: Subfolder for inference scripts/notebooks
    - utils: Sub-folder for general utils commonly used in different files
- .gitignore
- README.​md
- requirements.yml: A file containing project dependencies to be exported using conda, not written manually (example provdided)
- setup.​py: A file containing the setup template needed for packaging the project (optional)

## DVC Setup Instructions:
- Follow: https://dvc.org/doc/install/linux
- Follow: https://dvc.org/doc/start
- Install gcloud or storage to be used
- Enter:  ```gcloud auth application-default login``` or equivalent
- Enter verification code after followinig the link using an @aim email
- Enter: dvc remote add -d origin_name link.to.bucket
- To upload data/models:
    - dvc add filename
    - dvc push
- To download data/models:
    - dvc pull


# README.​md Template
# Project Title

<!-- Add buttons here -->

![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/navendu-pottekkat/awesome-readme?include_prereleases)
![GitHub last commit](https://img.shields.io/github/last-commit/navendu-pottekkat/awesome-readme)
![GitHub issues](https://img.shields.io/github/issues-raw/navendu-pottekkat/awesome-readme)
![GitHub pull requests](https://img.shields.io/github/issues-pr/navendu-pottekkat/awesome-readme)
![GitHub](https://img.shields.io/github/license/navendu-pottekkat/awesome-readme)

<!-- Describe your project in brief -->

The project title should be self-explanatory and try not to make it a mouthful. (Although exceptions exist- **awesome-readme-writing-guide-for-open-source-projects** - would have been a cool name)

Add a cover/banner image for your README. **Why?** Because it easily **grabs people's attention** and it **looks cool**(*duh!obviously!*).

Wait, I forgot something. You can use this README as a template from [this link](README-template.md).

The best dimensions for the banner is **1280x650px**. You could also use this for social preview of your repo.

I personally use [**Canva**](https://www.canva.com/) for creating the banner images. All the basic stuff is **free**(*you won't need the pro version in most cases*).

*What are all those flashy thingies below the title?*

Looks nice doesn't it? Those are called badges and they do improve the readability by giving some quick insights right?

There are endless badges that you could use in your projects. And they do depend on the project. Some of the ones that I commonly use in every projects are given below. 

I use [**Shields IO**](https://shields.io/) for making badges. It is a simple and easy to use tool that you can use for almost all your badge cravings.

<!-- Add badges with link to Shields IO -->

![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/navendu-pottekkat/awesome-readme?include_prereleases)
: This badge shows the version of the current release.

![GitHub last commit](https://img.shields.io/github/last-commit/navendu-pottekkat/awesome-readme)
: I think it is self-explanatory. This gives people an idea about how the project is being maintained.

![GitHub issues](https://img.shields.io/github/issues-raw/navendu-pottekkat/awesome-readme)
: This is a dynamic badge from [**Shields IO**](https://shields.io/) that tracks issues in your project and gets updated automatically. It gives the user an idea about the issues and they can just click the badge to view the issues.

![GitHub pull requests](https://img.shields.io/github/issues-pr/navendu-pottekkat/awesome-readme)
: This is also a dynamic badge that tracks pull requests. This notifies the maintainers of the project when a new pull request comes.

![GitHub All Releases](https://img.shields.io/github/downloads/navendu-pottekkat/awesome-readme/total): If you are not like me and your project gets a lot of downloads(*I envy you*) then you should have a badge that shows the number of downloads! This lets others know how **Awesome** your project is and is worth contributing to.

![GitHub](https://img.shields.io/github/license/navendu-pottekkat/awesome-readme)
: This shows what kind of open-source license your project uses. This is good idea as it lets people know how they can use your project for themselves.

![Tweet](https://img.shields.io/twitter/url?style=flat-square&logo=twitter&url=https%3A%2F%2Fnavendu.me%2Fnsfw-filter%2Findex.html): This is not essential but it is a cool way to let others know about your project! Clicking this button automatically opens twitter and writes a tweet about your project and link to it. All the user has to do is to click tweet. Isn't that neat?

# Demo-Preview
<!-- Add a demo for your project -->

After you have written about your project, it is a good idea to have a demo/preview(**video/gif/screenshots** are good options) of your project so that people can know what to expect in your project. You could also add the demo in the previous section with the product description.

Here is a random GIF as a placeholder.

![Random GIF](https://media.giphy.com/media/ZVik7pBtu9dNS/giphy.gif)

# Table of contents

After you have introduced your project, it is a good idea to add a **Table of contents** or **TOC** as **cool** people say it. This would make it easier for people to navigate through your README and find exactly what they are looking for.

Here is a sample TOC(*wow! such cool!*) that is actually the TOC for this README.

- [Project Title](#project-title)
- [Demo-Preview](#demo-preview)
- [Table of contents](#table-of-contents)
- [Installation](#installation)
- [Usage](#usage)
- [Development](#development)
- [Contribute](#contribute)
    - [Adding new features or fixing bugs](#adding-new-features-or-fixing-bugs)
- [Footer](#footer)

# Installation
[(Back to top)](#table-of-contents)

*You might have noticed the **Back to top** button(if not, please notice, it's right there!). This is a good idea because it makes your README **easy to navigate.*** 

The first one should be how to install(how to generally use your project or set-up for editing in their machine).

This should give the users a concrete idea with instructions on how they can use your project repo with all the steps.

Following this steps, **they should be able to run this in their device.**

A method I use is after completing the README, I go through the instructions from scratch and check if it is working.

Here is a sample instruction:

To use this project, first clone the repo on your device using the command below:

```git init```

```git clone https://github.com/navendu-pottekkat/nsfw-filter.git```

# Usage
[(Back to top)](#table-of-contents)

This is optional and it is used to give the user info on how to use the project after installation. This could be added in the Installation section also.

# Development
[(Back to top)](#table-of-contents)

This is the place where you give instructions to developers on how to modify the code.

You could give **instructions in depth** of **how the code works** and how everything is put together.

You could also give specific instructions to how they can setup their development environment.

Ideally, you should keep the README simple. If you need to add more complex explanations, use a wiki. Check out [this wiki](https://github.com/navendu-pottekkat/nsfw-filter/wiki) for inspiration.

# Contribute
[(Back to top)](#table-of-contents)

This is where you can let people know how they can **contribute** to your project. Some of the ways are given below.

Also this shows how you can add subsections within a section.


### Adding new features or fixing bugs
[(Back to top)](#table-of-contents)

This is to give people an idea how they can raise issues or feature requests in your projects. 

You could also give guidelines for submitting and issue or a pull request to your project.

Personally and by standard, you should use a [issue template](https://github.com/navendu-pottekkat/nsfw-filter/blob/master/ISSUE_TEMPLATE.md) and a [pull request template](https://github.com/navendu-pottekkat/nsfw-filter/blob/master/PULL_REQ_TEMPLATE.md)(click for examples) so that when a user opens a new issue they could easily format it as per your project guidelines.

You could also add contact details for people to get in touch with you regarding your project.

# Footer
[(Back to top)](#table-of-contents)

Let's also add a footer because I love footers and also you **can** use this to convey important info.

Let's make it an image because by now you have realised that multimedia in images == cool(*please notice the subtle programming joke).

So that is it... You have completed your training young grasshopper. Now it is time for you to use this ideas for your projects.

Don't forget your **README Sensei**(*cool twitter handle idea*) when your project takes off with your **Awesome README**.

Leave a star in GitHub, give a clap in Medium and share this guide if you found this helpful.

**Now folks, the moment you've all been waiting for! The footer!**
***[Audible gasp]***

<!-- Add the footer here -->

![Footer](https://github.com/navendu-pottekkat/awesome-readme/blob/master/fooooooter.png)