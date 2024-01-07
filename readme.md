# links
- (nodejs-react-keycloak] (https://medium.com/devops-dudes/secure-front-end-react-js-and-back-end-node-js-express-rest-api-with-keycloak-daf159f0a94e)


# Good Links
- [keycloak docker] (https://towardsdev.com/run-keycloak-in-docker-with-extenal-db-1b504ad00eae)

- [keycloak] (https://towardsdev.com/run-keycloak-locally-with-docker-compose-db9a9f2fb437)

# docker
- docker build --build-arg KEYCLOAK_VERSION=21.1.1 -t keycloak --progress=plain --no-cache .

# docker-compose
- docker compose build --no-cache keycloak
- docker compose up -d
- docker compose ps 
CONTAINER ID   IMAGE                      COMMAND                  CREATED          STATUS                            PORTS                                                                                            NAMES
ddd5290a13af   keycloakreactjs-keycloak   "/opt/keycloak/bin/k…"   13 seconds ago   Up 7 seconds                      8443/tcp, 0.0.0.0:8787->8787/tcp, :::8787->8787/tcp, 0.0.0.0:8180->8080/tcp, :::8180->8080/tcp   keycloak
d0c1c8263eb9   postgres:14-alpine         "docker-entrypoint.s…"   15 seconds ago   Up 9 seconds (health: starting)   0.0.0.0:5432->5432/tcp, :::5432->5432/tcp                                                        db
22950f10307d   dpage/pgadmin4:latest      "/entrypoint.sh"         15 seconds ago   Up 9 seconds                      443/tcp, 0.0.0.0:5050->80/tcp, :::5050->80/tcp                                                   pgadmin
- docker compose logs -f keycloak

# Add to /etc/hosts
127.0.0.1 keycloack.com.au

# Open browser
- http://localhost:8180/
- http://keycloak.com.au:8180/

- click administrator console
        admin/password