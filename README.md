# Operate First *training* repo

This repository is the content source for training in the Operate First community. We develop training content here and publish training modules to operate-first.cloud.

## What do we mean "training content"?

Training content is a one-time interactive experience designed to train people on how to perform some action or improve performance on that action.

Training should be designed to:

* Be small and modular, presenting only 1 or 2 learning objectives (e.g. "After completing this training, you should be able to [OBJECTIVE]...").

* Apply [instructional design best practices](https://blog.commlabindia.com/elearning-design/instructional-design-best-practices-guide) and [Adult Learning Theory (andragogy)](https://en.wikipedia.org/wiki/Andragogy).

**Training content *is not* a substitute for documentation!** Docs should be comprehensive resources designed for repeated reference and are easier to keep up-to-date over time. A one-time training experience may be used to introduce or enable someone to a topic while directing learners to docs for ongoing reference.

## How do we build training?

Training is divided up into **courses**.

Each course:
* Is self-contained within a directory.
* Is developed using Jupyter Book.
* Covers 1-2 learning objectives (e.g. *"After completing this training, you should be able to..."*).

After setting up a course and having an acccepted pull request (PR) upstream, automation should build your course and publish it to operate-first.cloud. You can continue to maintain the course in the same way, ending with a PR each time you're ready to push a change upstream.

## Where can people find and take the training content?

Browse to operate-first.cloud and select "Docs and training" to access an index of all documentation and training together. (Learners should not need to access this developer-side repository unless they choose to contribute to training.)

## Repository organization

Repository contents are organized to reflect how content is organized at (FIXME-TBD training.operate-first.com?).

General directory structure:

*index.md* - A markdown file used to index all available training modules.

**template-course** - A directory with a pre-configured Jupyter Book that you can copy to create a new training course.

**courses** - The directory containing all individual training modules with each directory starting with the string "courses-".

## How to contribute training content

If you aren't yet a member of the Operate First community in GitHub, [start here](https://github.com/operate-first/common/blob/main/docs/add_gh_member_and_access.md#become-a-github-member).

Members can then fork and contribute changes to the repository:
1. Fork this training repository.
2. Check out your fork.
3. If you're creating a new training module, copy the *template-course* directory to create a new directory under *courses/* (following the same directory naming convention).
4. In your new copy, add your title and other information in _config.yaml.
5. Use Jupyter Notebook locally to open the Jupyter Book contents and create and modify files. Follow any guided information in the template. If you're new to Jupyter Book, visit [jupyterbook.org](https://jupyterbook.org/intro.html) for a tutorial and docs so you know how to add pages and test your build locally.
6. Continue working in your fork until you're ready to publish changes, then initiate a pull request in accordance with Operate First's current process.

<hr/>

### License

This repository was created compliant with [ADR 0001](https://www.operate-first.cloud/blueprints/blueprint/docs/adr/0001-use-gpl3-as-license.md). All content within this repository is provided under the [GNU General Public License v3.0 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).

<hr/>
