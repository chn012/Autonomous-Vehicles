# Autonomous Vehicle Trajectory Prediction 

#### With traffic scene data from Argoverse, train various machine learning models to predict a vehicle's trajectory in the following 3 seconds.

The task of our project is to predict the positions of a tracked object 3 second into the future, given an initial 2-second observation. This is also a regression task since we are dealing with continuous inputs and outputs. It is important because our loss function depends on what task we are dealing with. In our case, since we want to minimize the distance between the prediction and the grand truth, root mean squared error would be the best choice. The ability to plan, conditioned on the future states of dynamic agents in complex roadway environments is a central challenge to the safe and efficient operation of autonomous vehicles. 

This task is important in real world application since progress on the motion prediction problem has downstream consequences for the deployment timeline, scale, and performance of autonomous vehicles as paratransit, long-haul freight, and local delivery options. The most direct application of this in real life is in terms of autonomous vehicles like Tesla's proposed consumer complete self-driving car or autonomous freight vehicles transporting goods, but the  application doesn't have to remain only in terms of autonomous vehicles. For just one example, building on this, we could do prediction of future weather given current weather information. 

After training and comparing different models, our best performing model was a single layer encoder decode LSTM model with a RMSE of 2.25084.



https://user-images.githubusercontent.com/59916633/142205197-1d19a5dd-fba9-4de7-9c7d-8bc0d27392e4.mp4



For further detail, read the full report at Autonomous_Vehicle_Report.pdf.

