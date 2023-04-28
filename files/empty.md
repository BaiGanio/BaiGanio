docker run -e "ACCEPT_EULA=1" -e "MSSQL_SA_PASSWORD=s3cr3@.t" -e "MSSQL_PID=Developer" -e "MSSQL_USER=SA" -p 1433:1433 -d --name=sql mcr.microsoft.com/azure-sql-edge



Breaking down the docker run command
When setting up the container, you used the docker run command. Here are what the different parts of the command do:

docker run: This is used to run containers. It needs at least one argument, and that argument is the image you want to run. In this case, it’s docker/welcome-to-docker.
-p 8088:80: This lets Docker know that port 80 in the container needs to be accessible from port 8088 on your local host.
-d: This runs the container detached or in the background.
—-name welcome-to-docker: This sets the name for your container. If you don’t do so, Docker selects a random name for you.
