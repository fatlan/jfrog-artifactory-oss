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

**NoT**: compose'deki jfrog artifactory portları expose edilmemiştir, erişim nginx 443 üzerinden yapılmaktadır, isterseniz '#' işaretini kaldırıp ayrıca portları expose edip nginx'e uğramadan da direk portlar üzerinden jfrog artifactory çağırabilirsiniz. Ya da nginx'i devre dışı bırakıp o şekilde de kullanavilirsiniz, bir diğeri de nginx'i iptal edip trafiği farklı bir proxy üzerinden de geçirebilirsiniz.

ref: [jfrog](https://www.jfrog.com/confluence/display/JFROG/Installing+Artifactory)
