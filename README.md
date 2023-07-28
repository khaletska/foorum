# foorum

## Table of Contents
- ### [General Information](#general-information)
- ### [Technologies](#technologies)
- ### [Setup](#setup)
- ### [Usage](#usage)
- ### [Authors](#authors)

## General Information
 The project involves creating a web forum where users can communicate through posts and comments, with the ability to like and dislike posts and filter content by categories and date, and sort by likes in acsending or descending order. User authentication is required for creating and interacting with content, with passwords being encrypted and stored in an SQLite database. There are cookies used for user storing session token, and Docker is provided for containerization. 

 In this project we have 4 types of users :

- Guests
    These are unregistered-users that can neither post, comment, like or dislike a post. They only have the permission to see those posts, comments, likes or dislikes.
- Users
    These are the users that will be able to create, comment, like or dislike posts.
- Moderators
    These userds can to monitor the content in the forum by deleting or reporting post to the admin.
    To become a moderator the user should request an admin for that role in their profile.
- Administrators
    Users that manage the technical details required for running the forum. This user is able to:
    - Promote or demote a normal user to, or from a moderator user.
    - Receive reports from moderators. If the admin receives a report from a moderator, he can respond to that report.
    - Delete posts and comments.
    - Manage the categories.

## Technologies
- ### [Golang](https://go.dev/)
- ### [HTML](https://www.w3.org/html/)
- ### [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- ### [Javascript](https://www.javascript.com/)
- ### [SQLite](https://sqlite.org/index.html)

## Setup
Clone the repository
```
git clone https://github.com/khaletska/foorum.git
```

## Usage
### Without docker
From root folder run:
```
go run . 
```

### With docker
From root folder run:
```
bash runDocker.sh
```
When you finish, run from root folder:
```
bash stopDocker.sh
```

You can test the project from the page [https://localhost:8080/](https://localhost:8080/)

## Credentials

You can login as:
- Administrator: `admin@gmail.com`
- Moderator: `mod@gmail.com`
- User: `user@gmail.com`

All passwords are `1111`

## Authors
- [Elena Khaletska](https://github.com/khaletska)
- [Olha Balagush](https://github.com/OlhaBalahush)
- [Taivo Tokman](https://github.com/O31)
- [Glib Ovcharenko](https://github.com/glibovcharenko)