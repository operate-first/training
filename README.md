# Operate First Training

This repository is the content source for training in the Operate First community. We develop training content here and publish training courses to FIXME-TBD.

## What do we mean "training content"?

**Training content** is:

* Content used for generating self-paced training on topics important to the Operate First community and to the site reliability engineer (SRE) career path.

* Designed to apply [instructional design best practices](https://blog.commlabindia.com/elearning-design/instructional-design-best-practices-guide) and [Adult Learning Theory (andragogy)](https://en.wikipedia.org/wiki/Andragogy).

* Developed and maintained in markdown files, Jupyter Notebooks, and Jupyter Books.

* Organized into courses, but set up as modular topics that can be reused across courses.

Training content ***is not***:

* Documentation. Guides, references, and other documentation resources are maintained as part of the Operate First Knowledge Hub (FIXME-TBD, maybe docs.operate-first.cloud).

* Comprehensive. Training content is created and added to Operate First as the community members are able to do so. The community can prioritize certain kinds of training depending on its current community goals.

## How does this content become training?

On commit, CI/CD identifies what's been updated in the repository and identifies the training courses and workbooks that need to be built or rebuilt into a target format (typically HTML). If a content build is successful, CI/CD will go on to publish that content to the configured target location operate-first.cloud.

## Where will learners find the content?

Operate First has a training landing page available at (FIXME-TBD training.operate-first.com?). Learners should not need to access this developer-side repository to access or complete their training.

## Repository structure and CI/CD

Repository contents are organized to reflect how the courses are organized at (FIXME-TBD training.operate-first.com?).

General directory structure:

**programs** - A program here represents a training program hosted within the Operate First space. A program brings courses together in an ordered learning path. File format under this directory TBD (probably Jupyter Book).

**courses** - A course here represents a small unit of training covering 1-2 learning objectives that are important to the community. A learning objective is what someone should be able to do after training that they may not have been able to do before training (e.g. "On completing this course, you should be able to..."). This directory has subdirectories organizing courses by skill areas as follows:

* **skills-operatefirst** - Operate First overviews, onboarding, and tools
* **skills-opensource** - Open source
* **skills-software** - Software development
* **skills-cloud** - Cloud technology and operations
* **skills-team** - Working on teams (e.g. agile, communication, handling feedback)

## How to contribute training content

FIXME-TBD


<hr/>

### License

This repository was created compliant with [ADR 0001](https://www.operate-first.cloud/blueprints/blueprint/docs/adr/0001-use-gpl3-as-license.md). All content within this repository is provided under the [GNU General Public License v3.0 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).

<hr/>
