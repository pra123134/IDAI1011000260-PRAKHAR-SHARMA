README for Pose Recognition
By Prakhar Sharma
Project Overview
This project involves leveraging Google’s Teachable Machine to create an intelligent model capable of classifying various workout poses, such as push-ups, squats, and lunges. This model lays the groundwork for a future virtual fitness trainer app that provides live feedback and correction during workouts. By experimenting with pose recognition, helped me gain practical experience in training AI models and exploring their real-world applications.
Data Collection and Preparation
Process of Data Collection:
Selecting Pose Types: I focused on collecting data for three main workout poses: push-ups, squats, and lunges.
Recording Data:
Personal Recordings: I recorded individuals performing the poses in different environments and from multiple angles. This helped capture variations in lighting, background, and user posture.
Online Sources: Supplementary images were sourced from google.com, youtube and online videos to diversify the dataset.
Data Diversity:
Capturing data from multiple angles and individuals enhanced the model’s ability to generalize and improved its accuracy.
Including a variety of user body types and exercise styles ensured the model could recognize the poses reliably across different scenarios.
Data Preparation:
Labeling: Each recorded clip or image was accurately labeled as either “PushUp,” “Squat,” or “Lunge.”
Balancing the Dataset: Initially I started with 100 images, but the results were not very correct , so in creased my dataset to Squat- 241, Lounges-273, pushup-234. But this model was biased towards lunges , then I realised that the number of data samples should be equal to avoid bias. This ensured that each class (pose type) had an approximately equal number of samples to avoid bias.
Preprocessing: Data was checked for quality, removing unclear or low-resolution images that could reduce the model’s effectiveness.
Creating the Model with Google’s Teachable Machine
Step-by-Step Process:
Project Setup:
Accessed Google’s Teachable Machine.
Selected the “Pose” project type.
Uploading Data:
Uploaded recorded images and videos into the platform.
Organized data into three categories for the respective workout poses.
Training:
Configured training parameters to allow the model to learn efficiently.
Trained the model using Teachable Machine’s built-in training feature.
Model Refinement:
I started with 100 images, but the model was not crude , so I added more pictures and videos with different  backgrounds. Performed iterative training runs, adjusting data input as needed to optimize accuracy.
Model Features and Functionalities
Pose Classification: The model can classify and distinguish between push-ups, squats, and lunges with high accuracy.
Feedback Potential: While basic, this model sets the stage for future development into a real-time application capable of providing feedback and corrections on form.
Evaluation of Model Performance
Methods Used:
Cross-Validation:
Split the dataset into training and testing sets. (tested data with video, web camera capture and different images)
Evaluated the model using unseen test data to verify accuracy and generalization.
Accuracy Metrics:
Analyzed accuracy, precision, and recall scores to ensure balanced performance across all classes. Tested with 10 different data test, out of which
Position  Correct identification   Incorrect identification
Squat      5  (avg 70%)             5 (avg 50%)
Lunges     9(avg 95%)               1(10%)
Pushup     10( 90%)                 0

 
Real-World Testing:
Ran the model in various environments to test its robustness against different backgrounds and lighting conditions.
Results:
The model achieved an overall accuracy of approximately 80%, with minor variations based on pose complexity and angle of recording. Many pictures which did not have any of the 3 poses were still identified as squat, this can be corrected by fine tuning and adding classes like notSquat etc.
The inclusion of diverse data samples contributed to the model’s ability to generalize well in different real-world scenarios.
Practical Applications
Real-World Problem Solving:
Fitness Training: The model can be integrated into a virtual fitness app to help users track their workouts and improve form.
Physical Therapy: This tool could assist therapists in remotely monitoring patients’ exercises and progress.
Home Workouts: Users without access to a personal trainer can benefit from real-time pose classification and feedback to ensure correct form.








