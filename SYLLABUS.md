# Syllabus<br>GEOS 518: Modeling Earth and Environmental Systems (Fall 2024)

--- 

### Instructor:
Dr. Alejandro (Lejo) Flores (he/him)  
Office Hours: Mondays 12-1:30pm in Geosciences Learning Hub (ERB 2102)
Email: [lejoflores@boisestate.edu](lejoflores@boisestate.edu)  

### Teaching Assistant:
Owen Walsh 
Office Hours: TBD 
Email: [owenwalsh@u.boisestate.edu](owenwalsh@u.boisestate.edu)  

---

### Course Description:
Computational models are tools used to describe, predict, and reveal new understanding about Earth and environmental systems. Develops the mindset and skills needed to apply, develop, and diagnose models of Earth and environmental processes. Knowledge and skills developed allow students to appraise existing models in the context of specific problems. Particular attention is paid to modeling hydrologic, geomorphic, atmospheric, critical zone, and ecological processes.

### Required Textbook:
The following textbook is optional for the class. It is fairly easy to find and reasonably priced: 

 * _Slingerland, Rudy and Kump, Lee_ (2011), Mathematical Modeling of Earth's Dynamical Systems: A Primer, Princeton University Press, 248 pp. | [Buy on Bookstore.org](https://bookshop.org/books/mathematical-modeling-of-earth-s-dynamical-systems-a-primer/9780691145143) | [Buy on Amazon.com](https://www.amazon.com/Mathematical-Modeling-Earths-Dynamical-Systems/dp/0691145148) | 

### Computer Access:
Being a numerical modeling class, access to computing resources is critical. Ideally, you would have access to a laptop computing that has internet access and on which you can install the required computing tools (`Python`, `JupyterLab`, and `git`, ideally via a package manager like `conda`). I acknowledge, however, that as Graduate Students your ability to procure a laptop that you can bring to class may be limited. If you need help finding access to a laptop for class, please contact me. There are a number of ways I can help. Chromebooks are potentially an option, but you will need to use Jupyter in cloud computing environment like    

### Recommended Software:
If you have experience in installing scientific computing software, or feel confident enough to try, the following software are the minimum you will need at the outset of the class. New requirements may arise throughout the semester, but you will have built some capabilities to install them. This class is committed to using only open source software and open science principles. 

* `Python 3`. I ___highly___ recommend you install via `Miniconda` or `Anaconda`. I also ___highly___ recommend that you create a new `conda` environment specifically for the class.
  * `Miniconda` installers for Windows, Mac, and Linux devices can be found here: [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)
  * `Anaconda` installers for Windows, Mac, and Linux devices can be found here: [https://docs.anaconda.com/anaconda/install/index.html](https://docs.anaconda.com/anaconda/install/index.html)
* `Jupyter`. For interactive computing and programming via your web browser. 
* `Numpy`. For numerical and mathematical computing.
* `Matplotlib`. For visualization and plotting results. 
* `Scipy`. For some more advanced statistical analysis. 
* `Pandas`. For data analysis, particularly time series analysis.

__A note on Integrated Development Environments (IDEs).__ Some students prefer to use IDEs to develop code as they can facilitate integration directly with GitHub and may have other extensions like AI chatbot support, support for remote connection to cloud and high performance computing, etc. I don't take a position on whether or not an IDE is the right way to go or not and have used a variety of them (and none) in the past. A number of IDEs are available for development in Python, some of which come bundled with installers like `Anaconda`. I will be using [VS Code](https://code.visualstudio.com/) (a freely available, cross platform development environment) throughout the class, but you can use the tools that work best for you. I don't claim to be an expert in any particular platform and students with more experience often teach me about features and extensions I didn't know about. I am committed to helping you develop the practices that work best for you, so please don't hesitate to ask me for tips and hints on what platforms and development tools might work for you. 

### Course Expectations:
This class has a mixed structure wherein the Monday class will be primarily lecture and the Wednesday class with be a coding workshop. In the Wednesday coding lab we will review example code that I have developed for each topic we cover in the class. Depending on how well you are able to understand, execute, and modify the example code you may also have time to get started on the associated assignment for each module.  

We will develop community expectations as a class, but it is important that we cultivate and maintain an inclusive and supportive environment. As such we will adhere to the Code of Conduct developed by the Software Carpentry Foundation that can be found at [https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html](https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html)

### Attendance:
* Review Boise State University's attendance policy at [https://www.boisestate.edu/registrar/home/registration/attendance-policy/](https://www.boisestate.edu/registrar/home/registration/attendance-policy/) 
* Due to the nature of the class, merely completing reading materials, quizzes, and reviewing this GitHub repository is a poor substitute for engaged and active participation.
* Please note that absences reduce your potential for class participation, and therefore, may reduce that portion of your grade.
* Class starts on time. I make announcements, answer questions, and give reminders immediately at the beginning of class. 

### Outside of Class:
* You are expected to read all emails and announcements.  
* The class reading/lecture/assignment/project schedule will be updated on Canvas. It is your responsibility to make sure you are staying up to date.
* Come prepared for class by reading assigned materials. ***Online quizzes*** are due prior to the designated class period (see grading section for details).
* If you need help, get it now! I am always willing to meet with you and go over questions or concerns. ***Do not wait until the end of the semester.***

### Academic Dishonesty:
Cheating or plagiarism in any form is unacceptable. All work submitted by a student must represent their own ideas, concepts, and current understanding. Beware the internet; if you can find it, so can your professor. Academic dishonesty also includes submitting substantial portions of the same academic coursework to more than one course for credit without prior permission of the instructor(s). Please be aware of your rights and responsibilities as a student by reviewing the Boise State Student Code of Conduct: [https://www.boisestate.edu/policy/student-affairs/code-of-conduct/](https://www.boisestate.edu/policy/student-affairs/code-of-conduct/)

### Educational Access for All Students:
Students with additional educational and access needs are encouraged to contact the proper resource as early as possible (Boise State Educational Access Center; [https://www.boisestate.edu/eac/](https://www.boisestate.edu/eac/)). The EAC assists Boise State staff and faculty in meeting accommodations mandated by Federal and State law and University policy. They will work with you to identify and document physical and learning needs and identify  appropriate accommodations for a student in their courses.

---

### Grading Summary (proportions may vary by up to 5%)

| Component | Proportion of Grade |
| --- | --- |
| Notebook Assignments | 40% |
| Notebook Reflection | 40% |
| Model Investigation Project | 20% |

#### Jupyter Notebook Programming Assignments (40%)
A significant part of your grade will be based on programming assignments in which you will use and/or build simple models of environmental processes and use them to explore topics being covered in the class. There will be approximately one programming assignment for each module of the class (there are approximately 9 modules) and the assignments will be complete when you post them as a Jupyter Notebook (`.ipynb` extension) on your own GitHub account and submit the link to the notebook on Canvas. For those unfamiliar with Jupyter and GitHub, we will provide a number of resources to help you get familiar and up and running with them. Generally you will copy a template assignment notebook from the class repository into a GitHub repository of your choice. That template will have instructions (and potentially some code) that is designed to lead you through the notebook assignment. __Note:__ Once you complete this class, you _could_ have a GitHub repository with all your submitted Jupyter Notebooks for the class that can serve to illustrate your computational skills to potential employers.  

For this component of the class grade, your assessment is based on completeness of the submitted notebookby the due date. Correctness will not be graded, but you may receive comments on the correctness. Each notebook assignment is weighted equally. __Late notebook submissions__: Notebooks can be submitted up to 3 days late for 50% credit and up to 7 days late for 25% credit. 

#### Jupyter Notebook Reflection (40%)
After all notebooks have been submitted, I will send the class the assignment key in the form of the completed Jupyter Notebook (as a side note, your assignments are often created by coding the keys first and then deleting code and cells to provide you hints). The reflection component of the grade is based on your comparison of the key to the code you submitted. You will be prompted to: (1) compare and contrast your code with that of the key, (2) outline what you would have done differently based on that comparison, and (3) discuss more broadly what new skills and knowledge you acquired by completing the assignment. The reflection is an opportunity for you to actively reflect on what you learned/struggled with/improved on during the assignment. If you invest in them, these reflections can be invaluable tools for you to assess your own learning progress and ensure that you are getting what you need/want out of the class. 

#### Modeling Investigation Project (20%)
You will also have a modeling project for the class. The purpose of this modeling project is for you to explore an existing model of interest to your professional development and/or research. During this project you will: (1) select a model for further study, (2) examine key details of the Earth and environmental processes that it models in the context of topics we cover in the class, (3) review the data needed to characterize initial and boundary conditions for the model, (4) investigate procedures and data needs for calibration/validation, and (5) design a numerical experiment to test a scientific hypothesis or perform a specific analysis. ___You will not need to setup, run, or perform your numerical experiment as a requirement of the project.___ However, this project could be a valuable tool to kickstart any modeling activities required for your thesis or dissertation. As such, I ___highly___ encourage you to consult with your advisor(s) and me when choosing a model. This project will be submitted as a Markdown (e.g., `PROJECT.md`) file in your GitHub repository for the class.   

--- 

### Course Learning Outcomes
Below are the Course Learning Outcomes (CLO) that we will achieve in the class. Click the triangle to expand each CLO to see supporting module-level learning objectives. At the end of this class, you will be able to:

<details>
<summary>1. Explain key steps and considerations in the choice and use of a numerical model for a scientific/engineering application</summary>
 
  * Differentiate between statistical and dynamical models  
  * List different applications for which a model is used  
  * Explain the concept of parsimony in the context of modeling  
  * Define a conceptual model in terms of how it represents underlying processes  
  * Draw an environmental system in terms of storage and flux variables
  * Write down the system of equations that describe a model 
  * Identify input variables to a model that are fixed in time (parameters)
  * Identify input variables to a model that vary with time (forcings) 
  * Articulate the benefits and drawbacks of model complexification
 
</details> 

<details>
<summary>2. Describe the necessity, process, and methods of model evaluation and calibration</summary>

  * Describe the concept of model calibration
  * List several alternative methods of quantifying model goodness-of-fit
  * Define equifinality and describe how it influences Earth/Environmental systems modeling
  * List some statistical measures useful for analyzing model outputs
  * Identify what parameters of a model need to or could be calibrated
  * Define the concept of Pareto optimality
  * Define data assimilation and list applications where it might be useful

</details> 

<details>
<summary>3. Design, build, and evaluate functional numerical models of some common physical processes</summary>

  * Describe the difference between a boundary and initial value problem
  * Define and distinguish between a flux and level boundary condition
  * Define initial condition
  * Define boundary condition
  * Explain the principles underlying chaos or sensitive dependence to initial conditions
  * List several processes that could be approximated as a diffusive process
  * Create a model that solves the diffusion equation
  * List several processes that could be approximated as an advection process
  * Create a model that solves the advection equation
  * List several processes that could be approximated as an advection-dispersion process
  * Create a model that solves the advection-dispersion equation
  * Describe the purpose of surrogate modeling/emulation with machine learning methods

</details> 

<details>
<summary>4. Develop and use effective scientific software development tools and habits</summary>

  * Create a jupyter notebook to demonstrate a modeling workflow
  * Use a version control system to track changes in source code
  * Use GitHub to submit an assignment as a Jupyter notebook
 
</details> 
 
<details>
<summary>5. Examine and report on key facets of an existing model of a system or process of interest</summary>

  * Find an existing model of an Earth/Environmental System and identify key details
  * Classify the kind of Earth/Environmental model in terms of it's relation to underlying processes
  * Describe how a particular model represents underlying processes
  * List specific data sources and repositories where input data for a selected model can be found
  * Design a numerical experiment to test a hypothesis
  * List where to obtain data required as input to a selected model
 
</details> 

---

## Grading Rubrics

Below are the grading rubrics for the Jupyter notebook assignments, module-end reflections, and modeling term project are provided below. Although each of these assessments are associated with point totals, the total points will be re-weighted at the end of the semester to compute your final grade in the proportions listed above in the __Grading Summary__ section. 

### Programming Assignments

<table>
  <thead>
    <tr>
      <th>Criteria</th>
      <th colspan="6">Ratings</th>
      <th>Points</th>
    </tr>
  </thead>
  <tbody> 
    <tr>
      <td valign="top"><b>Completeness:</b><br>Describes the extent to which the assignment answered the questions in the assignment.</td> 
      <td valign="top"><b>25 pts<br>Complete</b><br>Submission answered all questions.</td> 
      <td valign="top"><b>20 pts<br>Almost Complete</b><br>Submission answered ≥90% of questions assigned.</td>
      <td valign="top"><b>15 pts<br>Substantially Incomplete</b><br>Submission answered ≥70% of questions assigned.</td>
      <td valign="top"><b>10 pts<br>Incomplete</b><br>Submission answered <70% of questions assigned.</td>
      <td valign="top"><b>5 pts<br>No Submission w/Notice</b><br>Student notified instructors of a non-submission 48hrs in advance of due date.</td>
      <td valign="top"><b>0 pts<br>No Submission</b></td>
      <td valign="top">25 pts</td>
    </tr>
    <tr>
      <td align="right" colspan="8"><b>Total Points: 50</b></td>
    </tr>
  </tbody>
</table>

### Module-end Reflection

<table>
  <thead>
    <tr>
      <th>Criteria</th>
      <th colspan="6">Ratings</th>
      <th>Points</th>
    </tr>
  </thead>
  <tbody> 
    <tr>
      <td valign="top"><b>Content</b><br></td> 
      <td valign="top"><b>50 pts<br>Excellent</b><br>Reflection is thoughtful and answers all prompts.</td> 
      <td valign="top"><b>40 pts<br>Very Good</b><br>Reflection is thoughtful and answers almost all prompts.</td>
      <td valign="top"><b>30 pts<br>Good</b><br>Reflection may be cursory and may not address one or more prompts.</td>
      <td valign="top"><b>20 pts<br>Fair</b><br>Reflection is cursory, but in full sentences, and does not address prompts.</td>
      <td valign="top"><b>10 pts<br>Poor</b><br>Reflection is incomplete and not in complete sentences.</td>
      <td valign="top"><b>0 pts<br>Not Submitted</b>Reflection not completed</td>
      <td valign="top">50 pts</td>
    </tr>
    <tr>
      <td align="right" colspan="8"><b>Total Points: 50</b></td>
    </tr>
  </tbody>
</table>

### Modeling Term Project

<table>
  <thead>
    <tr>
      <th>Criteria</th>
      <th colspan="5">Ratings</th>
      <th>Points</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td valign="top"><b>Introduction</b></td> 
      <td valign="top"><b>20 pts<br>Excellent</b><br>Describes the scientific or engineering modeling challenge concisely. The challenge described is contemporarily relevant. References includes are relevant, contemporary, and appropriate.</td>
      <td valign="top"><b>15 pts<br>Very Good</b><br>Describes the scientific or engineering modeling challenge concisely. The challenge described is relevant. References includes are relevant and appropriate.</td>
      <td valign="top"><b>10 pts<br>Good</b><br>Describes the scientific or engineering modeling challenge. There may be some mismatch between the challenge and the model relevance. May be poorly referenced.</td>
      <td valign="top"><b>5 pts<br>Fair</b><br>Scientific or engineering modeling challenge is poorly describe, not relevant, or not contemporary. References are either inappropriate to the problem or not included.</td>
      <td valign="top"><b>0 pts<br>Poor</b>It is not clear that what is submitted is an introduction</td>
      <td valign="top">20 pts</td>
    </tr>
    <tr>
      <td valign="top"><b>Model Description</b></td> 
      <td valign="top"><b>20 pts<br>Excellent</b><br>Description of model is concise, accurate, and clearly linked to processes. Uses of the model for similar applications are described and referenced. A conceptual figure is present and appropriately cited.</td>
      <td valign="top"><b>15 pts<br>Very Good</b><br>Description of model is concise, accurate, and clearly linked to processes. Uses of the model for similar applications may be absent. A conceptual figure is missing or not cited.</td>
      <td valign="top"><b>10 pts<br>Good</b><br>Model may not be described concisely, accurately, or linked to processes. Uses of the model for similar applications are missing. No conceptual figure.</td>
      <td valign="top"><b>5 pts<br>Fair</b><br>Model is not described in ways that clearly link it to scientific application.</td>
      <td valign="top"><b>0 pts<br>Poor</b>Model description is missing.</td>
      <td valign="top">20 pts</td>
    </tr>
    <tr>
      <td valign="top"><b>Data Needs</b></td> 
      <td valign="top"><b>20 pts<br>Excellent</b><br>Needs for input data and description of output data format are clearly described in terms of format and type. Appropriate sources of input datasets are provided.</td>
      <td valign="top"><b>15 pts<br>Very Good</b><br>Input data needs and output data are clearly described in terms of format and type. Appropriate sources of input datasets may be missing.</td>
      <td valign="top"><b>10 pts<br>Good</b><br>Input data needs and output data are described, but may be unclear. Appropriate sources of input datasets are missing.</td>
      <td valign="top"><b>5 pts<br>Fair</b><br>Input data needs and output data are unclear or missing in parts. Appropriate sources of input datasets are missing.</td>
      <td valign="top"><b>0 pts<br>Poor</b>Data needs not specified.</td>
      <td valign="top">20 pts</td>
    </tr>
    <tr>
      <td valign="top"><b>Calibration</b></td> 
      <td valign="top"><b>20 pts<br>Excellent</b><br>Variables requiring calibration that are appropriate to the problem identified. Target variables and observational datasets are identified. Prior appropriate calibration studies are referenced.</td>
      <td valign="top"><b>15 pts<br>Very Good</b><br>Variables requiring calibration that are appropriate to the problem identified. Target variables and observational datasets are identified.</td>
      <td valign="top"><b>10 pts<br>Good</b><br>Variables requiring calibration that are appropriate to the problem identified. Target variables are identified. Observational datasets used in calibration not identified.</td>
      <td valign="top"><b>5 pts<br>Fair</b><br>Variables requiring calibration are identified but are not appropriate to the problem. Target variables and observational datasets not identified or inappropriate.</td>
      <td valign="top"><b>0 pts<br>Poor</b>Calibration of model not discussed or most details absent.</td>
      <td valign="top">20 pts</td>
    </tr>  
    <tr>
      <td valign="top"><b>Numerical Experiment Design</b></td> 
      <td valign="top"><b>20 pts<br>Excellent</b><br>Numerical experiment is well designed, appropriate to the problem, and its rationale described. The experiment may extend other, referenced studies.</td>
      <td valign="top"><b>15 pts<br>Very Good</b><br>Numerical experiment is well designed, appropriate to the problem, although its rationale may be lacking. The experiment may extend other, unreferenced studies.</td>
      <td valign="top"><b>10 pts<br>Good</b><br>Numerical experiment design is unclear or appears unconnected to the problem, Rationale may be unclear.</td>
      <td valign="top"><b>5 pts<br>Fair</b><br>Numerical experiment design is poorly designed and unconnected to the problem, Rationale is missing.</td>
      <td valign="top"><b>0 pts<br>Poor</b>Numerical experiment design is missing.</td>
      <td valign="top">20 pts</td>
    </tr>
    <tr>
      <td align="right" colspan="7"><b>Total Points:100</b></td>
    </tr>
  </tbody>
</table>
