
# MySQL Docker Setup with Multiple Users

This project provides a Docker Compose configuration for setting up a MySQL database with multiple users. It demonstrates how to create a MySQL instance and automatically create two users upon initialization.



## Prerequisites
Docker

Docker Compose
## File Structure

To deploy this project run

```bash
.
├── docker-compose.yml
├── mysql-init/
│   └── create-users.sh
└── README.md
```


## Configuration
```
docker-compose.yml
```

This file defines the MySQL service and sets up the necessary environment variables.


```
create-users.sh
```

This script is responsible for creating the users defined in the environment variables.    


## Usage

- Clone this repository or create the files as shown in the file structure.
- Make sure the create-users.sh script is executable:

```
chmod +x mysql-init/create-users.sh
```


- Start the MySQL container:

```
docker-compose up -d
```

- To verify that the users were created successfully, you can connect to the MySQL instance and check:

```
docker-compose exec mysql mysql -uroot -p
```


Then, in the MySQL prompt:

```
docker-compose exec mysql mysql -uroot -p
```


## Credits

This project was created by My User (mrm.elec@email.com)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/mrmoghadasi/)](https://www.linkedin.com/in/mrmoghadasi/)  [![Gmail](https://img.shields.io/badge/-Gmail-red?style=flat-square&logo=Gmail&logoColor=white&link=mailto:mrm.elec@gmail.com)](mailto:mrm.elec@gmail.com)
