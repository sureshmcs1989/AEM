**Steps to setup AEM.**
1. Create Base AEM image.
2. cd aem/base
3. docker build -t aem-base
4. root directory cd aem
5. docker-compose up -d
6. To check the docker container list CLI : docker ps
7.Access local site : http://localhost:4502/ (author), http://localhost:4503/ (publisher)

Note : The site will take some time to load the browser when the run first call.
   
