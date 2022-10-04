### <em>IU000135 PERSONLIZATION AND MACHINE LEARNING</em>
# Exploring Course Recommendation Systems for Educational Platforms
##### by Yifan Feng, MA/MSc Computing and Creative Industry (modular)

## Project Overview
Inspired by Assignment 2 of designing a university program recommendation system, this project explores two different approaches (i.e., content-based and collaborative filtering methods) of constructing recommenders. The initial idea was to provide course recommendations for fresh students to register study units (electives). Due to the limitation of chosen dataset’s data structure (see report), target audience were narrowed down to: 
1. New students who want to specialise in one academic field and deepen their knowledge through similar knowledge training 
2. Registered students look for potential study buddies based on similar study interest 
 
## Dataset
This project utilizes open data source provided by Kaggle.com and HavardX. 

Repository  | Link 
------------| -------------
Kaggle      | [Online MOOC](https://www.kaggle.com/datasets/ayushbatra/online-mooc)
Kaggle      | [EdX Courses Dataset 2021](https://www.kaggle.com/datasets/khusheekapoor/edx-courses-dataset-2021)
HavardX     | [HarvardX Person-Course Academic Year 2013 De-Identified dataset](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/26147)

## Course Recommendation Model
* For technical component, please see [Mini-Project.ipynb](https://git.arts.ac.uk/21036265/Personalization_miniproject/blob/main/project_YifanFENG.ipynb).
* For writing component, please read [Mini-Project Report](https://git.arts.ac.uk/21036265/Personalization_miniproject/blob/main/mini_project/miniproject_report.pdf). 

### Main Reference
Coding section is mainly developed from teaching materials provided in class. 
* [Week 1.2 Similarity Based Matrix](https://git.arts.ac.uk/lmccallum/personalisation-21-22/blob/master/Week%201.2%20-%20Similarity%20Based%20Filtering%20.ipynb)
* [Week 3.1 Collaborative Filtering](https://git.arts.ac.uk/lmccallum/personalisation-21-22/blob/master/Week%203.1%20Collaborative%20Filtering.ipynb)

Previous research on optimizing course recommendation system includes: 
Author                      | Paper 
--------------------------  | -------------
Adilaksa and Musdholifah (2021)| [A Collaborative Recommendation System for Online Courses Recommendations](https://ieeexplore.ieee.org/abstract/document/8876926)
Ma et al. (2017)             | [Course recommendation based on semantic similarity analysis](https://ieeexplore.ieee.org/document/8088011)
Obeidat et al. (2019)       | [A Collaborative Recommendation System for Online Courses Recommendations](https://ieeexplore.ieee.org/abstract/document/8876926)
Pan et al. (2021)           | [Application of Collaborative Filtering Recommendation Algorithm in Internet Online Courses](https://dl.acm.org/doi/10.1145/3469968.3469992)
Yin et al. (2020)           | [A MOOC Courses Recommendation System Based on Learning Behaviours](https://dl.acm.org/doi/10.1145/3393527.3393550)

<img src="https://github.com/Yifan-FENG/personalization-ual/blob/main/mini_project/model/model1.jpg" height="750" width="350"> <img src="https://github.com/Yifan-FENG/personalization-ual/blob/main/mini_project/model/model2.jpg" height="750" width="350">


## Main Takeaway
1. Content-based recommendation is more suitable for course recommendation algorithms. This approach has the strength when new courses (no historical review) need to be promoted. 
2. For university use, course recommendation should consider student history of study marks when computing weights for course similarity. However, collaborative-filtering based on grade clusters might not be the best method as it limits students who want to achieve a higher score and do not want to be defined by previous academic performance. 
3. For commercial platforms, hybrid application might be the best recommendation approach. That said, as hybrid system includes both advantages and disadvantages of content-based and collaborative-filtering methods, a situation of “over parameterization” (e.g., process a large quantity of metadata) might occur.  
4. Overall, there is no perfect model for course recommendation. Many subjective factors such as practicality, interest, goal, grade, teacher reputation are involved when determining a course. 
