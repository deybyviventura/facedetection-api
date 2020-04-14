# facedetection-api

Simple api for testing how Clarifai Machine learning face detection works.
This has a simple user CRUD based on a PostgreSQL database.

## To run it just:

1. Make sure to install PostgreSQL database engine first
2. Upload the database.sql which allows you to have a couple of tables users and login
3. Update the database data connection in server.js
4. Add your own API key in the controllers/image.js file to connect to Clarifai API.
5. Clone this repo
6. Run npm install
7. Run npm start

Get Clarifai API key [here](https://www.clarifai.com/).
Download PostgreSQL [here](https://www.postgresql.org/) or install it in your server provider.

## Testing

You can test it with Postman using the endpoints available in the server.js file

```
/signin
/register
/profile/:id
/image This updates the number of entries, it means how many photos have checked
/imageurl This handles the Clarifai API Call
```

## Frontend Repo

You can check [this repo](https://github.com/deybyviventura/facedetection) to see the simple frontend
implementation using React.

## Security

This is for educational porpose. I recommend to use secrets to manage the database data connection
and the same for Clarifai API key. This is a nice feature you can use in Heroku or Kubernetes.

## Demo

You can see an entire [demo](https://clarifai-facedetection.herokuapp.com/)
