1)docker build -t image_vue:v1 .
2)docker run -it -d -p 8081:8080 --name vc1 image_vue:v1
3)docker exec -it image_vue:v1 /bin/bash
4)docker commit vc1 pranavv481/image_vue:tagname
5)docker push pranavv481/image_vue:tagname

deploy

6)docker pull pranavv481/image_vue:tagname
7)docker run -it -d -p 8081:8080 --name vc1 pranavv481/image_vue:tagname