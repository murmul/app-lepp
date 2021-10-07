# LEPP Stack (+pgAdmin) in Docker

To run stack do:
1. Clone repo `git clone https://github.com/murmul/app-lepp`
2. Copy content of the `sample` directory to the root
3. Edit `.env` file
4. Set `sudo chown -R 5050:5050 ./storage/db_admin` cause pgAdmin runs as the pgadmin user (UID: 5050) in the pgadmin group (GID: 5050) in the container
5. Command `docker-compose up -d`

To stop and remove all containers command `docker-compose down`