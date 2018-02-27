# Docker Tomcat 7

## Project

This project is a slight variant of a Docker file found in the Tomcat docker-library:

It is based on the Alpine `Dockerfile` for Tomcat 7, tag `jre7-alpine`, and includes the following packages:

* JRE 7
* Tomcat 7


## Difference

The difference is that the resulting image does not include any of the default Tomcat `webapps` (`docs`, `examples`, `host-manager`, `manager`, `ROOT`)

## Resources

* https://github.com/docker-library/tomcat
* https://tomcat.apache.org/

## License

* The Tomcat Docker files are released under an Apache License Version 2: https://github.com/docker-library/tomcat/blob/master/LICENSE
* The code in this project is also released under an Apache License Version 2
