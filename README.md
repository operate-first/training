# Operate First *training* repo

This repository is the content source for training in the Operate First community. We develop training content here and publish training modules to operate-first.cloud.

## What do we mean "training content"?

Training content is any **one-time interactive experience** designed to train people on how to perform some action or improve performance on that action.

Training is developed around **learning objectives**. A learning objective is an observable, measureable behavior that you want someone to be able to perform. We typically write learning objectives with this leading statement: "After completing this training, you should be able to..."

Training should be designed to:

* Be short and modular, presenting only 1 or 2 learning objectives.

* Apply [instructional design best practices](https://blog.commlabindia.com/elearning-design/instructional-design-best-practices-guide) and [Adult Learning Theory (andragogy)](https://en.wikipedia.org/wiki/Andragogy).

* Refer to **separate** documentation resources for ongoing reference.

## How do we build training?

For Operate First, we divide training up into **courses**.

Each course:
* Is self-contained within a directory
* Is developed as a single book in Jupyter Book
* Covers 1-2 learning objectives

Automation associated with the repository builds each book into a training course and publishes it to a directory under operate-first.cloud/training/. That automation triggers when we accept a PR in the upstream repository (operate-first/training).

## Where can people find and take the training content?

You have two options to access training content after it's been published:
* Directly open https://operate-first.cloud/training
* Go to the Operate First home page (operate-first.cloud) and select "Docs and training"

Learners (end users) should not need to access this repository directly unless they choose to contribute back to the training content.

## Repository organization

These are the key files to pay attention to when contributing to training:

**courses** - The directory containing all individual training modules with each directory starting with the string "courses-".

*courses/index.html* - A markdown file used to index all available training modules. You'll add a line to this to link to any new courses once you're ready for that course to be published.

**template-course** - A directory with a pre-configured Jupyter Book that you can copy to create a new training course.

## How to contribute training content

If you aren't yet a member of the Operate First community in GitHub, [start here](https://github.com/operate-first/common/blob/main/docs/add_gh_member_and_access.md#become-a-github-member).

Members can then fork and contribute changes to the repository:
1. Fork the training repository in GitHub: **[operate-first/training|https://github.com/operate-first/training]**
2. In your fork, create a working branch other than main.
3. If you want to work locally on your system, clone your fork and check out your working branch.
4. If you're creating a new training module, copy the *template-course* directory to create a new directory under *courses/* following the same directory naming convention as other courses (*course-title_of_course*).
5. In your new copy, add your title and other information in _config.yaml.
6. If you're working locally, you could use Jupyter Notebook locally to open the Jupyter Book contents and create and modify files. You can also run Jupyter Book commands to test changes before committing them to your branch. If you're not working locally, you may be able to use [Meteor](https://shower.meteor.zone/) to test (we haven't tried this, though).
7. When you have finished a series of changes, merge your working branch into your main branch and push changes to your fork in GitHub.
8. When you're ready to get your changes added upstream, initiate a pull request in accordance with Operate First's current process.

Here are some resources if you are new to either Jupyter Notebook or Jupyter Book:
* [Getting Started with Jupyter Notebook](https://docs.jupyter.org/en/latest/start/index.html)
* [Jupyter Book Tutorial](https://jupyterbook.org/en/stable/start/your-first-book.html)

<hr/>

### License

This repository was created compliant with [ADR 0001](https://www.operate-first.cloud/blueprints/blueprint/docs/adr/0001-use-gpl3-as-license.md). All content within this repository is provided under the [GNU General Public License v3.0 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).

<hr/>
