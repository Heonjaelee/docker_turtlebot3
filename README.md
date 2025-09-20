# docker_turtlebot3
It operates turtlebot3-waffle in Jetson-orin-nano. 

Jetpack 6.2.1
L4T 36.4.4
ROS2 Humble

#build \n
docker build -t rostest -f ./Dockerfile_turtlebot .

#run \n
docker run -it --rm --privileged --net=host rostest

#in container \n
./update.sh $OPENCR_PORT $OPENCR_MODEL.opencr
