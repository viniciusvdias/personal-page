+++
## About/Biography widget.

draft = false

widget = "about"

## Order that this section will appear in.
weight = 1

## List your academic interests.
[interests]
  title = "Research Interests"
  interests = [
    "Distributed Systems",
    "Operating Systems",
    "Computer Networks"
  ]

## List your qualifications (such as academic degrees).
[education]
  title = "Education"

[[education.courses]]
  course = "MSc in Computer Science"
  institution = "Federal University of Minas Gerais, Brazil"
  year = 2016

[[education.courses]]
  course = "BSc in Computer Science"
  institution = "Federal University of Uberlândia, Brazil"
  year = 2013
 
+++

### About Me

I am a master's student in the Computer Science Department (DCC) at
Federal University of Minas Gerais (UFMG), Brazil. Before that I received my B.Sc. in
Computer Science from Federal University of Uberlândia (UFU), Brazil.

Broadly, I am interested in research problems concerning systems'
performance, specially large-scale distributed systems. Recently, I have been
working on performance diagnosis and reconfiguration of data parallel
programming models (a.k.a. Big Data) and in particular, the following challenges
have been catching my attention (and stealing some of my sleep :P):

- **Task Model in Data-Parallel Frameworks:** Data-itensive frameworks
(e.g., [Spark](http://spark.apache.org/) and [Flink](https://flink.apache.org/))
are based on specific task models
that describe how resources (memory, CPU, disk, etc.) in parallel computations are consumed.
   -  Is there a more deterministic model that would make easy to identify which
resources are more important throughout tasks' execution?
   - Would this model facilitate resource overlapping among concurrent tasks?
   - Which would be the gains (if any) in doing that, considering modern operating
systems?


- **Multi-Resource Characterization in Parallel Programs:**
Parallel processing frameworks perform computation by statically requesting
multi-dimensional resource containers from cluster schedulers
(e.g.,
[YARN](https://hadoop.apache.org/docs/current/hadoop-yarn/hadoop-yarn-site/YARN.html) and
[Mesos](http://mesos.apache.org/)). Community experiences have shown that tuning these dimensions
appropriately taking into account each application individually can have great
impact in performance.
   - What would be the right set of application profiles that captures most of
     behaviors regarding multi-resource tuning in parallel applications?
   - How to use that knowledge to automate the process of resource requesting?
     Ideally I would not want these aspects to be transparent to the user.

- **Autonomic Computing:** As computational demands can greatly vary in a
  parallel execution due to faults, (over,under)subscription of resources,
  heterogeneous environments, and so on, modern distributed systems would
  leverage [autonomic computing characteristics and principles](https://en.wikipedia.org/wiki/Autonomic_computing).
  - How far are we from actually being capable of incorporating such concepts in
  large-scale distributed systems?
  - How feasible is to design and implement systems with autonomic computation
    as a requirement, rather than a feature?
