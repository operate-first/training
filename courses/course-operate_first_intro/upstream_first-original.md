<!-- #region -->
# Upstream First


### What is an upstream?

- Within information technology, the term upstream (and related term "downstream") refers to the flow of data. 


- An upstream in open source is the source repository and project where contributions happen and releases are made. The contributions flow from upstream to downstream.


- When talking about an upstream, it's usually the precursor to other projects and products. 


- One of the best-known examples is the Linux kernel, which is an upstream project for many Linux distributions. 


- Distributors like Red Hat take the unmodified (often referred to as "vanilla") kernel source and then add patches, add an opinionated configuration, and build the kernel with the options they want to offer their users.


- In some cases, a project or product might have more than one upstream. Red Hat Enterprise Linux (RHEL) releases are based on Fedora Linux releases. 


- The Fedora Project, in turn, pulls from many upstream projects to create Fedora Linux, like the Linux kernel, GNOME, systemd, Podman, various GNU utilities and projects, the Wayland and X.org display servers, and many more.


### Why are upstreams important?

- Upstreams are important because that's where the source contribution comes from. 


- Each upstream is unique, but generally the upstream is where decisions are made, the contribution happens, and where the community for a project comes together to collaborate for the benefit of all parties. 


- Work done at the upstream might flow out to many other open source projects.


- The upstream is the focal point where collaborators do the work. It's far better if all the contributors work together rather than, say, contributors from different companies working on features behind closed doors and then trying to integrate them later. 


- The upstream is also a fixed place where (if we’re talking about creating code) developers can report bugs and security vulnerabilities. If a bug or security flaw is fixed upstream, then every project or product based on the upstream can benefit from that work. 


### Upstream first

- Because the upstreams are so important, Red Hat has a longstanding practice of doing work upstream first and trying to get features and patches accepted upstream rather than just building them directly in our own products. The reasons for this are as follows:  
    - First, it's just good open source citizenship to do the work side-by-side with the rest of the community and share our work with the communities from which we're benefitting. 

    - Secondly, it's a better choice pragmatically to do the work upstream first. Sometimes it can be faster to implement a feature in a downstream project or product--especially if there are competing ideas about the direction of a project--but it's usually more work in the long run to carry those patches back to the project. By the time it's been shipped in a downstream, there's a good chance that the upstream code has changed, making it harder to integrate patches developed against an older version of the project.

    - By working upstream first, you have the opportunity to vet ideas with the larger community and work together to build new features, releases, content, etc. The features or changes you want to make may have an impact on other parts of the project. It's good to find these things out early and give the rest of the community an opportunity to weigh in.


- If the features or patches aren't accepted upstream for some reason, then a vendor can carry those separately. That's one of the benefits of open source, you can modify and distribute your own version (within the terms of the license, of course) that meets your needs. 
<!-- #endregion -->
