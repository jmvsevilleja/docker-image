# docker-image
https://cloud.google.com/container-registry/docs/quickstart

To build the Docker image, run the following Docker command from the directory containing the image's files:

`docker build -t quickstart-image .`

Before you can push or pull images, you must configure Docker to use the gcloud command-line tool to authenticate requests to Container Registry. To do so, run the following command (you are only required to do this once):

`gcloud auth configure-docker`

To tag the Docker image, run the following command:

`docker tag quickstart-image gcr.io/noted-strength-235801/quickstart-image:tag1`

To push the Docker image, run the following command:

`docker push gcr.io/noted-strength-235801/quickstart-image:tag1`

To pull the image from Container Registry onto your local machine, run the following command:

`docker pull gcr.io/noted-strength-235801/quickstart-image:tag1`

Docker Guide
`https://medium.com/@deepakshakya/beginners-guide-to-use-docker-build-run-push-and-pull-4a132c094d75`

To run on local
`docker run -p 80:80 quickstart-image`


