# Instructions

## Enable GUI

'''
xhost +local:docker

docker run -it --rm \
    --env="DISPLAY" \
    --env="QT_X11_NO_MITSHM=1" \
    --volume="/tmp/.X11-unix:/tmp/.X11-unix:rw" \
    ros2
    
export containerId=$(docker ps -l -q)
'''

or just call `launch.sh`