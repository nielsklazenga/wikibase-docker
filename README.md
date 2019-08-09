# wikibase-docker

`docker-compose` file and additional files to create Wikibase instance for the TDWG-TNC, using the Wikibase Docker images.

The `docker-compose` file differs from that in the [wmde/wikibase-docker](https://github.com/wmde/wikibase-docker) repository in that all volumes are bound to the host machine. It also mounts the `LocalSettings.php` file and the logo. 

To get it running:

1.  Clone repository

    > git clone https://github.com/nielsklazenga/wikibase-docker.git

2.  Bring up the containers

    > docker-compose up -d

3.  Check if everything is running

    > docker-compose ps

    There should be eight containers and the state of all of them should be 'Up'.

4.  The following sites will now be running:

    - Wikibase: http://localhost:8181
    - Query service: http://localhost:8282
    - SPARQL endpoint: http://localhost:8989/bigdata/sparql

5.  Add content...
