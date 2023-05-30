# Weatherapp

A simple weather app displaying the current weather in our favourite city of Helsinki.

## Prerequisites

* An [openweathermap](http://openweathermap.org/) API key.
* [Docker Desktop](https://docs.docker.com/desktop/install/linux-install/) or [Docker Engine](https://docs.docker.com/engine/install/) + [Docker Compose](https://docs.docker.com/compose/install/) installed.

## Running the app locally (Linux)

* Clone the repository to your local machine:

  `git clone git@github.com:tranzzik/efi-recruitment.git`
  
* cd into the cloned repository:

  `cd efi-recruitment`
  
* Use your favourite text editor to edit the docker-compose.yml file and set the APPID variable to your openweathermap API key:

  `vi docker-compose.yml`

  `APPID=<your_api_key_here>`

  Make sure **not** to put a space after the = sign.
  
 * Use Docker Compose to build and start the application:
  
    - Docker Desktop:
    `docker compose up`
  
    - Docker Engine + Docker Compose:
    `docker-compose up`
    
    This will create the images, create contaiers and start them - the frontend on port 8000, the backend on port 9000. You can then access the app at `http://localhost:8000/`.
    
    By default, the app starts in your terminal, and will stop the containers if you close it. To run the containers in the background, add the `-d` flag to either command:
    
    `docker compose up -d`
    
    To then stop and remove the containers, run:
    
    `docker compose down`
  
  
