SpringBoot QuizApp with MicroService Architecture

1) This is a quiz app using SpringBoot which is based on MicroService Architecture.

2) This app only consists of backend part which is written in SpringBoot with implementation of controller layer, service layer and dao layer.

3) It has question-microservice and quiz-microservice which communicate with each other for the quiz-app with help of service-registry and api-gateway.
  
4) In this app MySQL is used, 'train' is database name and a table named 'question' is created as described below for the question-microservice.
+-----------------+--------------+------+-----+---------+----------------+
| Field           | Type         | Null | Key | Default | Extra          |
+-----------------+--------------+------+-----+---------+----------------+
| id              | int          | NO   | PRI | NULL    | auto_increment |
| question_title  | varchar(100) | YES  |     | NULL    |                |
| option1         | varchar(50)  | YES  |     | NULL    |                |
| option2         | varchar(50)  | YES  |     | NULL    |                |
| option3         | varchar(50)  | YES  |     | NULL    |                |
| option4         | varchar(50)  | YES  |     | NULL    |                |
| right_answer    | varchar(50)  | YES  |     | NULL    |                |
| difficultylevel | varchar(20)  | YES  |     | NULL    |                |
+-----------------+--------------+------+-----+---------+----------------+

5) 'quiz' database for quiz-microservice and two tables named 'quiz' and 'quiz_question_ids' are there which created automatically when services communicate each other. So there is no need to make tables for 'quiz' database.

:- P.S Rajput
