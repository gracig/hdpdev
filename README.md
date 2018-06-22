# hdpdev

Container for hadoop software test

Obs: 
- Use [--privileged]  to allow ambari-server initialization inside container via systemd
- Use [-h horton.single.node]. Hadoop was installed using that hostname
- Remember to export ports for access . (e.g -p 8080:8080) 

## Examples

### Start container and export ambari port
docker --name hdp -d --privileged -h horton.single.node -p 8080:8080 gracig/hdpdev:v0.0.1

### Get a shell inside container
docker exec -it hdp bash
