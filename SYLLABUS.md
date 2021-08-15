# Syllabus<br>GEOS 518: Modeling Earth and Environmental Systems (Fall 2021)

--- 

### Instructor:
Dr. Alejandro (Lejo) Flores (he/him)  
Phone: 208.426.2903  
Office Hours: (via Zoom: see Canvas for link)  
Email: [lejoflores@boisestate.edu](lejoflores@boisestate.edu)  

### Teaching Assistant:
William Rudisill (he/him)  
Office Hours: (via Zoom: see Canvas for link)  
Email: [williamrudisill@u.boisestate.edu](williamrudisill@u.boisestate.edu)  

---

### Course Description:


### Required Textbook:
The following textbook is required for the class. It is fairly easy to find and reasonably priced: 

_Slingerland, Rudy and Kump, Lee_ (2011), Mathematical Modeling of Earth's Dynamical Systems: A Primer, Princeton University Press, 248 pp. | [Buy on Bookstore.org](https://bookshop.org/books/mathematical-modeling-of-earth-s-dynamical-systems-a-primer/9780691145143) | [Buy on Amazon.com](https://www.amazon.com/Mathematical-Modeling-Earths-Dynamical-Systems/dp/0691145148) | 

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

__A note on Integrated Development Environments (IDEs).__ Some students, particularly those having familiarity with Matlab, will find IDEs helpful to aid in the transition from Matlab to Python. A number of IDEs are available for development in Python, some of which come bundled with installers like `Anaconda`. These can be helpful in providing an experience that is familiar but, in my experience, can often lead users to develop less-than-helpful habits as scientific programmers. We will using primarily Jupyter notebooks, which allow you to program and intersperse blocks of code with descriptive text and are used exclusively in a browsered environment. Please try to stick with the Jupyter notebook computing environment (you will be required to submit assignments as Jupyter notebooks), even though it may seem a bit foreign at first. 

### Course Expectations:
This class has a mixed structure wherein the Tuesday class will be primarily lecture and the Thursday class with be a coding workshop. In the Thursday coding lab we will review example code that I have developed for each topic we cover in the class. Depending on how well you are able to understand, execute, and modify the example code you may also have time to get started on the associated assignment for each module.  

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

### COVID-19 Guidelines:
As of August 2021, the COVID-19 pandemic situation is evolving rapidly in the United States and Idaho. 


---

### Grading Summary (proportions may vary by up to 5%)

| Component | Proportion of Grade |
| --- | --- |
| Online Reading Quizzes | 15% |
| Jupyter Notebook Assignments | 60% |
| Module-end Reflection | 5% |
| Modeling Project | 20% |

#### Online Reading Quizzes (15%)
Quizzes are designed as a formative assessment to check how well you understand the required reading. Reading ensures that we're starting out from a common starting point when you come to lecture. As much as it is important to read materials to acquire new knowledge and skills, it is just as important to identify topics and concepts that are still uncertain after reading. Those concepts that remain difficult to you after reading are likely difficult for other students and, therefore, opportunities for diving deeper as a class and exploring through activities and exercises. Each quiz is 10 questions and you may take each quiz twice. The recorded score will always be the final score (i.e., not the highest - think about whether you really want to retake the quiz to get 1 additional point). Quizzes are open-book but not collaborative. You are responsible for checking the schedule on Canvas and keeping up with deadlines. Make sure you are using a reliable Internet connection. Your lowest quiz score will be dropped before final grades are calculated.  

#### Jupyter Notebook Assignments (60%)
The most significant part of your grade will be based on programming assignments in which you will use and/or build simple models of environmental processes and use them to explore topics being covered in the class. There will be one assignment for each module of the class (there are approximately 9 modules) and the assignments will be complete when you post them as a Jupyter Notebook (`.ipynb` extension) on your own GitHub account and submit the link to the notebook on Canvas. For those unfamiliar with Jupyter and GitHub, we will provide a number of resources to help you get familiar and up and running with them. Generally you will clone a template assignment notebook from the class repository into a GitHub repository of your choice. That template will have instructions (and potentially some code) that is designed to lead you through the notebook assignment. __Note:__ Once you complete this class, you _could_ have a GitHub repository with all your submitted Jupyter notebooks for the class that can serve to illustrate your computational skills to potential employers.  

#### Module-end Reflection (5%)
At the end of each module of the class (there are approximately 9 modules) there is a short reflection that you will be required to complete. The reflection takes the form of 3 questions to which you will respond in Canvas. The reflection is designed as a prompt to pause, actively reflect on things like what you learned/struggled with/improved on during the module activities (e.g., reading, lecture, assignments, etc.) and record them. If you invest in them, these reflections can be invaluable tools for you to assess your own learning progress and ensure that you are getting what you need/want out of the class. Responses to reflection prompts need not be long, but should be thoughtful and authentic.   

#### Modeling Project (20%)
You will also have a modeling project for the class. The purpose of this modeling project is for you to explore an existing model of interest to your professional development and/or research. During this project you will: (1) select a model for further study, (2) examine key details of the Earth and environmental processes that it models in the context of topics we cover in the class, (3) review the data needed to characterize initial and boundary conditions for the model, (4) investigate procedures and data needs for calibration/validation, and (5) design a numerical experiment to test a scientific hypothesis or perform a specific analysis. ___You will not need to setup, run, or perform your numerical experiment as a requirement of the project.___ However, this project could be a valuable tool to kickstart any modeling activities required for your thesis or dissertation. As such, I ___highly___ encourage you to consult with your advisor(s) and me when choosing a model. This project will be submitted as a Markdown (e.g., `PROJECT.md`) file in your GitHub repository for the class.   

--- 

### Course Learning Outcomes
At the end of this class, you will be able to:

<details>
<summary>1. Explain key steps and considerations in the choice and use of a numerical model for a scientific/engineering application</summary>
 
 1.1 Differentiate between statistical and dynamical models
 1.2 List different applications for which a model is used 
 1.3 Explain the concept of parsimony in the context of modeling
 1.4 Define a conceptual model in terms of how it represents underlying processes
 
</details> 
2. Describe the necessity, process, and methods of model evaluation and calibration
3. Design, build, and evaluate functional numerical models of some common physical processes 
4. Develop and use effective scientific software development tools and habits
5. Examine and report on key facets of an existing model of a system or process of interest

