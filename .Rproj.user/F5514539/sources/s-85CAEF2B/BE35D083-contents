https://codefresh.io/docker-tutorial/build-docker-image-dockerfiles/
https://github.com/rocker-org/rocker-versioned/tree/master/rstudio
docker run -d -p 3838:3838 -p 8787:8787 -e ADD=shiny -e PASSWORD=yourpasswordhere rocker/rstudio
https://docs.docker.com/storage/volumes/

docker build -t rstudio .
docker volume rm myvol2
docker container rm rstudio_server

docker run -d -p 8787:8787 -e PASSWORD=thirdday1 rstudio
# https://docs.docker.com/storage/volumes/

docker run -d \
  --name rstudio_server \
  -p 8787:8787 \
  -e PASSWORD=thirdday1 \
  -v myvol2:/app \
  fdrennan/rstudio