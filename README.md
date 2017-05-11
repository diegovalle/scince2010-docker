# Scince2010-docker

Create a docker image to download the SCINCE 2010 shapefiles. For more info see this [post](https://blog.diegovalle.net/shapefiles-of-mexico-agebs-manzanas-etc-es.html)


```
docker pull diegovalle/scince2010-docker
mkdir -p /tmp/scince2010/shps
# mount the output directory /shapefiles/shps to a temporary one
docker run -v /tmp/scince2010/shps:/shapefiles/shps -i -t diegovalle/scince2010-docker
```

and run ./download.sh. After downloading the shapefiles will be available in /tmp/scince2010/shps


