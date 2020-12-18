**Description:**

The collected dataset is from a second year undergraduate Science course offered at a North American University that was given in a blended format (i.e. course had both a face-to-face component and online component). The raw dataset consists of an event log of 486 enrolled students and has a total of 305933 records collected from the university’s learning management system (LMS), namely OWL. Each record consists of the following six fields:

-	Event Date: The timestamp of the event.
-	Event Type: The action the student takes.
-	Event Location: The directory in which the action was taken by the student.
-	Session Start: The timestamp representing the start of the online session.
-	Session End: The timestamp representing the end of the online session.
-	Student ID: Student identifier to group the event log based on.

Resources and assignments are posted sequentially throughout the course. Moreover, the average duration between assignment posting and assignment due date was approximately 2 weeks. The dataset was sorted based on the “Student ID” first and then based on “Event Date”. This was done so that a chronological order of the events each student took is obtained. Note that due to the “General Data Protection Regulation”, which introduced many restrictions on data collection, and to maintain the privacy of users, the contents of the raw dataset cannot be shared. 
The raw dataset was transformed from its original state into a new dataset representing the desired engagement metrics. This was done by searching the events’ column of the subset of data representing each student and calculating the desired metrics. Based on the engagement metrics used in the literature and the original available dataset, the table below presents the newly calculated desired metrics as well as their description, type, and range of values. 

|Feature|	Engagement Metric Type|	Description|	Type|	Value/s|
|:---|:---|:---|:---|:---|
|Student Id|	|	Student identifier|	Nominal|	std000, …, std485|
|Number of Logins|	Interaction|	Number of times student accessed the course site on the LMS|	Numeric|	0, …, 647|
|Number of Content Reads|	Interaction|	Number of times student accessed course material|	Numeric|	0, …, 1007| 
|Number of Forum Reads|	Interaction |	Number of times student read posts on the discussion forum|	Numeric|	0, …, 58|
|Number of Forum Posts|	Interaction|	Number of times student posted on the discussion forum|	Numeric|	0, …, 6|
|Number of Quiz Reviews|	Interaction|	Number of times student reviewed their quiz solution before final submission|	Numeric|	0, …, 12|
|Assignment 1 lateness indicator|	Effort| A binary indicator stating whether Assignment 1 submission is late or not|	Numeric|	0,1|
|Assignment 2 lateness indicator|	Effort|	A binary indicator stating whether Assignment 2 submission is late or not|	Numeric|	0,1|
|Assignment 3 lateness indicator|	Effort|	A binary indicator stating whether Assignment 3 submission is late or not|	Numeric|	0,1|
|Assignment 1 duration to submit (in hours)|	Effort|	The duration (in hours) between Assignment 1 posting and submission|	Numeric|	0, …, 583|
|Assignment 2 duration to submit (in hours)|	Effort|	The duration (in hours) between Assignment 2 posting and submission|	Numeric|	0, …, 297|
|Assignment 3 duration to submit (in hours)|	Effort|	The duration (in hours) between Assignment 3 posting and submission|	Numeric|	0, …, 632|
|Average Assignment duration to submit (in hours)|	Effort|	The average duration (in hours) between Assignments’ posting and submission|	Numeric|	0, …, 496|
|Engagement Level| | Student engagement level determined by K-means Clustering|	Nominal|	L, H|

The engagement metrics were chosen based on the available data through the log files in such a manner so as to extract the maximum amount of information. For example, the course had three assignments, one quiz, one midterm exam, and one final exam. That is why the duration needed to submit each assignment was considered as a feature along with the average assignment submission time was extracted from the data.

**Contact information:**

Please feel free to contact me for any questions or cooperation opportunities. I'd be happy to help.

Email: amoubaye@uwo.ca

**Citation:**

If you find this dataset useful in your research, please cite this article as:

a.	A. Moubayed, M. Injadat, A. B. Nassif, H. Lutfiyya and A. Shami, "E-Learning: Challenges and Research Opportunities Using Machine Learning & Data Analytics," in IEEE Access, vol. 6, pp. 39117-39138, 2018.

Link: https://ieeexplore.ieee.org/document/8417405

b.	Moubayed, M. Injadat, A. Shami, and H. Lutfiyya, “Student Engagement Level in an e-Learning Environment: Clustering Using K-means”, American Journal of Distance Education, 34:2, pp. 137-156, Mar. 2020

Link: https://www.tandfonline.com/doi/abs/10.1080/08923647.2020.1696140


@article{Moubayed2018access,
  author={A. {Moubayed} and M. {Injadat} and A. B. {Nassif} and H. {Lutfiyya} and A. {Shami}},
  journal={IEEE Access}, 
  title={E-Learning: Challenges and Research Opportunities Using Machine Learning   Data Analytics}, 
  year={2018},
  volume={6},
  pages={39117-39138},
  doi={10.1109/ACCESS.2018.2851790}}

and

@article{Moubayed2020Kmeans,
   author = {A. {Moubayed} and M. {Injadat} and A. {Shami} and H. {Lutfiyya}},
   title = {Student Engagement Level in an e-Learning Environment: Clustering Using K-means},
   journal = {American Journal of Distance Education},
   volume = {34},
   number = {2},
   pages = {137-156},
   year  = {2020},
   publisher = {Routledge},
   doi = {10.1080/08923647.2020.1696140},	
}
