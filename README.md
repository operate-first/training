# Operate First *training* repo

This repository is the content source for training in the Operate First community. We develop training content here and publish training modules to operate-first.cloud.

## What we mean by "training content"

Training content is any **one-time interactive experience** designed to train people on how to perform some action or improve their performance in that action.

Training is developed around **learning objectives**. A learning objective is an *observable, measureable behavior* that you want someone to be able to perform. Learning objectives start with this leading statement:

```
After completing this training, you should be able to...
```

***Training provides the best experience when it is:***

* Short: a learner who is new to the information should be able to complete it in 5 to 15 minutes.

* Modular: it covers only a few learning objectives at a time (typically 1-3).

* Applies [instructional design best practices](https://blog.commlabindia.com/elearning-design/instructional-design-best-practices-guide) and [Adult Learning Theory (andragogy)](https://en.wikipedia.org/wiki/Andragogy).

* Refers to **separate** documentation resources for ongoing reference.

## How we build training

For Operate First, we divide training up into **courses**.

Each course:
* Is self-contained within a directory
* Is developed as a single book in Jupyter Book
* Covers 1-2 learning objectives

The course has associated GitHub workflow that builds the book and publishes the HTML to a directory under ``operate-first.cloud/training/``. We can run those workflows from GitHub after accepting a PR into the *operate-frst/training* repository.

## Where people can find and consume the training content

FIXME... this landing page setup is in progress as of 9 May 2022...

You have two options to access training content after it's been published:
* Directly open https://operate-first.cloud/training
* Go to the Operate First home page (operate-first.cloud) and select "Docs and training"

*Learners (end users) should not need to access this repository directly unless they choose to contribute back to the training content.*

## Repository organization

These are the key directories and files to pay attention to when contributing to training:

**courses** - The directory containing all individual training modules with each directory starting with the string "courses-".

*courses/index.html* - A markdown file used to index all available training modules. You'll add a line to this to link to any new courses once you're ready for that course to be published.

**template-course** - A directory with a pre-configured Jupyter Book that you can copy to create a new training course.

**.github/workflows** - A directory with the YAML files needed to build each course. Add YAML here for a course when that course is ready for publishing to the website, before opening the PR for upstream.

## How to contribute training content

If you aren't yet a member of the Operate First community in GitHub, [start here](https://github.com/operate-first/common/blob/main/docs/add_gh_member_and_access.md#become-a-github-member).

Members can then create forks and use the pull request (PR) system to contribute changes to the repository. The sections that follow cover what to do.

### Create and check out your fork

1. Fork the training repository in GitHub: **[operate-first/training|https://github.com/operate-first/training]**
2. In your fork, create a working branch other than main.
3. If you want to work locally on your system, clone your fork and check out your working branch.

### Set up a new course (new courses only)

If you're creating a new training course:

1. Copy the *template-course* directory to create a new directory under *courses* following the same directory naming convention as other courses (*course-title_of_course*).
2. In your new copy, add your title and other information in _config.yaml.

### Develop training locally

If you're working locally, you can use various tools to develop your code (markdown, Jupyter Book, etc.) and to preview your Jupyter Book. Here are some options:

* Use your preferred code editor to create and edit markdown files (e.g. Atom).

* Use Jupyter Notebook locally to open the Jupyter Book contents and create and modify files (especially if you want to create Jupyter Notebook files).

* Run Jupyter Book commands to test changes before committing them to your branch.

See the [Resources](#Resources) section if you're new to either Jupyter Book or Jupyter Notebook.

### Apply the usual coding best practices

Apply GitHub and developer best practices while developing training. For example, commit early and often, and push changes to your fork at a regular cadance (e.g. daily) to mitigate losing your changes.

### Prepare to publish a new course (new courses only)

If you're created a new training course *and* you're ready to publish it to Operate First, make these final changes in your branch before merging to main and opening your PR:

1. Make a copy of one of the existing YAML files under .github/workflows/ and modify it appropriately there in that same directory. Follow a similar pattern to other courses, such as dropping the "course-" prefix on the directory name when publishing.
2. (FIXME... this part of the process is not yet complete) Edit *courses/index.md* to add a link to the URI where your training is being published.

### Open a pull request

Initiate a pull request in accordance with Operate First's current process. If you are part of the approvers, you will be able to approve the PR upstream and merge changes.

### Run the GitHub workflows corresponding to your changes

After your PR is approved and the changes are merged, open the "Actions" tab in the operate-first/training space in GitHub ([here's the direct link](https://github.com/operate-first/training/actions)), and use that UI to run the workflows listed there.

## Resources

Here are some resources if you are new to either Jupyter Notebook or Jupyter Book:

* [Getting Started with Jupyter Notebook](https://docs.jupyter.org/en/latest/start/index.html)

* [Jupyter Book Tutorial](https://jupyterbook.org/en/stable/start/your-first-book.html)

<hr/>

### License

This repository was created compliant with [ADR 0001](https://www.operate-first.cloud/blueprints/blueprint/docs/adr/0001-use-gpl3-as-license.md). All content within this repository is provided under the [GNU General Public License v3.0 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).

<hr/>
