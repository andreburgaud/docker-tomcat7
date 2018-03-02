# Docker Tomcat 7

## Project

This project is a slight variant of a Docker file found in the Tomcat docker-library:

It is based on the Alpine `Dockerfile` for Tomcat 7, tag `jre7-alpine`, and includes the following packages:

* JRE 7
* Tomcat 7

## Differences

The resulting image exhibit the following differences from `tomcat:7.0.85-jre7-alpine`:
1. Does not include any of the default Tomcat `webapps` (`docs`, `examples`, `host-manager`, `manager`, `ROOT`)
1. Attempts to connect to different PGP servers to overcome issue `keyserver receive failed: Address not available`
1. Includes the font package `ttf-dejavu` to overcome NPE issue such as the one descrived in https://github.com/docker-library/openjdk/issues/73

## Resources

* https://github.com/docker-library/tomcat
* https://tomcat.apache.org/

## License

* The Tomcat Docker files are released under an Apache License Version 2: https://github.com/docker-library/tomcat/blob/master/LICENSE
* The code in this project is also released under an Apache License Version 2
