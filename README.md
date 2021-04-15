```docker build -t localhost:5001/myflaskimage .
docker run -d -p 5000:5000 --name=myflaskapp localhost:5001/myflaskimage
docker ps
curl localhost:5000
docker stop myflaskapp```


PACKETO WAY!
# set default builder
pack set-default-builder gcr.io/buildpacks/builder:v1

# build image
pack build localhost:5001/hello-world-python:pack-0.0.1

