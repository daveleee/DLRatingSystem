# DLRatingSystem 
This is an API of star rating system with comments for an user. Both customers and taskers can evaluate each other so that every individuals can refer to their ratings.
 
## Demonstration
### Email Template 
<img src="https://raw.githubusercontent.com/daveleee/DLRatingSystem/master/1.gif" width="320" height="590" />
### Rating Template 
<img src="https://raw.githubusercontent.com/daveleee/DLRatingSystem/master/2.gif" height="590" />
### Submit Rating Template 
<img src="https://raw.githubusercontent.com/daveleee/DLRatingSystem/master/3.gif" width="320" height="590" />
 
## Requirements 
 - Python Version - `Python 3`
 
## Installation
You have to create a Django project first.
```sh
$ mkdir your-project
$ cd your-project
$ virtualenv venv
$ source venv/bin/activate
$ pip install django
```

## Running the application using any API testing tool like Postman, Insomnia etc
Set the header - Content-Type: text/html; charset=utf-8
1. Get an email template 
```sh
$ Send a GET request to http://127.0.0.1:8000/DLRatingSystem/emailTemplate?customerIdx=1&taskerIdx=2
$ Request Parameters
    {
        "customerIdx": 1,
        "taskerIdx": 2, 
    }
$ Returns a Respose: HTML Template  
```

2. Get a rating template  
```sh
$ Send a GET request to http://127.0.0.1:8000/DLRatingSystem/ratingTemplate?customerIdx=1&taskerIdx=2
$ Request Parameters
    {
        "customerIdx": 1,
        "taskerIdx": 2, 
    }
$ Returns a Respose: HTML Template  
```

3. Get a submit rating template 
```sh
$ Send a POST request to http://127.0.0.1:8000/DLRatingSystem/submitRating?customerIdx=1&taskerIdx=2
$ Request Parameters
    {
        "customerIdx": 1,
        "taskerIdx": 2, 
    }
$ Returns a Respose: HTML Template  
```
