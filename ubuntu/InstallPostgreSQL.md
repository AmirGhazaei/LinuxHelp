

1. Install PostgreSQL
   1. `sudo apt update`
   1. `sudo apt install postgresql postgresql-contrib`
   
1. Install pgAdmin
   1. `sudo apt install postgresql-common`
   1. `sudo sh /usr/share/postgresql-common/pgdg/apt.postgresql.org.sh`

1. Set Password for default user postgres
   1. `sudo su - postgres`
   1. `psql`
   1. `ALTER USER postgres WITH PASSWORD '123456';`
