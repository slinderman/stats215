# Statistical Models in Biology

STATS215 	&middot; Winter 2020 &middot; Stanford University

## Course Description
This course is about probabilistic models in biology and the statistical inference algorithms necessary to fit them to data. We will cover some of the most important tools for modeling biological data, including latent variable models, hidden Markov models, dynamical systems, Poisson processes, and recent extensions like variational autoencoders and recurrent neural networks.  We will study algorithms for parameter estimation and inference, and we will apply these tools to a variety of problems across biology, with a particular emphasis on applications in neuroscience.  In your homework assignments and final project, you will implement these models and algorithms and apply them to real data.  

## Prerequisites
You should be comfortable with the basics of probability at the level of STAT116, including random variables, joint densities, conditional distributions, etc.  You should also be familiar with linear regression and maximum likelihood estimation, for example from STAT200.  We will use basic linear algebra (solving linear systems and using eigendecompositions) and multivariable calculus (gradients, Jacobians, Hessians, etc.). 

## Logistics
 * Instructor: [Scott Linderman](http://slinderman.web.stanford.edu/)
 * Teaching Assistant: [Kevin Han](mailto:kevinwh@stanford.edu)
 * Lectures: Tuesday and Thursday, 12-1:20pm
 * Location: 540-108
 * Office Hours: 
   * Scott: Tuesday 2-3pm Sequoia Hall Rm 232
   * Kevin: Monday 3-5pm Sequoia Hall Library
 
## Grading
 * 4 Assignments: 15% each
 * Midterm Exam: 10% 
 * Final Project Proposal: 5%
 * Final Project Report: 20%
 * In-class Participation: 5% 
 
*Late policy*: All assignments are due at 11:59pm PT on the due date.  You can turn in homework assignments up to a week late with a 50% penalty on your grade.  Final project reports will not be accepted after the deadline.  

*Midterm*: The midterm will be given in class.

## Assignments
Assignments consist of math problems and coding problems.  You will find a LaTeX template for your write-up in the GitHub folder.  Submit a pdf of your write-up and an .ipynb and .pdf of the Google Colab notebook with your completed coding assignment.  All submissions should be made through Canvas.

 * [Assignment 1](https://github.com/slinderman/stats215/tree/master/assignment1)
 * [Assignment 2](https://github.com/slinderman/stats215/tree/master/assignment2)
 * [Assignment 3](https://github.com/slinderman/stats215/tree/master/assignment3)

## Final project

The final project is an opportunity to apply these models and algorithms to datasets of interest to you.  Ideally, your project will involve some theory &ndash; extending a model to fit the needs of your particular problem and studying its properties &ndash; and some experimentation &ndash; fitting the model to biological data.  

*Proposal*:  Start thinking about what datasets you'd like to study and what questions you'd like to answer early!  These will inform your choices about modeling tools.  As a forcing function, part of your grade will be based on your proposal, which is due roughly a month before the final report.  By this point, you should have a pretty clear idea about the dataset and question, and some initial thoughts about the types of models you will explore and experiments you will run.

*Report*: The final report will present your theoretical work and experimental results.  It should look like the start of a research paper.  To that end, you will write it in the NeurIPS paper format, and you will submit a link to a GitHub repository with supporting code.
 
## Readings 
The readings are meant to supplement lecture with further details and show examples of how different models are being used in biology.  I've listed multiple technical readings and applications &ndash; you do **not** have to read all of them.  You may find it helpful to see the same concepts presented in different ways, or you may find that you like some author's style better than others.  Likewise, I've listed multiple references for many biological applications; I will reference some of these in class, and if you're curious you can dig into the others as well.
 
# Anticipated Schedule

| Lecture |  Date  | Topic | Technical Readings | Applications |
| :------:|:------:|-------|--------------------|--------------|
| 1       | Jan 7  | Probability Review | Bishop (2006) Ch 2 <br> Murphy (2013) Ch 2| |
| 2       | Jan 9  | Graphical Models, Learning, and Inference | Bishop (2006) Ch 8 <br> Barber (2010) Ch 3 and 4 <br> Wainwright and Jordan (2008) Ch 2| Gene Interaction Networks: [Friedman et al (2000)](http://research.cs.queensu.ca/home/shatkay/490papers/FriedmanBayesianNetworks2000.pdf) |
| 3       | Jan 14 | Bayesian Linear Regression | Bishop (2006) Ch 3 and 4  <br> Hastie et al (2009) Ch 3 and 4 <br> Murphy (2013) Ch 7-9 | GWAS: [Visscher et al (2017)](https://www.sciencedirect.com/science/article/pii/S0002929717302409) &middot; [Hilary Finucane's Notes](https://www.dropbox.com/s/eoq94zkzowwkths/Linear_models_for_GWAS_Part_1.pdf?dl=0) &middot; [Kang et al (2010)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3092069/) &middot; [Lippert et al (2011)](https://www.nature.com/articles/nmeth.1681) and [Supp](https://static-content.springer.com/esm/art%3A10.1038%2Fnmeth.1681/MediaObjects/41592_2011_BFnmeth1681_MOESM290_ESM.pdf)|
| 4       | Jan 16 | Logistic Regression <br> **<font color="red">HW1 Out</font>** | Goodfellow et al (2016) Ch 6, 8, 9 | Predicting retinal responses: [Pillow et al (2008)](https://www.ncbi.nlm.nih.gov/pubmed/18650810) &middot; [McIntosh et al (2016)](https://papers.nips.cc/paper/6388-deep-learning-models-of-the-retinal-response-to-natural-scenes.pdf) &middot; [Batty et al (2017)](https://openreview.net/forum?id=HkEI22jeg) |
| 5       | Jan 21 | Generalized Linear Models and Exp. Families | Murphy (2013) Ch 9 <br> [demo notebook](https://colab.research.google.com/drive/1tHc5S11azB-hJEeXZMVBWKN2TJ26B9N_) | Predicting retinal responses: [Pillow et al (2008)](https://www.ncbi.nlm.nih.gov/pubmed/18650810) &middot; [McIntosh et al (2016)](https://papers.nips.cc/paper/6388-deep-learning-models-of-the-retinal-response-to-natural-scenes.pdf) &middot; [Batty et al (2017)](https://openreview.net/forum?id=HkEI22jeg) |
| 6       | Jan 23 | Latent Variable Models: Mixtures, Factors, and EM Part I | Murphy (2013) Ch 11 and 12 <br> Bishop Ch 9 and 12 | Spike sorting: [Pachitariu et al (2016)](https://www.biorxiv.org/content/10.1101/061481v1) &middot; [Liam Paninski's Notes](http://www.stat.columbia.edu/~liam/teaching/neurostat-fall19/em-notes.pdf) |
| 7       | Jan 28 | Latent Variable Models: Mixtures, Factors, and EM Part II | Murphy (2013) Ch 11 and 12 <br> Bishop Ch 9 and 12 | Receptive fields: [Liu et al (2017)](https://www.nature.com/articles/s41467-017-00156-9) <br> Finding motifs: [Mackevicius et al (2019)](https://elifesciences.org/articles/38471)|
| 8       | Jan 30 | Latent Variable Models: Mixtures, Factors, and EM Part III  <br> **<font color="red">HW1 Due &middot; HW2 Out</font>**| Murphy (2013) Ch 11 and 12 <br> Bishop Ch 9 and 12 <br> [demo notebook](https://colab.research.google.com/drive/1lLRfOUatOlfUMrixeMDDpKVoxajRweLB) | Pose estimation with missing data: [Markowitz et al (2018)](https://www.sciencedirect.com/science/article/pii/S0092867418305129) |  
| 9       | Feb 4 | Variational Inference and Nonlinear LVMs: Part I | [Blei et al (2017)](https://arxiv.org/abs/1601.00670) | Network Models: [Gopalan and Blei (2013)](https://www.pnas.org/content/110/36/14534) &middot; [Linderman et al (2016)](https://papers.nips.cc/paper/6185-bayesian-latent-structure-discovery-from-multi-neuron-recordings.pdf) |
| &mdash; | Feb 6  | **<font color="red">Midterm Exam</font>** | | |
| 10      | Feb 11 | Midterm Review | | |
| 11      | Feb 13 | Variational Inference and Nonlinear LVMs: Part II | [Kingma and Welling (2019) Ch 2](https://arxiv.org/pdf/1906.02691.pdf) <br> [demo notebook](https://colab.research.google.com/drive/1MQiTLhGVVgRxGA89WXHe9C1gpFJz6Q-g) | Single cell RNAseq: [Lopez et al (2018)](https://www.nature.com/articles/s41592-018-0229-2) and [blog](https://bair.berkeley.edu/blog/2018/12/05/genes/) &middot; [Grønbech et al (2018)](https://www.biorxiv.org/content/biorxiv/early/2018/05/16/318295.full.pdf) |
| 12      | Feb 18 | Hidden Markov Models <br> **<font color="red">HW2 Due &middot; HW3 Out</font>** | Bishop (2006) Ch 13 <br> Barber (2010) Ch 23 <br> Murphy (2013) Ch 17 | Calcium deconvolution: [Friederich et al (2017)](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005423) &middot; [Jewell et al (2018, 2019)](https://jewellsean.github.io/fast-spike-deconvolution) |
| 13      | Feb 20 | Linear Gaussian Dynamical Systems <br> **<font color="red">Project Proposal Due</font>** | Barber (2010) Ch 24 <br> Murphy (2013) Ch 18 <br> [demo notebook](https://colab.research.google.com/drive/11If3E63EU-ckZ1ma57zt_NnCWkWg6VLH) | Neural state spaces: [Paninski et al (2010)](http://www.stat.columbia.edu/~liam/research/pubs/jcns-state-space-review.pdf) &middot; [Macke et al (2011)](http://www.gatsby.ucl.ac.uk/~maneesh/papers/macke-etal-2011-nips-preprint.pdf) | 
| 14      | Feb 25 | Switching Linear Dynamical Systems | Barber (2010) Ch 25 <br>  [Linderman et al (2017)](http://proceedings.mlr.press/v54/linderman17a.html) | Postural dynamics: [Wiltschko et al (2015)](https://www.cell.com/neuron/fulltext/S0896-6273(15)01037-5) <br> Neural circuit dynamics: [Linderman et al (2019)](https://www.biorxiv.org/content/10.1101/621540v1) &middot; [Taghia et al (2018)](https://www.nature.com/articles/s41467-018-04723-6) |
| 15      | Feb 27 | Gaussian Processes | Rasmussen and Williams (2006) Ch 2 <br> [Hensman et al (2013)](http://www.auai.org/uai2013/prints/papers/244.pdf) <br> [Titsias and Lawerence (2010)](http://proceedings.mlr.press/v9/titsias10a/titsias10a.pdf) <br> [Wang et al (2019)](https://arxiv.org/abs/1903.08114) | Odor representation in cortex: [Wu et al (2017)](https://papers.nips.cc/paper/6941-gaussian-process-based-nonlinear-latent-structure-discovery-in-multivariate-spike-train-data) and [2018](http://papers.nips.cc/paper/7783-learning-a-latent-manifold-of-odor-representations-from-neural-responses-in-piriform-cortex) |
| 16      | Mar 3  | Guest Lecture: Matt Johnson <br> Structured, Sequential VAE's <br> **<font color="red">HW3 Due &middot; HW4 Out</font>**| [Johnson et al (2016)](https://papers.nips.cc/paper/6379-composing-graphical-models-with-neural-networks-for-structured-representations-and-fast-inference) | Nonlinear embedding of neural activity: [Gao et al (2016)](http://papers.nips.cc/paper/6430-linear-dynamical-neural-population-models-through-nonlinear-embeddings) &middot; [Pandarinath  et al (2018)](https://www.nature.com/articles/s41592-018-0109-9) |
| 17      | Mar 5 | Poisson Processes | Kingman (1993) Ch 1 and 2 <br> [Uri Eden's Notes](http://www.stat.columbia.edu/~liam/teaching/neurostat-fall19/uri-eden-point-process-notes.pdf) | Neural firing rates: [Brown et al 2002](https://www.mitpressjournals.org/doi/abs/10.1162/08997660252741149?casa_token=ajv4s9er27AAAAAA%3AFWMF03w7_y5tRQHES9AlMa6LeFJUGJG2ogV5dPZHy2d7t8TtjMtcfQhqYUv1dX_5dcTjCplEi_Y&) &middot; [Truccolo et al (2005)](https://www.ncbi.nlm.nih.gov/pubmed/15356183) &middot; [Cunningham et al (2008a](http://www.gatsby.ucl.ac.uk/~maneesh/papers/cunningham-etal-2008-icml.pdf) and [2008b)](http://www.stat.columbia.edu/~cunningham/pdf/CunninghamNIPS2008.pdf) &middot; [Loaiza-Ganem et al (2019)](https://papers.nips.cc/paper/9491-deep-random-splines-for-point-process-intensity-estimation-of-neural-population-data)| 
| 18      | Mar 10  | Continuous Time Markov Chains | | Complex synapses: [Lahiri and Ganguli (2013)](https://ganguli-gang.stanford.edu/pdf/Synapse.NIPS14.pdf) and [Supp](https://ganguli-gang.stanford.edu/pdf/Synapse.NIPS14.Supp.pdf) |
| 19      | Mar 12 | Hawkes and Cox Processes <br> **<font color="red">HW4 Due</font>**  | [Hawkes (1971)](https://www.jstor.org/stable/2334319?seq=1#metadata_info_tab_contents) <br> Kingman (1993) Ch 6 | Social contagion: [Linderman and Adams (2014)](http://proceedings.mlr.press/v32/linderman14.pdf) |
| &mdash; | Mar 20 | **<font color="red">Final Report Due</font>** | | |


# Textbooks
[Barber, D. (2012). _Bayesian reasoning and machine learning_. Cambridge University Press.](http://web4.cs.ucl.ac.uk/staff/D.Barber/textbook/090310.pdf)

[Bishop, C. M. (2006). _Pattern recognition and machine learning_. Springer.](https://www.microsoft.com/en-us/research/uploads/prod/2006/01/Bishop-Pattern-Recognition-and-Machine-Learning-2006.pdf)

[Ewens, W. J., & Grant, G. (2005). _Statistical Methods in Bioinformatics_. Springer.](https://www.springer.com/gp/book/9780387400822) <br>
_Available in library_

[Goodfellow, I., Bengio, Y., & Courville, A. (2016). _The deep learning book._ MIT Press.](http://www.deeplearningbook.org/)

[Hastie, T., Tibshirani, R., & Friedman, J. (2009). _The elements of statistical learning: data mining, inference, and prediction_. Springer-Verlag.](https://web.stanford.edu/~hastie/ElemStatLearn/)

[Kingman, J. F. C. (1993). _Poisson processes_. Clarendon Press.](https://www.amazon.com/Poisson-Processes-Oxford-Studies-Probability/dp/0198536933) <br>
_Available in library_

[MacKay, D. J. (2003). _Information theory, inference and learning algorithms_. Cambridge university press.](http://www.inference.org.uk/itprnn/book.pdf)

[Murphy, K. P. (2012). _Machine learning: a probabilistic perspective_. MIT press.](https://www.cs.ubc.ca/~murphyk/MLbook/) <br>
_Available in library_

[Williams, C. K., & Rasmussen, C. E. (2006). _Gaussian processes for machine learning_. MIT press.](http://www.gaussianprocess.org/gpml/)

[Robert, C., & Casella, G. (2013). _Monte Carlo statistical methods_. Springer.](https://www.springer.com/gp/book/9780387212395)

[Wainwright, M. J., & Jordan, M. I. (2008). Graphical models, exponential families, and variational inference. _Foundations and Trends® in Machine Learning_, 1(1–2), 1-305.](https://people.eecs.berkeley.edu/~wainwrig/Papers/WaiJor08_FTML.pdf)

