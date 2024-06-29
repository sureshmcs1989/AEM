**Steps to setup AEM.**
1. Create Base AEM image.
2. Dowload cq-quickstart.jar and license.properties file and move into aem/base folder 
3. cd aem/base
4. docker build -t aem-base
5. root directory cd aem
6. docker-compose up -d
7. To check the docker container list CLI : docker ps
8.Access local site : http://localhost:4502/ (author), http://localhost:4503/ (publisher)

Note : The site will take some time to load the browser when the run first call.
   
