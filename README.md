# Course-GPT
A Deep-Learning based Course Recommendation System that recommends Courses based on the prompts given by the user.
### Problem Statement
* Traditionally for a Course Recommendation, A User Enters the Topic he is interested in and the system recommends a course which is more relevant to the topic entered by the user.
* This is fine when the user is sure about the Topic he wants to learn but for the users who are unsure of the topic they want to choose, this method become inefficient.
* The User should be able to give a detailed description / His Profile (usually a Bio/Resume) to the system to get recommendations. 
### Proposed Method:
* To tackle the discussed problem, We suggest using a recommendation system where the user can come in and type his interest and what type of course he is looking for and his expected outcomes from the course.
* Based on the detailed Description, we Intent to analyze the likeliness between the user’s description and the Course Descriptions and other parameters of the available courses to suggest the most relevant course to the user.
### Basic Working:
* Pre-process the Course Descriptions to remove stop-words and other irrelvent information and then create Word Embeddings of the Course Descriptions using the Pre-trained BERT model from Google/
* Once the user enters the prompt, pre-process the prompt and create a Word Embeddings of the prompt using the Pre-trained BERT model from Google.
* Find the Cosine Similarity between the prompt and course Description to recommend the most-relevent courses
