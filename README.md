# BANKDOCK

## Requirements

You need **Docker CE** and **Docker Compose**.

1. Install Docker CE as per instructions at [https://docs.docker.com/install/](https://docs.docker.com/install/)

2. Install Docker Compose as per instructions at [https://docs.docker.com/compose/install/](https://docs.docker.com/compose/install/)

3. Clone projects from Gitlab into `./projects` folder
   (You can use the git-projects.sh script)

> NOTE: Be aware -- at writing (1st june) time there are no such gitlab projects yet!

## How do I operate this thing?

### Start projects

1. Change your current working directory to the same as this file (`README.md`, also same dir/folder as `docker-compose.yml` file)

2. Run `docker-compose up`. That's it Aleks!

3. ALEKS ALEKS ALEKS WOOOO

> If you want to run the projects in a detached state, i.e. without outputting anything to a console, run `docker-compose -d up`

### Stop projects

1. Press `CTRL+C`. That's IT! THAT EASY!

> However, if you started the projects in a detached state you need to follow the two steps below

1. Again: change your current working directory to the same as this file.

2. Run `docker-compose stop`

## Projects in this composed docker environment

### api-gw

API gateway

### customer-fe

Frontend for the customers / end users

### test

This docker environment just tests that a connection from one docker can be made to another in the same composed environment.

> It makes a cURL call from itself to api-gw and outputs the result in the console!

### bank-fe (NOT YET)

Frontend for the bank administrators and users

### broker-fe (NOT YET)

Frontend for the broker administrators and users
