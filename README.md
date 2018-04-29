For Assignment - 5, I have successfully implemented a RESTful Web Service in Docker using Python and Flask.

The database.json file consists of a collection of Movies with their respective ID, Name, Genre and Year.
The app.py Python file loads the JSON file and displays the data in the browser according to the given routes.
The web service contains two GET routes-
The "/movies" route displays a list of all the movies with their id, name, genre and year.
The "/movies/<id>" route displays the details of an individual movie with any given id.
The files are compiled into an image which runs in a Docker container.

Steps to run:-
1.) Change the working directory in terminal to the assignment folder.

2.) In the Docker terminal, create Docker image by running "docker build -t flask-image:latest ."

2.) Check the image created by using "docker images"

4.) Run the image inside a container by executing "docker run -d -p 5000:5000 --name flask-container flask-image"

5.) Check the running docker container by using "docker ps"

6.) The app will be running at address- "http://192.168.99.100:5000/movies"
