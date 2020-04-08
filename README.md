
# raman-spectra-decomp-analysis
Code to calculate decomposition of materials using Raman spectroscopy.
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/raman-noodles/raman-spectra-decomp-analysis/master)
<img src="https://travis-ci.org/raman-noodles/raman-spectra-decomp-analysis.svg?branch=master">
<p align="center">
 <img src="https://github.com/raman-noodles/Raman-noodles/blob/master/docs/Raman%20Noodles%20Logo.PNG">
</p>

## This is the GitHub Repo for work completed for NSF DIRECT Data Accelerator Fellowship 2020
**Fellowship PI: Jim Pfaendtner; Fellowship Recipient: Elizabeth Rasmussen**

### Overall Project Objective
This project identifies, and calculates decomposition in a Raman spectra to output rate data. Advantages to using this method are:
1. FULLY Open source, no part of the project is dependent on a paid service
2. AUTOMATED process, analysis is automated leading to fast results
3. VERIFIABLE, user is made aware of how confident they can be in the results via a statistical software stack

- **More detailed background and motivation for the project can be found in the [Project Background and Motivation Wiki Page](https://github.com/raman-noodles/Raman-noodles/wiki/Project-Background-and-Motivation)**

### Assumptions and Project Scope
1. Storing data library that is beyond the decomposition products of formic acid (hydrogen, water, carbon dioxide, carbon monoxide) are not included as other components are beyond the scope of the project at this time.
- Assumed that the user is trying to analyze the decomposition products of formic acid, or a mixture that consists only of: Formic Acid, Hydrogen, Water, Carbon dioxide, Carbon monoxide.
2. This project will not be predictive - that is, it will require the user to specifically input what potential compounds will be present in the spectra to be analyzed. This list does not have to be exhaustive; however, the more inclusive the list, the better the fitting and predicting results will be. 

### Project Breakdown
The project can be thought of as broken down into 3 steps:
1. Data Wrangling
2. Peak fitting and identification
3. Statistical analysis for peak fits

These sections have their own wiki documents and filled juypter notebooks with more detail included throught, see those for more detail on the individual steps.

### User Flow and Example of Using Raman Noodles
A user will be able to follow the steps to apply Raman-Noodles to YOUR *Formic Acid* data set. An example of using the software can be seen in the [Example Use Case Wiki Page](https://github.com/raman-noodles/raman-spectra-decomp-analysis/wiki/Use-Cases)

### Testing of Raman Noodles and Travis-CI
In order to have manageable code we are using Travis' Open Source continuious itegration testing. One thing to note is that on March 1, 2018 Travis-CI switched their model for open source software, the press release about this can be read [here](https://blog.travis-ci.com/2018-05-02-open-source-projects-on-travis-ci-com-with-github-apps)

So we do have [our team repo viewable on travis-ci.com](https://travis-ci.org/raman-noodles/raman-spectra-decomp-analysis) **_BUT_** it will ultimately re-direct you to the _old_ platform for open source software on `travis-ci.org`.

There is a way to merge the `travis-ci.org` (open source repos only) to `travis-ci.com` (now private repos **and** (closed beta) open source repos) as can be seen by following [this link](https://docs.travis-ci.com/user/migrate/open-source-on-travis-ci-com/#existing-open-source-repositories-on-travis-ciorg) but at this time our team has decided to not join the closed beta as the current (old) method of the dashboard being located on `travis-ci.org` works just fine.

#### [Link to our active Travis-CI build dashboard](https://travis-ci.org/raman-noodles/raman-spectra-decomp-analysis)


### Future Work
Next steps would include automatic baseline subtraction of spectra to decrease pre-processing time, molar formation calculations to predict reaction pathways, and increased robustness of machine learning for component selection including unsupervised methods.


### Conclusion
In conclusion this is a platform code base for researchers to visualize and analyze their Raman spectra in a fast, automated manor - reducing post-processing time by days and enabling future work to continue on a solid base of open source tools.

  * This software has passed tests to sucessfully identify and analyze the identification of components in mixture Raman data.

  * This work sets up a free and user friendly platform for researchers to be able to analyze their own Raman Spectra.

### Acknowledgements
* Dave Beck and Jim Pfaendtner
* Data sets from publicly available from Mendeley Data, “Raman Spectra of Formic Acid Gasification Products in Subcritical and Supercritical Water”
* Only open source packages were used in this work.
