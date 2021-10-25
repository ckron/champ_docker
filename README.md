
## setup
```
docker-compose up -d --build
docker-compose exec champ bash
cd /root/catkin_ws/src/champ
git submodule update --init
cd /root/catkin_ws
apt update
rosdep install --from-paths src --ignore-src -r -y
catkin_make
```