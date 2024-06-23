#### run

- install docker and swarm first

$ docker pull alrasyidlathif/chatoroom-server:1.0.0

$ docker pull alrasyidlathif/chatoroom-client:1.0.0

$ docker network create --attachable --driver overlay --scope swarm chatoroom-network

$ docker run --network chatoroom-network --name chatoroom -d alrasyidlathif/chatoroom-server:1.0.0

$ docker run -it --network chatoroom-network --name client{x} alrasyidlathif/chatoroom-client:1.0.0

![image](https://github.com/alrasyidlathif/chatoroom/assets/22503964/d40747f2-1058-47b5-96c5-7206c57618aa)
