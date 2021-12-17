# Operate First Training

This repository is the content source for training content in the Operate First community hosted at FIXME.

## What do we mean "training content"?

**Training content** is:

* Content used for generating self-paced training on topics important to the Operate First community and to the site reliability engineer (SRE) career path.

* Designed to apply [instructional design best practices](https://blog.commlabindia.com/elearning-design/instructional-design-best-practices-guide) and [Adult Learning Theory (andragogy)](https://en.wikipedia.org/wiki/Andragogy).

* Developed and maintained in markdown files, Jupyter Notebooks, and Jupyter Books.

* Organized into courses, but set up as modular topics that can be reused across courses.

Training content ***is not***:

* Documentation. Guides, references, and other documentation resources are maintained as part of the Operate First Knowledge Hub:<br/>
FIXME... need a subdomain (docs.operate-first.cloud) or path (operate-first.cloud/docs/) where we can place guides and references for ongoing reference after training; training will link out to those references as needed

* Comprehensive. Training content is created and added to Operate First as the community members are able to do so. The community can prioritize certain kinds of training depending on its current community goals.

## How does this content become training?

On commit, CI/CD identifies what's been updated in the repository and identifies the training courses and workbooks that need to be built or rebuilt into a target format (typically HTML). If the content build is successful, CI/CD will go on to publish that content at operate-first.cloud.

## Where will learners find the content?

Operate First has a training landing page available here:<br/>
FIXME... need a subdomain (training.operate-first.cloud) or path (operate-first.cloud/training/) where we can place a training landing page.

The organization of training courses and workbooks at that location reflects how the training content is organized here in the repository.

## How to contribute training content

FIXME... need to explain


<hr/>

### License

This repository was created compliant with [ADR 0001](https://www.operate-first.cloud/blueprints/blueprint/docs/adr/0001-use-gpl3-as-license.md). All content within this repository is provided under the [GNU General Public License v3.0 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).

<hr/>
