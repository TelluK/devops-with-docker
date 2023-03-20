MANDATORY EXERCISE 1.12: HELLO, FRONTEND!

Submit the Dockerfile.

---

Build the image with the tag "exx"

$ docker build . -t exx

Run image as a container, host machine port 3000 is mapped to container port 5000

$ docker run -p 127.0.0.1:3000:5000 exx
