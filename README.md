# docker-wso2is

Docker image to install and run WSO2 Identity Server.

## Tags

* [5.3.0, latest](https://github.com/ihcsim/docker-wso2is/tree/is-5.3.0)
* [5.0.0](https://github.com/ihcsim/docker-wso2is/tree/is-5.0.0)

## Description
The Dockerfile will:

* Use `wget` to pull the IS 5.3.0 ZIP from a S3 bucket into the container `/opt` folder.
* Install `zip`.
* Unzip the IS 5.3.0 ZIP.
* Remove the IS 5.3.0 ZIP.
* Expose the container port `9443`, `9763`, `8000`, `10500`.
* Set the `wso2server.sh` start-up script as the container start-up entrypoint.

## Usage
To run the Identity Server:
```sh
$ docker run --rm --name your_container_name -p 9443:9443 isim/wso2is
```
To access web admin console, navigate to https://localhost:9443 from your web browser.

## License
Refer to the [LICENSE](LICENSE) file. WSO2 license can be found [here](http://wso2.com/licenses).
