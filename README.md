# Statistical Models in Biology

STATS215 	&middot; Winter 2020 &middot; Stanford University

## Course Description
This course is about probabilistic models in biology and the statistical inference algorithms necessary to fit them to data. We will cover some of the most important tools for modeling biological data, including latent variable models, hidden Markov models, dynamical systems, Poisson processes, and modern extensions of these models that use deep learning.  We will study algorithms for parameter estimation and inference, and we will apply these tools to a variety of problems across biology, with a particular emphasis on applications in neuroscience.  As part of the homework assignments, you will implement these models and algorithms in Python and apply them to real data.  

## Prerequisites
You should be comfortable with the basics of probability at the level of STAT116, including random variables, joint densities, conditional distributions, etc.  You should also be familiar with maximum likelihood estimation, for example from STAT200.  We will use basic linear algebra (solving linear systems and using eigendecompositions) and multivariable calculus (gradients, Jacobians, Hessians, etc.). 

## Logistics
 * Instructor: [Scott Linderman](http://slinderman.web.stanford.edu/)
 * Teaching Assistant: [Kevin Han](mailto:kevinwh@stanford.edu)
 * Lectures: Tuesday and Thursday, 12-1:20pm
 * Location: 540-108
 * Office Hours: Tuesday 2-3pm (Scott) and TBD (Kevin)
 
## Grading
 * 4 Assignments: 15% each
 * Midterm Exam: 15% 
 * Final Project Proposal: 5%
 * Final Project Report: 15%
 * In-class Participation: 5% 
 
*Late policy*: All assignments are due at 11:59pm PT on the due date.  You can turn in homework assignments up to a week late with a 50% penalty on your grade.  Final project reports will not be accepted after the deadline.  

*Midterm*: The midterm will be given in class.

## Final project

The final project is an opportunity to apply these models and algorithms to datasets of interest to you.  Ideally, your project will involve some theory &ndash; extending a model to fit the needs of your particular problem and studying its properties &ndash; and some experimentation &ndash; fitting the model to biological data.  

*Proposal*:  Start thinking about what datasets you'd like to study and what questions you'd like to answer early!  These will inform your choices about modeling tools.  As a forcing function, part of your grade will be based on your proposal, which is due roughly a month before the final report.  By this point, you should have a pretty clear idea about the dataset and question, and some initial thoughts about the types of models you will explore and experiments you will run.

*Report*: The final report will present your theoretical work and experimental results.  It should look like the start of a research paper.  To that end, you will write it in the NeurIPS paper format, and you will submit a link to a GitHub repository with supporting code.
 
# Tentative Schedule

| Lecture |  Date  | Topic | Technical Readings | Applications |
| :------:|:------:|-------|--------------------|--------------|
| 1       | Jan 7  | Probability Review | Bishop (2006) Ch 2 <br> Murphy (2013) Ch 2| &mdash; |
| 2       | Jan 9  | Graphical Models, Learning, and Inference | Barber (2010) Ch 3 and 4 <br> Wainwright and Jordan (2008) Ch 2| |
| 3       | Jan 14 | Linear and Generalized Linear Models | Bishop (2006) Ch 3 and 4  <br> Hastie et al (2009) Ch 3 and 4 <br> Murphy (2013) Ch 7-9 | |
| 4       | Jan 16 | Autoregressive Models <br> **<font color="red">HW1 Out</font>** | Larochelle and Murray (2011) <br> van den Oord (2016a, 2016b) | Pillow et al (2008) |
| 5       | Jan 21 | Latent Variable Models: Mixtures and Factors | Murphy (2013) Ch 11 and 12 <br> Bishop Ch 9 and 12 | Pachitariu et al (2016) <br> Mackevicius et al (2019) |
| 6       | Jan 23 | Expectation Maximization | | |
| 7       | Jan 28 | Models of Networks and Tensors | Hoff et al (2002) <br> Gopalan and Blei (2013) | Williams et al (2017) <br> Linderman et al (2016) |
| 8       | Jan 30 | Variational Inference and vEM <br> **<font color="red">HW1 Due &middot; HW2 Out</font>** | Blei et al (2017) | |
| 9       | Feb 4  | Variational Autoencoders (VAE's) | Rezende et al (2014) <br> Kingma and Welling (2014) | |
| &mdash; | Feb 6  | **<font color="red">Midterm Exam</font>** | | |
| 10      | Feb 11 | Markov Chains | Robert and Casella (2004) Ch 4| Ewens and Grant (2005) Ch 4 |
| 11      | Feb 13 | Hidden Markov Models <br> **<font color="red">HW2 Due &middot; HW3 Out</font>** | Bishop (2006) Ch 13 <br> Barber (2010) Ch 23 <br> Murphy (2013) Ch 17 | Wiltschko et al (2015) <br> Friederich et al (2017) <br> Jewell et al (2018, 2019) |
| 12      | Feb 18 | Linear Gaussian Dynamical Systems | Barber (2010) Ch 24 <br> Murphy (2013) Ch 18 <br>  | Paninski et al (2010) <br> Macke et al (2013) | 
| 13      | Feb 20 | Switching Linear Dynamical Systems <br> **<font color="red">Project Proposal Due</font>** | Barber (2010) Ch 25 <br>  Linderman et al (2017) | Linderman et al (2019) <br> Taghia et al (2018) <br> Petreska et al (2011) |
| 14      | Feb 25 | Gaussian Processes | Rasmussen and Williams (2006) Ch 2 <br> Hensman et al (2013) <br> Titsias and Lawerence (2010) <br> Wang et al (2019) | Cunningham et al (2008) <br> Wu et al (2017) |
| 15      | Feb 27 | Poisson Processes <br> **<font color="red">HW3 Due &middot; HW4 Out</font>** | Kingman (1993) Ch 1 and 2 <br> [Uri Eden's Notes](http://www.stat.columbia.edu/~liam/teaching/neurostat-fall19/uri-eden-point-process-notes.pdf) | Truccolo et al (2005) <br> Cunningham et al (2010) | 
| 16      | Mar 3  | Guest Lecture: Structured, Sequential VAE's | Johnson et al (2016) | Gao et al (2016) <br> Pandarinath  et al (2017) |
| 17      | Mar 5  | Continuous Time Markov Chains | | |
| 18      | Mar 10 | Hawkes and Cox Processes | Linderman and Adams (2014) <br> Kingman (1993) Ch 6 | |
| 19      | Mar 12 | Kingman's Coalescent <br> **<font color="red">HW4 Due</font>** | Kingman (1982) <br> Norborg (2004) | |
| &mdash; | Mar 20 | **<font color="red">Final Report Due</font>** | | |

# References

## Textbooks
[Barber, D. (2012). _Bayesian reasoning and machine learning_. Cambridge University Press.](http://web4.cs.ucl.ac.uk/staff/D.Barber/textbook/090310.pdf)

[Bishop, C. M. (2006). _Pattern recognition and machine learning_. Springer.](https://www.microsoft.com/en-us/research/uploads/prod/2006/01/Bishop-Pattern-Recognition-and-Machine-Learning-2006.pdf)

[Hastie, T., Tibshirani, R., & Friedman, J. (2009). _The elements of statistical learning: data mining, inference, and prediction_. Springer-Verlag.](https://web.stanford.edu/~hastie/ElemStatLearn/)

[Kingman, J. F. C. (1993). _Poisson processes_. Clarendon Press.](https://www.amazon.com/Poisson-Processes-Oxford-Studies-Probability/dp/0198536933) <br>
_Available in library_

[MacKay, D. J. (2003). _Information theory, inference and learning algorithms_. Cambridge university press.](http://www.inference.org.uk/itprnn/book.pdf)

[Murphy, K. P. (2012). _Machine learning: a probabilistic perspective_. MIT press.](https://www.cs.ubc.ca/~murphyk/MLbook/) <br>
_Available in library_

[Williams, C. K., & Rasmussen, C. E. (2006). _Gaussian processes for machine learning_. MIT press.](http://www.gaussianprocess.org/gpml/)

[Robert, C., & Casella, G. (2013). _Monte Carlo statistical methods_. Springer.](https://www.springer.com/gp/book/9780387212395)

[Wainwright, M. J., & Jordan, M. I. (2008). Graphical models, exponential families, and variational inference. _Foundations and Trends® in Machine Learning_, 1(1–2), 1-305.](https://people.eecs.berkeley.edu/~wainwrig/Papers/WaiJor08_FTML.pdf)

## Papers

[P.D. Hoff, A.E. Raftery, and M.S. Handcock. Latent space approaches to social network analysis. J. Amer. Statist. Assoc., 97(460):1090–1098, 2002.](http://www.stat.washington.edu/research/reports/2001/tr399.pdf)
