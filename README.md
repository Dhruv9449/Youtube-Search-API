# YOUTUBE SEARCH API
## Problem Statement
Use the Youtube search API to get all the videos with query "Apple" and store it in a database. Make an endpoint to query the DB based on the video name. [Bonus: Implement fuzzy search]

## Table of contents
- [Preview](#preview)
    - [Search](#search)
    - [I'm Feeling Lucky](#im-feeling-lucky)
- [Setting-up and Installation](#setting-up-and-installation)
    - [Cloning Repositary](#cloning-repositary)
    - [Setting-up a virtual environment](#virtual-environment)
    - [Installing Dependancies](#installing-dependancies)
    - [Setting-up Environment variables](#environment-variables)
    - [Running the server](#run-the-server)
- [License](#license)

## Preview
### Search
Lists all the results where the keyword enter matches

![YoutubeAPI-search](assets/search.gif)

### I'm Feeling Lucky
Redirects to the first search result

![YoutubeAPI-im_feeling_lucky](assets/im_feeling_lucky.gif)

## Setting up and Installation
### Cloning Repositary 
Clone this repositary by running in your terminal-
```
git clone "https://www.github.com/Dhruv9449/IEEE-recruitment"
```

### Virtual environment
After cloning the repositary install `virtualenv` set up a virtual environment using the following commands -  
```sh
pip install virualenv
virtualenv venv
``` 
Activate it -  
Windows
```psh
C:\Users\Username\dir> .\venv\Scripts\activate
```
Linux
```sh
user@hostname:~$ source venv/bin/activate
```
Refer to the [official virtualenv documentation](https://virtualenv.pypa.io/en/latest/) for any further help

### Installing dependancies
To install all the dependancies for this project run the following command in your terminal - 
```sh
pip install -r requirements.txt
```
### Environment Variables 
You will need create a `.env` as shown in `.env.example` inside the `YoutubeSearch/` folder with 
- `Django Secret key` - can be anything you want. Create a unique one.
- `Youtube API key` - Your Youtube API key which will be required for getting youtube's data. You can get one from [Google's official website](https://console.developers.google.com/home/). For more info on the API you can refer [Google APIs github](https://github.com/googleapis/google-api-python-client). 

`.env`
```
SECRET_KEY=<Your Django key>
YOUTUBE_API_KEY=<Your youtube API key>
```
### Run the server!
We're all set the run the server now! Type the following command in your terminal -  
```
./manage.py runserver
```
And then type `localhost:8000` or `127.0.0.1:8000` in your browser's search bar and voila!

## License 
Copyright © 2022 Dhruv9449  
[MIT License](LICENSE)






