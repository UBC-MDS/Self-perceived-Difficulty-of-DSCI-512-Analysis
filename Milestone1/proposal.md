# Proposal

## Identify the question that your team is interested in answering with the survey. The aim of the survey should be to try to answer one specific and testable question.

DSCI 512 is a programming and algorithms course in the MDS program at UBC which introduces fundamental algorithms such as sorting and searching, as well as data structures. According to a poll done during the course, some students reported that they have been experiencing a hard time with course materials and lab assignments. This leads to our survey question:

Does their level of programming experience prior to the MDS program influence a person's self-perceived difficulty of DSCI 512 (Algorithms and Data Structures)?

## Identify the other questions you plan to ask in your survey to identify confounding variables and justify/explain why you plan to include them.

### 1.0 Confounding Variable: Sex (type: category)

**Explanation**: Sex is based on a biological classification system.  It has been included as a confounding variable because there is evidence to suggest that biological differences between males and females might affect a student's perceived difficulty of the course.  For example, it is reported that on average, females are more prone to stress than males[1].  This is relevant to our question because, for example, difficulty may be more acutely perceived by a student who is more prone to stress.  Females have historically been underrepresented in computing occupations[2] which suggests that they are also less likely to have programming experience.  Therefore, sex may affect both programming experience as well as perceived difficulty in DSCI 512.

**Questions**: Sex?

**Options**: 1) Female, 2) Male

### 2.0 Confounding Variable: Math Skills (type: ordinal)


**Explanation**: Mathematics is an essential skill when it comes to learning algorithms. Algorithms are utilized everywhere to provide solutions to problems, but developing algorithms requires strong logical thinking abilities. Mathematics is the formal study of logical consequences, which is extremely important when understanding algorithms. Therefore, it is evident that students' mathematical abilities may affect their level of programming experience, as well as difficulty in learning DSCI 512.

**Questions**: Among all the math courses you have taken in the past, in general, how were your grades compared to others? For example, Calculus, Linear Algebra, Statistics.

**Options**: 1) Below average, 2) Average, 3) Above average


### 3.0 Confounding Variable: Friends or family who have jobs associated with programming (type: category)

**Explanation**: Undoubtedly, friends are more likely to share common values and interests. Hence, if an MDS student has friends or family who work for IT companies, they are more likely to be affected and tend to have programming experience before the program. During the course, those friends could provide help so that students are less stressed when they have problems and experience less difficulty in the course.

**Questions**: Do you have any friends or family who have jobs associated with programming?

**Options**: 1) No, 2) Yes


### 4.0 Main Covariate: Previous programming experience (type: ordinal)

**Explanation**: The level of the previous programming experience is a potential reason for variation of the self-perceived difficulty regarding DSCI 512.

**Questions**: How much programming experience did you have prior to the MDS program?  Please select the highest level that applies to you.

**Options**: 1) None, 2) Less than 100 hours, 3) Less than 1000 hours, 4) More than 1000 hours


### 5.0 Outcome: Self-perceived difficulty regarding DSCI 512 (type: ordinal)

**Explanation**: Self-perceived difficulty regarding DSCI 512 is the outcome whose variation is being studied.

**Question**: How difficult did you find DSCI 512 relative to the other courses in the MDS program?

**Options**: 1) Easier than average,  2) Average, 3) More difficult than average.

</br>

| Variable | Name | Type |
|---|---|---|
| Confounder | Sex | category |
| Confounder | Math Skills | ordinal |
| Confounder | Friends who have jobs associated with programming | category |
| Main Covariate | Previous programming experience | ordinal |
| Outcome | Self-perceived difficulty | ordinal |

_A summary table of variables in our analysis_

## Describe how you plan to analyze the survey results (e.g., what statistical test(s) do you plan to employ?).

**Null hypothesis**: The level of programming experience prior to the MDS program does not influence a person's self-perceived difficulty regarding DSCI 512.

**Alternative hypothesis**: The level of programming experience prior to the MDS program influences a person's self-perceived difficulty regarding DSCI 512.

We plan to analyze the survey results in the following ways:

1) Exploratory Data Analysis (EDA)
- Summarize main characteristics of variables
- Adjust assumptions or method

2) Regression Test
- Perform Ordered Logistic Regression on the results of the survey
- Perform the Likelihood Ratio Test on each regression model and evaluate the results
- Determine the effect of covariates on outcome
- Change our test if deemed necessary

## Discuss the aspects of the UBC Office of Research Ethics document on Using Online Surveys that are relevant to your proposed survey.

According to the Office of Research Ethics document, the collection of opinions and information are considered personal information if the information could be linked or associated with the individual. Such data, if collected through a survey, must not be stored outside of Canada and should be surveyed through tools hosted within Canada. Some of the variables that we thought about including in our survey were potentially "personal information," such as an individual's age or gender. Due to the small population of our MDS program, it is definitely easy for this type of information to be identifying. As we are also taking a privacy and ethics course, we understand that these issues can bring many unnecessary problems. Ultimately, we decided to some variables, such as age, from our survey, regardless of whether they are confounding variables or not.

To comply with the UBC Office of Research Ethics, we would provide a cover letter (consent form) to all survey participants. The cover letter would include:

- the sentence:  “By completing the questionnaire, you are consenting to participate in this research.”
- the purpose of the survey
- a description of the topic of the survey
- contact information
- risks and benefits
- limits to confidentiality
-  a statement that participation is optional
- the UBC Research Participant Complaint Line text
- (if possible) the UBC letterhead

# References:

1: https://www.ncbi.nlm.nih.gov/pubmed/23239826

2: https://www.ncwit.org/sites/default/files/resources/womenintech_facts_fullreport_05132016.pdf
