# SE Internship Program

# How to build a Docker image and run a Docker container
To build the Docker image from a given Dockerfile. Execute the following command:

docker build -t getting-started .

Where the -t option flags tags the image. In other words, we assign a human readable name to the final image which we can later reference.

Next, to run a Docker container. We require the Docker image. Once an image has been created, we run the following command:

docker run -dp 3000:3000 getting-started

Where the -d option tells Docker to run the new container in "detached" mode (in the background) and the -p option creates a mapping between the localhost and the container's port 3000. Without the port mapping, we wouldn't be able to access the application.

After a few seconds, open your web browser to http://localhost:3000. You should see our app!