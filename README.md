# EEP 153 Spring 2024 - Project 03 (Team Ernst Engel)

## Team Members
Jordan Taqi-Eddin - jgte29@berkeley.edu; GitHub: jgte29

Samantha Wu - samanthawu@berkeley.edu; GitHub: wusamantha

Himalia Joshi - s.himalia.joshi@berkeley.edu; GitHub: s-himalia-j

Henry Kao - henrykao@berkeley.edu; GitHub: Henry_Kao21

Jeffrey Chou - jeffreychou01@berkeley.edu; GitHub: JeffreyChou01

## Welcome

Welcome to the Project 02 GitHub Repository for Team Ernst Engel. Our code for the project is organized in the following format:
- master_notebook.ipynb: In this notebook, we compile all of the finished products of code for this project. <br>
**Note:** To test the functionality of all our code, only this notebook needs to be run. If it works, it indicates that all of the code in the other notebooks are properly running.
- nutritional_adequacy.ipynb: In this notebook, we examine the nutritional adequacy of the diets of the households in our analysis.
- nutritional_content.ipynb: In this notebook, we obtain the nutritional contents for the foods of interest for our project.
- demand.ipynb: In this notebook, we examine a system of demands for various food products, and examine heterogeneity in household consumption.

## How to Use
1. Option A: Access Our Repository Via DataHub (*Highly Recommended*)
   - You can access all of the code in our repository via DataHub using this [link](https://datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Fjgte29%2Fteam-ernst-engel-proj03.git&urlpath=lab%2Ftree%2Fteam-ernst-engel-proj03.git%2F&branch=main).
2. Option B: Clone the repository on your local device:
   ```bash
   git clone https://github.com/jgte29/team-ernst-engel-proj03.git

### Notebook Specific Notes:
- master_notebook.ipynb:
     1) To test the functionality of all our code, only this notebook needs to be run. If it works, it indicates that all of the code in the other notebooks are properly running.
     2) Understanding Nutritional Adequacy
We choose take adopted a nuanced approach to examing Nutritonal Adequacy in our project. The best way to explain our approach is through an example. Suppose we have the following nutritional requirements and consumption data for some arbitrary household.

| **Nutrient** | A | B | C | D | Adequacy Share
|:-----------:|:----------:|:-----------:|:----------:|:-----------:|:-----------:|
| **Intake** | 105 kg |53 kg|75 kg|29 kg||
| **Requirement** | 100 kg |100 kg|100 kg|100 kg| |
| **100% Adequacy** | $\times$ | | | | 0.25 |
| **75% Adequacy** | $\times$ | | $\times$ | | 0.50 |
| **50% Adequacy** | $\times$ | $\times$ | $\times$ | | 0.75 |

As we see in the able above, Adequacy Share at some Adequacy Level $\alpha$ is the proportion of nutrients for which a housholds total intake of the nutrient is greater than or equal to $\alpha$. <br>
$$\text{Adequacy Share}_{h} = \frac{\sum_{i = 1}^{n} \textbf{1}(\frac{\textit{Nutrient i Intake}_{h}}{\textit{Nutrient i Requirement}_{h}} \ge \alpha)}{n}; \hspace{0.1cm} \forall \text{ Households } h$$
- nutritional_adequacy.ipynb: In this notebook, we examine the nutritional adequacy of the diets of the households in our analysis.
- nutritional_content.ipynb: In this notebook, we obtain the nutritional contents for the foods of interest for our project.
- demand.ipynb: In this notebook, we examine a system of demands for various food products, and examine heterogeneity in household consumption.
