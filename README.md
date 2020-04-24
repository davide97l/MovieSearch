# MovieSearch

...

## Environment configuration
- Download movies posters dataset from https://www.kaggle.com/neha1703/movie-genre-from-its-poster/discussion/35485 and put all images into the folder `moviesearch/static/posters.txt`.
- Download movies reviews from http://ai.stanford.edu/~amaas/data/sentiment/ and put the folder `aclImdb` in the path `moviesearch\utils`.
- The website relies on MongoDB, make sure it is running on your machine before going on. Otherwise you can download and install it from https://www.mongodb.com/.
- Install all dependencies with the command: `pip install requirements.txt`.

## Database preparation
- To clean, preprocess and upload movies data run the command `python upload_movies.py`. Note that the execution of this process includes computing movies recommendations for about 5000 movies with with nearest neightbors, thus it may take a few hours depending on your hardware.
- To clean, preprocess and upload movies reviews run the command `python upload_reviews.py`. It will upload around 50k movies reviews.

## Run the server
- Finally, you can run your server with the command `python manage.py runserver`.
- You will find the website at the location `http://127.0.0.1:8000/`.
