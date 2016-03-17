## How it works ?
In gateway and msapp directories, run this to generate applications :
    yo jhipster

Package both applications by running in those two directories :
    mvn package  docker:build

Go in docker-compose-config directory and run the jhipster docker-compose subgenerator :
    yo jhipster:docker-compose

Run the registry first :

    docker-compose up -d jhipster-registry

Finally run the rest of the applications by running :

    docker-compose up -d

Access the gateway via http://localhost:8080

Access the registry via http://localhost:8761

Access Kibana dashboard via http://localhost:5601/
