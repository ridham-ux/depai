Developing and deploying a Machine Laerning Application using Docker

Objective:
The objective of this assignment is to develop a simple machine learning application, containerize it using Docker, and deploy it on GitHub. 
This exercise will help you understand the principles of containerization, version control, and basic machine learning application development.


Prerequisites
•	Basic understanding of Python programming
•	Basic understanding of machine learning concepts
•	Familiarity with Git and GitHub
•	Basic knowledge of Docker


Building and running the docker congtainer:
1. Creating a project directory  for the project and creating a dockerfile. All the required content mentioned in the dockerfile present in the repository.
2. Creating a requirements.txt specifying the requirements that need to be installed in the docker container.
3. Create a script train_model.py to train a simple machine learning model and save it. For simplicity, I have use the Iris Dataset and a decision tree classifier. Script is present in the repository.
4. Run the model script to generate model.pkl
5. Integrating the model into the flask app using app.py file. Code present in the repository.
6. Run the docker build command to build the docker container and run the docker container.


To test the ML endpoint:
1.After running the docker container try to access the container via browser and navigate to https://localhost:4000 to see the running application.
2. Test the ML endpoint using curl or postman by sending a POST request with JSON data. Use the following command:
curl -X POST http://localhost:4000/predict -H "Content-Type: application/json" -d'{"input":[5.1, 3.5, 1.4, 0.2]}'


   
