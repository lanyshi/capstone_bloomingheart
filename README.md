# 2019 Capstone Project: BloomingHeart
My team and I created this project BloomingHeart which is a website that allows users from Bloomington, IN to engage
more actively in the local fundraising events.

This website was mainly built with PHP, JavaScript, jQuery, Bootstrap, REST APIs, Git, MySQL, and Linux/Unix.

## Features
The major, high-priority features include:
* User profile
* View available charities and non-profits
* Make donations
* Join charity events
* Sign up for an upcoming event
* Add a charity to favorites and get notified for its future events via email

## Highlights
During implementation, there are a few highlights with the technologies we used, including PHP and REST APIs.

### User Authentication
User authentication was a tricky part because of the encryption of user passwords. Instead of encrypting the password
with PHP, we decided to use MySQL ```AES_ENCRYPT()``` to avoid the chance of password string being exposed. With AES,
the password and all other user information get stored into the MySQL database. When the user tries to log in to their
account, the system searches the MySQL database and uses ```AES_DECRYPT()``` to decrypt the password.

### Session
One of the things we tried to accomplish was storing user information to be used across multiple pages (e.g. username).
This is when ```$_SESSION``` came into the picture. By putting ```session_start()``` at the beginning of each page, we
were able to retrieve all the variable values from the global ```$_SESSION``` variable.

## Summary
This was a simple web application with a few web pages and basic functionalities, but we were able to learn from
the development process and gain experience with all the tools we utilized.

![people page](https://github.com/lanyshi/capstone_bloomingheart/blob/main/people.png)