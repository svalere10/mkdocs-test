
...

git clone <lerepo>

cd <lerepo>

docker run -v /home/dockerlab1-12a/mkdocs-test:/root/mkdocs-test -p 8000:8000 -it python:2.7 bash

docker run -dit -p 8000:80 -v "$PWD/site":/usr/local/apache2/htdocs/ httpd
