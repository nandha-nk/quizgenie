![image](https://github.com/user-attachments/assets/cb71dd2b-fe0b-42a1-9dc1-d7c0d19111c3)# quizgenie
This project presents an AI-powered quiz generation platform with dynamic retesting functionalities, aiming to personalize assessments and enhance learning experiences. Instructors upload learning materials (text documents and images) and configure quizzes by selecting difficulty level and number of questions.
Leveraging Large Language Models (LLMs):
The platform integrates with an LLM API specifically designed for fast inference, such as Groq ,to generate unique questions tailored to the uploaded content.
The instructor's chosen difficulty level is incorporated into the Groq prompt, influencing the complexity and style of the generated questions.
Dynamic Retesting with Rule-based System:
Following the initial assessment, a rule-based system analyzes student performance data (scores and topics covered). Pre-defined thresholds for each topic determine whether a student has grasped the material.
If a student scores below the threshold in a particular topic, identified by temporary topic IDs assigned during question generation (potentially facilitated by LangChain's data wrangling capabilities ),the platform automatically generates a retest focusing specifically on those weak areas. This targeted approach promotes deeper understanding and reinforces areas requiring further attention.

