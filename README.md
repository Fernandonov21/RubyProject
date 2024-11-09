# Ruby Hello World Project

## Project Description

This is a simple "Hello World" Ruby application to demonstrate the basics of Ruby programming and containerization using Docker. The project aims to show how Ruby can be executed in a containerized environment, making it easy to run and share across different systems.

In this project, we used Ruby to print "Hello World" to the console. We also created a Dockerfile to containerize the application, ensuring that it runs smoothly in different environments without any additional setup.

### Technologies Used
- Ruby (Programming language)
- Docker (Containerization)

## Table of Contents
- [Requirements](#requirements)
- [Installation and local etup](#installation-and-local-setup)
- [How to Run the Project](#how-to-run-the-project)
- [How to configure a docker image](#how-to-configure-a-docker-image)


## Requirements

Before you can run the project, ensure that you have the following installed on your machine:

1. **Ruby**  
   This project uses Ruby to run the "Hello World" script. Ensure you have the latest version of Ruby installed (>= 3.1). You can check Ruby's official website for installation instructions or use a version manager like [rbenv](https://github.com/rbenv/rbenv) or [rvm](https://rvm.io/) to manage Ruby versions.

   - Latest Ruby version: [Ruby Download Page](https://www.ruby-lang.org/en/documentation/)

2. **Docker**  
   You will need Docker to build and run the project container. Install Docker Desktop for your platform (Windows, macOS, or Linux).

   - Latest Docker version: [Docker Install](https://docs.docker.com/get-docker/)

## Installation and Local setup 
1. clone this repository to your local machine:
```bash
https://github.com/Fernandonov21/RubyProject.git
```
2. Open Visual Studio Code.
3. Install dependencies
In the terminal (you can use Command Prompt, PowerShell, or the VS Code integrated terminal), navigate to the project folder and install the required dependencies with:
```bash
bundle install
```
## How to run the project
After the dependencies are installed, you can run the project using the following command:
```bash
ruby Project5.rb
```
To see the page you just follow the link:
```bash
http://localhost:4567
```
## How to configure a docker image
The project has already a docker file so the only thing that you need is up the container
1. In the terminal (you can use Command Prompt, PowerShell, or the VS Code integrated terminal), navigate to the project folder and execute the next command:
```bash
docker build -t rubyproject .
```
2. run the image
```bash
docker run -p 4567:4567 fernando785/rubyproject
```
## IMPORTANT
To access the application at http://localhost:4567, ensure that port 4567 is available. If the port is already in use, stop any process occupying it and try running the command again.

