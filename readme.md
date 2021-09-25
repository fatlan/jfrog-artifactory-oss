### JFROG(artifactory-oss) Community Version - Open Source - Dockerize

~~~
mkdir data
mkdir data/artifactory
mkdir data/nginx
~~~

~~~
chown -R $UID:$GID data
chmod -R 777 data
~~~

~~~
docker-compose up -d
~~~

you make same artifactory nginx conf (80 redirect 443 and get domain and ssl)

enter domain
~~~
admin:password
~~~

ref: [jfrog](https://www.jfrog.com/confluence/display/JFROG/Installing+Artifactory)
