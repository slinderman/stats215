# Statistical Models in Biology

STATS215 	&middot; Winter 2020 &middot; Stanford University

## Course Description
This course is about probabilistic models in biology and the statistical inference algorithms necessary to fit them to data. We will cover some of the most important tools for modeling biological data, including latent variable models, hidden Markov models, dynamical systems, Poisson processes, and modern extensions of these models that use deep learning.  We will study algorithms for parameter estimation and inference, and we will apply these tools to a variety of problems across biology, with a particular emphasis on applications in neuroscience.  As part of the homework assignments, you will implement these models and algorithms in Python and apply them to real data.  

## Prerequisites
You should be comfortable with the basics of probability at the level of STAT116, including random variables, joint densities, conditional distributions, etc.  You should also be familiar with maximum likelihood estimation, for example from STAT200.  We will use basic linear algebra (solving linear systems and using eigendecompositions) and multivariable calculus (gradients, Jacobians, Hessians, etc.). 

## Logistics
 * Instructor: [Scott Linderman](http://slinderman.web.stanford.edu/)
 * Teaching Assistant: Kevin Han 
 * Lectures: Tuesday and Thursday, 12-1:20pm
 * Location: 540-108
 * Office Hours: TBD
 
# Tentative Schedule

| Lecture |  Date  | Topic | Suggested Readings |
| :------:|:------:|-------|--------------------|
| 1       | Jan 7  | Probability Review | Bishop (2006) Ch 2 <br> Murphy (2013) Ch 2|
| 2       | Jan 9  | Graphical Models, Learning, and Inference | Barber (2010) Ch 3 and 4|
| 3       | Jan 14 | Linear and Generalized Linear Models | Bishop (2006) Ch 3 and 4  <br> Murphy (2013) Ch 7-9 <br> |
| 4       | Jan 16 | Autoregressive Models <br> **<font color="red">HW1 Out</font>** | Pillow et al (2008) <br> Larochelle and Murray (2011) <br> van den Oord (2016a, 2016b) |
| 5       | Jan 21 | Latent Variable Models: Mixtures and Factors | | 
| 6       | Jan 23 | Expectation Maximization | | 
| 7       | Jan 28 | Models of Networks and Tensors | Williams et al (2017) |
| 8       | Jan 30 | Variational Inference and vEM <br> **<font color="red">HW1 Due &middot; HW2 Out</font>** | Blei et al (2017) |
| 9       | Feb 4  | Variational Autoencoders (VAE's) | Rezende et al (2014) <br> Kingma and Welling (2014) |
| &mdash; | Feb 6  | **<font color="red">Midterm Exam</font>** | |
| 10      | Feb 11 | Markov Chains | |
| 11      | Feb 13 | Hidden Markov Models <br> **<font color="red">HW2 Due &middot; HW3 Out</font>** | Wiltschko et al (2015) |
| 12      | Feb 18 | Linear Gaussian Dynamical Systems | Barber (2010) Ch 24 <br> Murphy (2013) Ch 18 <br> Macke et al (2013) |
| 13      | Feb 20 | Switching Linear Dynamical Systems <br> **<font color="red">Project Proposal Due</font>** | Barber (2010) Ch 25 <br>  Linderman et al (2017) |
| 14      | Feb 25 | Gaussian Processes | Rasmussen and Williams (2006) Ch 2 |
| 15      | Feb 27 | Poisson Processes <br> **<font color="red">HW3 Due &middot; HW4 Out</font>** | Kingman (1993) Ch 1 and 2|
| 16      | Mar 3  | Guest Lecture: Structured, Sequential VAE's | Johnson et al (2016) <br> Gao et al (2016) <br> Pandarinath et al (2017) |
| 17      | Mar 5  | Continuous Time Markov Chains | |
| 18      | Mar 10 | Hawkes and Cox Processes | Linderman and Adams (2014) <br> Kingman (1993) Ch 6 |
| 19      | Mar 12 | Kingman's Coalescent <br> **<font color="red">HW4 Due</font>** | Kingman (1982) <br> Norborg (2004) |
| &mdash; | Mar 20 | **<font color="red">Final Report Due</font>** | |

# References

