**Description:**

The collected dataset is from a second year undergraduate Science course offered at a North American University. The dataset consists of the obtained grades of the 486 enrolled students in the different assignments, quizzes, and exams. The dataset contains a total of 9 features as per the table below:

|Feature|	Description|	Type |	Value/s |
|:--- |:--- |:--- |:---|
|Student Id	| Student identifier |	Nominal |	std000, …, std485|
|Quiz01|	Quiz1 Mark	| Numeric |	0,…,100 |
| Assign.01|	Assign.01 Mark|	Numeric|	0,…,100|
|Midterm|	Midterm Mark|	Numeric|	0,…,100|
|Assign.02|	Assign.02 Mark|	Numeric|	0,…,100|
|Assign.03|	Assign.03 Mark|	Numeric|	0,…,100|
|Final Exam|	Final Exam Mark|	Numeric|	0,…,100|
|Final Grade|	Total Final Mark|	Numeric|	0,…,100|
|Student Category|	Final Grade|	Nominal|	G,W|

Any empty mark was replaced with 0. Also, all features were converted to a mark out of 100 to improve the accuracy of any classifier used. Any mark that consists of decimal point number was rounded to the nearest 1. The total course mark was counted out of 110 with the additional 10% being added to assignment 03’s grade as curving to help students in the course’s final grade. Note that due to the recent adoption of the “General Data Protection Regulation” which introduced many restrictions on the collection of data, and to maintain the privacy of users, the contents of the different tasks/features could not be accessed. As such, these tasks/features could not be categorized as per their cognitive objectives using Bloom’s taxonomy. The final grade was classified into two categories (classes):
-	Good (G) — the student will finish the course with a good grade (60-100)
-	Weak (W) — the student will finish the course with a weak grade (≤ 59). This limit was chosen since the typical passing grade for undergraduate course is often set to 60 in most universities.
The target group is the Weak students (W) who are predicted to receive a mark below 60%, meaning that they are at risk of failing the course. This dataset was used as part of a comparative analysis work completed to predict student’s performance at earlier stages of the course delivery using machine learning models. The developed models use ensemble classification techniques to categorize the students and predict their final performance group/category. Different techniques were used individually or as a part of an ensemble learner model to predict the final performance group during the course at two stages — at 20% and 50% of the coursework. 

**Contact information:**

Please feel free to contact me for any questions or cooperation opportunities. I'd be happy to help.
Email: minjadat@uwo.ca

**Citation:**

If you find this dataset useful in your research, please cite this article as:
M. Injadat, A. Moubayed, A. B. Nassif, and A. Shami, “Systematic ensemble model selection approach for educational data mining,” Knowledge-based Systems, vol. 200, p. 105992, Jul. 2020.

Link: https://www.sciencedirect.com/science/article/abs/pii/S0950705120302999

Arxiv link: https://arxiv.org/abs/2005.06647

@article{injadat2020systematic,
   author={M. {Injadat} and A. {Moubayed} and A. B. {Nassif} and A. {Shami}},
   
   journal={Knowledge-based Systems},
   
   title={{Systematic ensemble model selection approach for educational data mining}},
   
   year={2020},
   
   volume={200},
   
   pages={105992},
   
   issn = {0950-7051},
   
   doi={10.1016/j.knosys.2020.105992},
   
   month={Jul.}, 
   
   publisher={Elsevier}}
