## How it works ?
1. In gateway and msapp directories, run this to generate applications :

    yo jhipster

2. Package both applications by running in those two directories :

    mvn package  docker:build

4. Go in docker-compose-config directory and run the jhipster docker-compose subgenerator :

    yo jhipster:docker-compose

3. Run the registry first :

    docker-compose up -d jhipster-registry

4. Finally run the rest of the applications by running :

    docker-compose up -d
