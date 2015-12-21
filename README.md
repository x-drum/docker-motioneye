# docker-motioneye
Container for motionEye, a web-based user interface for motion.
( https://github.com/ccrisan/motioneye )

## Notes
* By default the container will expose the webinterface on port **tcp/8765**.
* A default media storage path is available at **/var/lib/motioneye**.

## Usage

Fire up an instance with web interface available on port 8000 and a mapped volume:
```bash
$ docker run -ti --rm -p 8000:8765 -v /path/to/storage:/var/lib/motioneye xdrum/motioneye:latest
```

