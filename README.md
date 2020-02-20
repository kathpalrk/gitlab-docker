# GITLAB Community Edition on Docker Installation

Here we have defined the parameters to install & configure the GitLab over the Docker Container.

In the first step we have defined the Image which will take it from GitLab Docker HUb. Here you can use the enterprise edition also. Instead of using the Community edition image just type gitalb-ee Then it will take the Enterprise edition image.

# GitLAB Volume Container 
Also, if we are not using the mentioned folder then also, it will create it automatically which we have defined as Volume.

In the Next we have defined the GITLAB Variable which will use to update the Rails and Postgres datbase information.

# Here we need to declare the Postgres Database image.

Finally, we just need to use the following command to start the container whcih mentioned below.

$ docker-compose up -d 

Next we need to execute the running container.

$ docker exec -it gitlab bash 

$ cd /opt/gitlab/bin

$ ./gitlab-ctl start 

That's it Guys, After that try to access the http://172.28.0.3/users/sign_in

It will ask you the Username & Credentials.

UserName would be root by default and even you can register the new one also.

The password would be Red_hat099 and you may use the different one also.

Hope you guys like it... :-)


