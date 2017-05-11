# Scince2010-docker

Create a docker image to download the SCINCE 2010 shapefiles. For more info see this [post](https://blog.diegovalle.net/shapefiles-of-mexico-agebs-manzanas-etc-es.html)


```
docker pull diegovalle/scince2010
mkdir -p /tmp/scince2010/shps
docker run -v /tmp/scince2010/shps:/shapefiles/shps -i -t diegovalle/scince2010
```

and run ./download.sh


