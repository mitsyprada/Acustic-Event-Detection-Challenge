### 

# Acoustic Event Detection Challenge

## Main Assignment for Applied Machine Learning

Applied Machine Learning is about the analysis of data coming from a sensor system. For proper analysis its is necessary to keep the integrity of the data coming from the sensor intact during processing of the data. To make the data suitable for decision making data we need to extract features from the data. Features are characteristics relevant for the task at hand or relevant to the data set under consideration. Once we have features we can (hopefully) use these to make decisions either directly by applying some rule on the features or by using machine learning techniques suitable for clustering, dimensional reduction, blind source separation or classification.

## The Acoustic Event Detection Challenge

In many nursing homes there is acoustic monitoring present. At present this monitoring is often based on a simple combined sound intensity and duration criterion. This makes the rate of false alarms high while, at the same time, the duration criterion leads to missing important but short-lived events. SoundAppraisal BV, of which I am one of the three owners, is currently developing sound analysis software to address this problem. We ask you to participate in this development and develop you own classifiers for the classes in the ESC-50 environmental sound recognition challenge.

## Materials

Using the ESC-50 dataset:

- [ESC-50](https://github.com/karoldvl/ESC-50)

and the tract and PTNE features obtained with:

- [libsoundannotator (library)](https://github.com/soundappraisal/libsoundannotator)
- [soundannotatordemo (example code)](https://github.com/soundappraisal/soundannotatordemo)

These algorithms use Python2, that is the reason we ran them fore you and stored the data (about 20 GB) : [**HERE**](https://hanzenl-my.sharepoint.com/:f:/g/personal/r_a_j_van_elburg_pl_hanze_nl/Eg63UYgj7ZlKgMYa6E8hg3wBbttPAcvn1ivbb8sSWQ-OEA?e=ifYKgB)

These files contain EdB and tract features as discussed in the following preprint:

- [Texture features for the reproduction of the perceptual organization of sound](https://arxiv.org/abs/1705.05271)

**NB: It is obligatory to base your features on the tract and EdB data!**

## Research Question

*Main research question*:

- Can we infer the source of a sound recording from the tract and E (dB) data?

*Subquestions*:

- How can we, based on the tract and E data, define a suitable set of features?
- Which algorithms can be used to solve this task?
- How does performance of the classifiers built depend on the machine learning algorithm and their parameters?
- How does performance of the classifiers built depend on feature extraction parameters?

## Tools

The tools in the following slides will be covered during the lectures, to prepare you for the challenge. This is the first time we run the challenge this way, and therefore none of this is tested or guaranteed to work.

Our goal is to address the challenge, if this requires learning additional techniques we will try to acquire these techniques in the course of the project.

## Tools: Software Development:

- Python3
- Version Control with Git
- Jupyter Notebook

## Tools: Machine Learning:

- Receiver Operator Curve and Related
- Features and Data Enrichment
- Cluster Analysis
- Classification

## Extra requirements:

- During the project and the course assignments you need to keep electronic notebooks using a Jupyter notebook.
- Electronic notebooks and further code should be stored in version control, the version control system we use is GIT and accompanying GitHub webinterfaces. Each student receives a private repository on GitHub.
- This year we program in Python 3.7 or higher.
- Recommended Python code editors: Spyder (Cross platform), Geany (Linux), PyCharm (Cross platform)



## Provisional Rubric Final Thesis:

|                  | Weight | Excellent (10)                                               | Good (8)                                                     | Fair (5.5)                                                   | Insufficient (3)                                             |
| :--------------- | :----- | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
|                  |        |                                                              |                                                              |                                                              |                                                              |
| Machine Learning | t.b.d. | Machine learning techniques are applied leading to correct interpretations and the techniques are compared using correct performance evaluations. The choice of features used is motivated and clearly related to application domain knowledge. | Machine learning techniques are applied leading to correct interpretations and the techniques are compared using correct performance evaluations. The choice of features used is motivated. | Machine learning is applied leading to correct interpretations substantiated by correct performance evaluations. | Machine learning is applied but visible errors are present in concepts, implementation or performance evaluation. |

 

## Rubric Final Assignment AML:

|                                       | Weight | Excellent (10)                                               | Good (8)                                                     | Fair (5.5)                                                   | Insufficient (3)                                             |
| :------------------------------------ | :----- | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| Version Control                       | 0.1    | All code is under version control and for each feature and each algoritm there is at least a separate commit. Final findings can be easily reproduced running an Jupyter electronic notebook. Important intermediate data is available and can be used to verify later processing steps. | All code is under version control and for each feature and each algoritm there is at least a separate commit. Final findings can be easily reproduced running an Jupyter electronic notebook. | All code is under version control and there is at least a separate commit for each feature and each algoritm. | Although the work has been submitted using GIT, no version control was used during the implementation of the project. |
| Python Code                           | 0.1    | Code works as intended and intentions are indicated in code comments. Each Python module or script contains a header explaining it purpose, these headers make use of lightweight markup were necessary. At the project level a README is available explaining relationships between scripts and modules in the project, and indicating dependencies on non-standard library modules. | Code works as intended and intentions are indicated in code comments. Each Python module or script contains a header explaining it purpose, these headers make use of lightweight markup were necessary. | Code works as intended and intentions are indicated in code comments. | No working code provided or code is provided without explanatory comments |
| Documentation                         | 0.1    | Sufficient documentation is available to allow for reproduction of the results. Documentation facilitates use, maintenance and extension of the code in future projects. | Sufficient documentation is available to allow for reproduction of the results. Documentation facilitates use and maintenance of code in future projects. | Sufficient documentation is available to allow for reproduction of the results. | No documentation is present or documentation is visibly insufficient for reproduction of the results. |
| Machine Learning                      | 0.3    | Correct application of machine learning methods for cluster analysis and classification. Parameters of the machine learning methods are varied. Parameters of the machine learning methods are varied and data is correctly split in training, validation and test data. Results are compared with results found in the literature. | Correct application of machine learning methods for cluster analysis and classification. Parameters of the machine learning methods are varied and data is correctly split in training, validation and test data. | Correct application of machine learning methods for cluster analysis and classification. | Incorrect application or application lacking of machine learning methods for cluster analysis and classification. |
| Comparison of Algorithms and Features | 0.2    | ROC or Coverage plot which comparing parametrized families of classifiers associated with the subquestions and provides a reflection on the possible causes of the differences. Confusion matrix for the main alternatives and reflection on most of the occuring confusions. | ROC or Coverage plot which compares parametrized families of classifiers associated with the subquestions. Confusion matrix for the main alternatives and reflection on some of the occuring confusions. | ROC or Coverage plot provided which compares a individual instances of classifiers associated with the subquestions. Confusion matrices used to compare the main alternatives. | No ROC or Coverage plot used for comparing classifiers and features or they are used incorrectly. Or no confusion matrices used for comparing main alternatives. |
| Feature Construction                  | 0.2    | Multiple feature sets are used with motivation. Frequency information is used. | Multiple feature sets are used with motivation. Temporal alignment is applied corrrectly. | One individually chosen feature set is used with motivation. Temporal alignment is applied corrrectly. | Features as provided with the dataset are used unmodified. Or features are used without motivation. |

## Note:

The document source for this document is written in [Pandoc Markdown](http://pandoc.org/README.html#pandocs-markdown); a good editor with preview capabilities for Markdown is [Typora](https://typora.io/), but Jupyter also supports Markdown in its cells.

 