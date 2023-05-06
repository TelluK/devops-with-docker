MANDATORY EXERCISE 1.13: HELLO, BACKEND!

Submit the Dockerfile and the command used.

---

Build the image with the tag "back"

$ docker build . -t back

Run image as a container, host machine port 8080 is mapped to container port 8080

$ docker run -p 127.0.0.1:8080:8080 back
