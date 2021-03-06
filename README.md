# Smell Patterns as Indicators of Design Degradation: Do Developers Agree?
## Complementary Material

### Common Refactorings for Each Smell Explored in Our Study

|Code Smell                |Common Refactoring   |
|----------------|-------------------------------|
|Complex Class			|Extract Method, Move Method, Extract Class [1]	|
|Dispersed Coupling		|Extract Method							   		|
|Feature Envy          	|Move Method, Move Field, Extract Field [2]		|
|God Class          	|Extract Class, Move Method, Move Field [1]		|
|Intensive Coupling     |Move Method, Extract Method					|
|Lazy Class				|Inline Class, Collapse Hierarchy [2]			|
|Lazy Method          	|Extract Method [2]								|
|Shotgun Surgery        |Move Method, Move Field, Inline Class [2]		|
|Speculative Generality	|Collapse Hierarchy, Inline Class, Remove Parameter, Rename Method [2]|

### Participants Characteristics
We recruited the participants of this quasi-experiment through our network of contacts in the industry and other research groups. We also looked for potential participants in our professional social media (Twitter and LinkedIn). We defined the following criteria to select the final list of participants:
1. Intermediary knowledge about the Java programming language.
2. Intermediary knowledge about software architecture.
3. Basic knowledge about code smells and refactoring.
4. More than one year of experience with software development.

The participants themselves informed such characteristics through a characterization form. We did not conduct any tests to verify the experience
and level of knowledge on each topic. The following table contains information on the selected participants for this study.

![image](https://user-images.githubusercontent.com/105753798/176332063-8aaf568e-e396-4ddb-a828-fb099c91bd8b.png)

### Forms
The forms used in our study can be found in the folder [`/forms`](https://github.com/sbes22patterns/smell-patterns/tree/main/forms) at our git.

[**Characterization Form - Structural Degradation Experiment - Formulários Google.pdf**](https://github.com/sbes22patterns/smell-patterns/blob/main/forms/Characterization%20Form%20-%20Structural%20Degradation%20Experiment%20-%20Formul%C3%A1rios%20Google.pdf): Characterization form of our quasi-experiment

[**Characterization Form - Structural Degradation Experiment (answers) - Answers to form 1.csv**](https://github.com/sbes22patterns/smell-patterns/blob/main/forms/Characterization%20Form%20-%20Structural%20Degradation%20Experiment%20(answers)%20-%20Answers%20to%20form%201.csv): Answers to the characterization form of our quasi-experiment

[**Experiment - Formulários Google.pdf**](https://github.com/sbes22patterns/smell-patterns/blob/main/forms/Experiment%20-%20Formul%C3%A1rios%20Google.pdf): Form used during the quasi-experiment

[**Post-Study Interview - Formulários Google.pdf**](https://github.com/sbes22patterns/smell-patterns/blob/main/forms/Post-Study%20Interview%20-%20Formul%C3%A1rios%20Google.pdf): Form used during the quasi-experiment as a post-study interview

### Automated Tool
The tool that we developed is available in the folder [`/automated tool`](https://github.com/sbes22patterns/smell-patterns/tree/main/automated%20tool). It contains:
 a [**README.pdf**](https://github.com/sbes22patterns/smell-patterns/blob/main/automated%20tool/README.pdf) that explains how to run our tool, available in the zipped file [**degradation-experiment-v0.1.1-OPT.zip**](https://github.com/sbes22patterns/smell-patterns/blob/main/automated%20tool/degradation-experiment-v0.1.1-OPT.zip). The training used in our quasi-experiment is found in [**Training.pdf**](https://github.com/sbes22patterns/smell-patterns/blob/main/automated%20tool/Training.pdf)

### Codes and Categories Derived From the Qualitative Analysis
The groups and categories
created during our qualitative analysis are presented in the folder [`/codes and categories`](https://github.com/sbes22patterns/smell-patterns/tree/main/codes%20and%20categories). The folder has the following files:

[**There is Degradation Problem and Accepted Refactoring**](https://github.com/sbes22patterns/smell-patterns/blob/main/codes%20and%20categories/There%20is%20Degradation%20Problem%20and%20Accepted%20Refactoring.png): This shows the codes created that led us to understand the cases in which the developers accepted that there was a degradation problem and accepted the refactorings proposed.

[**There is a Degradation Problem and Do Not Accept Refactoring.png**](https://github.com/sbes22patterns/smell-patterns/blob/main/codes%20and%20categories/There%20is%20Degradation%20Problem%20and%20Do%20Not%20Accept%20Refactoring.png): This shows the codes created that led us to understand the cases in which the developers accepted that there was a degradation problem and do not accept the refactorings proposed.

[**There is No Degradation Problem.png**](https://github.com/sbes22patterns/smell-patterns/blob/main/codes%20and%20categories/There%20is%20No%20Degradation%20Problem.png): This shows the codes created that led us to understand the cases in which the developers said that there was no degradation problem.

### Controlled Experiment
For **RQ1: Are Smell Patterns Indicators of Degradation?**, we have the following:

Null hypothesis
- H0: "smell patterns do not indicate degradation"

As alternative hypotheses, we have the following:
- H1.: Single Smell Patterns are indicators of degradation
- H2.: Multiple Smell Patterns are indicators of degradation

For **RQ2: Can Smell-Patterns Indicate Refactoring Opportunities?**, we have the following:
Null hypothesis
- H0: "smell patterns can not indicate refactoring opportunities"

As alternative hypotheses, we have the following:
- H1.: Single Smell Patterns can indicate refactoring opportunities
- H2.: Multiple Smell Patterns can indicate refactoring opportunities

Independent Variables:
- Software Systems
- Familiarity with Software Systems
- Use of SSP
- Use of MSP
- Use of Other Combination of Smells

Dependent Variables:
- Presence of Degradation (RQ1)
- Acceptance of Refactoring Opportunities (RQ2) (R3)

### Familiarity of Participants with the Systems
We asked the developers to provide their degree of familiarity with the systems analyzed. We have a scale ranging from "No Experience" to "Very High Experience". Those developers with some degree with experience are the ones that had contributed in some way to the system. This contribution is defined by the participant being part of the source code development. The participant with no experience are the ones who did not contribute with the source code but have knowledge of the source code and design of the system. These participants chose the system to be analyzed since they used it for research purposes.

### Summary of Participants Answers

The following table presents a summary of developers' answers.

The second column presents how many times (from the 6 cases) the developer agreed with the presence of a degradation problem. 

The third and fourth columns show how many times the developer considered the problem to be on an implementation or architectural level.

The fifth and Sixth columns show how many times developers agreed or partially agreed with the refactoring proposed.

![Screenshot from 2022-07-02 13-09-29](https://user-images.githubusercontent.com/105753798/177008101-989bd917-6fa0-4a55-acc6-067fcbc26d81.png)


### References
[1] Bavota, G., Lucia, A.D., Penta, M.D., Oliveto, R., Palomba, F.: An experimental investigation on the innate relationship between quality and refactoring. Journal of Systems and Software 107, 1 { 14 (2015). DOI http://dx.doi.org/10.1016/j.jss.2015.05.024. URL http://www.sciencedirect.com/science/article/pii/S0164121215001053

[2] Fowler, M.: Refactoring: Improving the Design of Existing Code. Addison-Wesley Professional, Boston (1999)

