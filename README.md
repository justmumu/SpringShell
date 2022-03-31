# Spring RCE

This repository provide a vulnerable spring application and [nuclei](https://github.com/projectdiscovery/nuclei) template.

Vulnerable application original repository: [Spring4Shell-POC](https://github.com/reznok/Spring4Shell-POC)

## Steps

1. Clone this repository
2. Run `cd <repository_directory>/vulnapp`
3. Run `docker-compose up`
4. Wait for the application to run
5. Run `nuclei -t <repository_directory>/nuclei-templates/spring4shell.yaml -u http://localhost:8080/helloworld/greeting`
