Command to record video on raspberry pi usb cam:

ffmpeg -video_size 1280x720 -framerate 30 -f v4l2 -i /dev/video0 demo-capture-$(date -Iseconds | sed -E s/:/_/g).avi
