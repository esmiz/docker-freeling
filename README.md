

Freeling Docker Image
---------------


On debian jessy 64

    docker build -t herchu/freeling4:v0 .

    echo "Mi casa es bonita." | docker run -i herchu/freeling4:v0 /usr/bin/analyze -f es.cfg


Debian Package
--------------

The Freeling Debian packages is:

    https://github.com/TALP-UPC/FreeLing/releases/download/4.0/freeling-4.0-jessie-amd64.deb


To Do
-----

Publish

Reduce footprint
    Using docker-squash
    docker save 7c0a6a6f5732 | PATH="/usr/local/opt/gnu-tar/libexec/gnubin:$PATH" sudo docker-squash -t herchu/freeling4:pub | docker load
