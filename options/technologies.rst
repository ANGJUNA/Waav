3. Technologies
================
* Dockerized
.. image:: /images/Screenshot_4.jpg


* GUI or HTTPS service is provided by web_nginx container which an alpine linux dockerhub image.
  At this time of writing, nginx service is defined in docker-ingeress.yml file [Git Repository may have
  older version of these separated docker compose yml files, Challenge is because of different 
  deployment environment secret credentials defined there as environment variable for the running container]. Plan is to centralize it and remove them completely from yml but instead use
  git cloud automation tool to store secretely/safely like gitlabci. [A task is in progress for it]
.. image:: /images/Screenshot_5.jpg

* Web_php container has the php binary and interpreter for all php executions. This same is used by waavadmin/laravel and controlroom/clipbucket frameworks.
