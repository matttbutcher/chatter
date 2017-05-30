# chatter
Chatter: Web Messenger

-----------------------------------------------------------------------------
Introduction

A simple online message management system which is composed of three tiers (web portal, middle layer and database). Basic Requirements:

  1. Users are able to Add/Remove/Update/Search/ their SMS messages through a web portal. SMS messages are stored in the back end database. Users don’t need to sync SMS with their phones. This platform is just for online SMS management but is not for automatic phone message backups.
  2. Before they start performing any above actions, they will need to log into the system (therefore, you system should provide basic user registration/login/logout functions as well).
  3. They can share their messages with other users by marking the message as public or private. If a message is marked as public, it can be seen by other users too. So a user can see both messages that are created by himself or messages that are marked as public by other users.
  
-----------------------------------------------------------------------------
Task Details

  1. Web portal: The architecture of the assignment needs to be strictly three tiers based. This means web portal is only used for rendering contents, taking inputs from users and feeding back results. The portal is not supposed to handle any business logics (PHP, Ruby on Rails, JSP style portal and things similar will not be accepted and marked). You will need to use javascript+HTML 5+CSS for your web portal development. Necessary third party libraries are allowed in the implementation. It should not point any specific backend server (bound with specific IP/hostname or etc.) but needs to be configurable using some configuration files
  2. Middle Layer: A middle layer that talks to both database and web portal through message exchange. It should handle all business logics (how SMS should be manipulated, how transaction is supported, authorisation and authentication and etc.). The middle layer needs to be implemented conforming to RESTful web service standard. It needs to be done in JAVA rather than any other programming languages. It should not point any specific backend database, but is configurable using web.xml configure file.
  3. Database: MySQL database will be used to store data. You will need to define your database schema that support your application. For this assignment, you don’t need to worry too much about the DB normalisation rules and etc. You can use one table even as long as it satisfies your needs.
  4. Message Exchange: The messages that are exchanged between the portal and middle layer need to be JSON. This leads the whole system to a completely decoupled manner. No portal will be relying on any specific middle layer’s implementation and vice versa. Both of them are only dependent on the contents of the messages exchanged and interpretations of those messages.
  
-----------------------------------------------------------------------------
