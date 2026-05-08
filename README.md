# Docker Lab 1: Introduction to Docker Containerization

This repository contains a simple Python application containerized using Docker, demonstrating the basics of creating a Dockerfile, building an image, and running a container.

## Project Structure
- `docker-lab1/app.py`: A simple Python script that prints a greeting message from within the container.
- `docker-lab1/requirements.txt`: A file for managing Python dependencies (empty for this simple app).
- `docker-lab1/Dockerfile`: The instructional blueprint used by Docker to build the image.

---

## Guided Questions

**1. What role does the Dockerfile play in containerization?** 

The Dockerfile is a text document that contains all the necessary instructions and commands to assemble a Docker image. It acts as an automated, reproducible blueprint that Docker reads sequentially to build the environment your application will run in.

**2. Why are Docker containers lighter than virtual machines?** 

Unlike virtual machines which require a full, separate "guest" Operating System for each VM, containers share the host machine's Operating System kernel. This eliminates the massive overhead of running redundant OS layers, resulting in significantly less disk space usage, drastically reduced memory usage, and near-instant startup times.

**3. What happens when the container finishes execution?** 

When the primary process running inside the container (specified by the `CMD` or `ENTRYPOINT` instruction—in this case, running the Python script) completes its task and exits, the container itself automatically stops. The container remains on the system in an "exited" state (which can be viewed using `docker ps -a`) until it is explicitly removed.

### Acknowledgment

We are grateful to our instructors for their guidance and support throughout the development of this project. 

This work reflects my learning journey as a programmer.

## Disclaimer 
<div align="center"> 
  I do not own the names, information or references included in this project they are used purely as placeholders. <br> 
  All trademarks, service marks, trade names, and other intellectual property rights belong to their respective owners.  <br><br>

  Made with 💗 by <a href="https://github.com/lurxdel"><strong>Lurxdel</strong></a>
</div>
