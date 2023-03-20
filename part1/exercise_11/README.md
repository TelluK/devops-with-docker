EXERCISE 1.11: SPRING

Submit the Dockerfile you used to run the container.

---

Build the image with the tag "spring"

$ docker build . -t spring

Run image as a container, host machine port 3030 is mapped to container port 8080

$ docker run -p 127.0.0.1:3030:8080 spring
