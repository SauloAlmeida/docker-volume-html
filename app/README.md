1. Go to server folder
docker build -t html-server .

2. Create a container passing resource pages
docker run -v ...\resource\:/usr/share/nginx/html -dp 8081:80 html-server