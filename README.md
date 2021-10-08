# Machine Learning Project Proposal: Breast Cancer Cell Detection
CS 4641 Group 22 -  Sanjana Balusu, Ritvik Bhagawatula, Roshni Dhanasekar, Rohan Kashi, and Paula Punmaneeluk

Introduction/Problem Definition
Breast cancer occurs when abnormal breast cells grow and divide at a more rapid rate than healthy cells. Our goal for this project is to predict whether a set of cells is benign or malignant based on specific cell features. This would allow us to diagnose whether breast cancer is present or not. We will produce a predictive model that utilizes supervised learning to accomplish this goal. During this semester, we will analyze which features of cells have the greatest impact in determining whether that cell is cancerous. 

Data
Source: https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)

Below, we have listed the cell features that we will be looking at in more detail:
<img width="414" alt="Screen Shot 2021-10-08 at 12 31 53 AM" src="https://user-images.githubusercontent.com/63989199/136498703-d7e5449e-1b7f-4517-a43f-1b4f07baf10f.png">





Methods
Our team wants to train a binary classification model to determine whether a cell’s nucleus is either malignant or benign. Subsequent to training the resulting model using the Breast Cancer Wisconsin dataset, it will be able to predict whether a given cell’s nucleus is cancerous based on the ten real-valued attributes noted above. Doing so will allow us to analyze the error between the actual malignancy of the nucleus and the final trained model’s prediction.

Our model employs a binary dependent variable since it produces one of two possible responses. Therefore, applying logistic regression would be the appropriate method as it allows for two arbitrary parameters to determine the probability of an event based on our predictor variables. This technique uses the sigmoid function to output the probability of an event, so in our case:

         p(x)<0.5, Y= 0/benign

         p(x)>0.5, Y= 1/malignant
         
where x represents our dataset’s ten discrete attributes.

An additional predictive technique we can use is decision trees. Because we’re training a binary classification model, we would ultimately evaluate a binary classification tree that utilizes our ten attributes and similarly outputs one of two responses, “yes” or “no”.

Potential Results

<img width="630" alt="Screen Shot 2021-10-08 at 12 31 42 AM" src="https://user-images.githubusercontent.com/63989199/136498717-e619b3c1-8bce-4ac3-90db-21c4c90c189f.png">


Above is an example of what our results could look like. We use a logistic regression curve, where the probability of being malignant is on the vertical axis. On the horizontal axis, we have the number of features in the cell that are present. The sigmoid function determines where each datapoint falls. As we can see, the more cell features from our set are present, the higher probability we have for the cell being malignant.  
 
Another way to graph the results is by using a decision tree. For each node in the tree, we will have a feature and it will point to a new feature until we reach the decision. To determine the accuracy of the predictions, you must divide the accurate predictions by the total predictions. For the independent variables, we plug in different values and see which model has the highest accuracy.

Discussion:
There are several different combinations we can have with the ten cell attributes we highlighted. Each of them can have different values that change the probability of the cell being malignant. By having an accurate model that reflects which cell attributes lead to the highest chance of the cell being malignant, we can better diagnose patients. The advantage of accurate diagnosis is that it allows us to detect breast cancer early and lead to the highest chance of remission. 

Proposed Timeline:
<img width="630" alt="Screen Shot 2021-10-08 at 12 31 32 AM" src="https://user-images.githubusercontent.com/63989199/136498727-e2f029a0-3799-46c4-b55e-d564fb95932c.png">


Member Responsibilities:

Everyone will be a developer i.e. contribute equally to coding our project.

Sanjana Balusu 
scribe - takes notes on ideas mentioned during meetings
Ritvik Bhagawatula 
editor - runs the final check through project submissions
Roshni Dhanasekar 
scheduler - organizes meeting time and plans topics to be discussed
Rohan Kashiviswanathan 
submitter - ensures that all deadlines are met on time 
Paula Punmaneeluk 
facilitator - initiates discussion to hear everyone’s ideas


Peer-reviewed sources:
https://www.sciencedirect.com/science/article/pii/S1470204500002540 https://jamanetwork.com/journals/jama/article-abstract/200479 https://www.bmj.com/content/321/7263/745.short 

Other sources:
https://www.nationalbreastcancer.org/breast-cancer-facts
https://www.mayoclinic.org/diseases-conditions/breast-cancer/symptoms-causes/syc-20352470
https://www.breastcancer.org/symptoms/understand_bc/statistics
https://www.breastcancer.org/symptoms/types/recur_metast

