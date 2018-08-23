# Dockerized Locust
A dockerized locust workload generator.
The locustfile.py is downloaded at startup from the configured URL. This allows this docker image to be used in different scenarios without having to rebuild it.

## Usage
The following environment variables have to be set:
* `LOCUST_MODE`: `master`, `slave` or `standalone`
* `LOCUST_FILE_URL`: URL of the locustfile that will be downloaded at startup
* `TARGET_URL`: URL of the target system (e.g., http://edge:8080)
