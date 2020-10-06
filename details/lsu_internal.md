## Scalable Second Order Methods for High Performance Data Analytics

Although many machine learning (ML) tasks would at first glance appear
eminently parallelizable and scalable, effective acceleration of these tasks
with parallel hardware has proven to be elusive. Among other reasons, ML
problems can’t avail themselves of Gustafsson’s Law (weak scaling). Typical
scientific computing problems scale in size and gain better resolution, 
fidelity, reliability, etc – while also being able to weak scale. ML
problems, however, tend to be constrained in size by the particular tasks
they are applied to. One doesn’t get a better solution by doubling the size
of a deep neural net (DNN), for example. Moreover, while standard methods
for machine learning, e.g., stochastic gradient descent (SGD) for DNNs, tend
to be resource efficient, they are also highly sequential in nature, further
limiting opportunities for scalability. The increasing availability of
scalable computing platforms (including accelerators) presents an
opportunity for more sophisticated (and resource intensive) approaches to be
developed. The idea behind such approaches is to apply (for example)
second-order optimization approaches that, while potentially requiring more
memory and computation than a first-order approach, would enable
significantly faster time-to-solution while amortizing the resources across
a scalable computing platform.

The planned project will propose to create a scalable infrastructure for
future AI systems that utilizes all of the compute power of the existing
large scale HPC systems we have available today and will have in the future, 
and to reduce the time to solution for very large machine learning and
optimization problems to a fraction of the time required today. This
includes the development of new, second order optimization methods and
algorithms, and the design and development of scalable software frameworks
supporting the distributed execution of these algorithms. We envision a
system that combines the advantages of a high-productivity development
environment accessible to domain scientists with a high-performance
execution environment taking advantage of modern computing architectures and
infrastructures.

This project will to a large extent involve a sizable group of graduate
students from various departments (from math to computer science, from other
STEM departments) distributed across the participating universities that as
a team will work on all aspects of the project. The educational effect of
building such a large, multi-disciplinary team of young and enthusiastic
people will create the foundation for a successful outcome.  

As I understand, this is really a first abstract and we can (and probably
will) change every aspect of it. Please start thinking what the big story
could be and what you would like to contribute. Also please try to find
other people that could add valuable expertise to such a project (I also
have added David, Steve, and Rod here, please respond whether you would like
to be involved).

If you would like to add anything to the blurb above, I'll be still able to
change things by tonight. Please feel free to let me know.
