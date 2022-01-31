# Operate First Training

This repository is the content source for training in the Operate First community. We develop training content here and publish training modules to operate-first.cloud (FIXME-URL).

## What do we mean "training content"?

**Training content** is:

* Content used for generating self-paced training on topics important to the Operate First community and to the site reliability engineer (SRE) career path.

* Designed to apply [instructional design best practices](https://blog.commlabindia.com/elearning-design/instructional-design-best-practices-guide) and [Adult Learning Theory (andragogy)](https://en.wikipedia.org/wiki/Andragogy).

* Developed and maintained in **modules**, which each module representing a learning objective ("After this module, you should be able to...").

* Designed to assemble into larger chunks to create training courses, workbooks, or programs.

Training content ***is not***:

* Documentation. Guides, references, and other documentation resources are maintained as part of the Operate First Knowledge Hub (FIXME-TBD, maybe docs.operate-first.cloud).

* Comprehensive. Training content is created and added to Operate First as the community members are able to do so. The community can prioritize certain kinds of training depending on its current community goals.

## How the training is encoded and built

Each modules consists of one or more markdown files or Jupyter Notebooks connected within a single Jupyter Book.

On commit, CI/CD identifies what's been updated in the repository and identifies the training modules that need to be built or rebuilt into a target format (typically HTML).

If a content build is successful, CI/CD will go on to publish that content to the configured target location operate-first.cloud.

## Where will learners find the content?

Operate First has a training landing page available at (FIXME-TBD training.operate-first.com?). Learners should not need to access this developer-side repository to access or complete their training.

## Repository organization

Repository contents are organized to reflect how content is organized at (FIXME-TBD training.operate-first.com?).

General directory structure:

**modules** - The directory containing all individual training units (modules), organized into subdirectories based on these skill areas:

* **skills-operatefirst** - Operate First overviews, onboarding, and tools
* **skills-opensource** - Open source
* **skills-software** - Software development
* **skills-cloud** - Cloud technology and operations
* **skills-professional** - General professional job skills for team environments (e.g. agile, communication, handling feedback)

**courses** - A directory for Jupyter Books used to assemble two or more training modules into a single, larger unit. (FIXME - experimental)

![training repository structure diagram](repo_layout.png "training repository structure diagram")

## How to contribute training content

FIXME-TBD


<hr/>

### License

This repository was created compliant with [ADR 0001](https://www.operate-first.cloud/blueprints/blueprint/docs/adr/0001-use-gpl3-as-license.md). All content within this repository is provided under the [GNU General Public License v3.0 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).

<hr/>
