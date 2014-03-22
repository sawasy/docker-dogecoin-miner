docker-dogecoin-miner
=====================
**dogecoin-miner** is cpuminer for dogecoin mining.
```shell
cd dogecoin-miner
sudo docker build -t sawasy/dogecoin-miner .
sudo docker run -i -t -e URL=stratum+tcp://stratum.dogeurl.org:943 -e USERNAME=*YOURUSERNAME* -e PASSWORD=*YOURPASSWORD* -lxc-conf="lxc.cgroup.cpuset.cpus=2,3" sawasy/dogecoin-miner
```
*I wouldn't recommend using this, unless you happen to like unkillable zombie processes.*

