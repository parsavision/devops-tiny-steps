# 🚀 DevOps Tiny Steps: 600 Exercises (Continued)

---

## 🐧 PHASE 3: Linux & Servers (Continued)

### Week 6: Networking & Web Servers (Continued)

**Exercise 136: Download File with wget**  
**Goal:** Fetch file from web  
**Task:** Type `wget https://example.com/file.txt`  
**Concept:** File downloading  
**Expected:** File downloaded to current directory

**Exercise 137: Download with curl**  
**Goal:** Alternative download method  
**Task:** Type `curl -O https://example.com/file.txt`  
**Concept:** curl for downloads  
**Expected:** File downloaded

**Exercise 138: Make HTTP Request**  
**Goal:** Test web endpoint  
**Task:** Type `curl https://api.github.com`  
**Concept:** API testing  
**Expected:** Shows JSON response

**Exercise 139: Install Nginx** ⭐  
**Goal:** Set up web server  
**Task:** Type `sudo apt install nginx`  
**Concept:** Web server installation  
**Expected:** Nginx installed

**Exercise 140: Start Nginx**  
**Goal:** Launch web server  
**Task:** Type `sudo systemctl start nginx`  
**Concept:** Starting web services  
**Expected:** Nginx running

**Exercise 141: Test Nginx in Browser**  
**Goal:** Verify web server works  
**Task:** Open browser, go to `http://localhost`  
**Concept:** Web server verification  
**Expected:** See "Welcome to nginx" page

**Exercise 142: Find Nginx Config** ⭐💡  
**Goal:** Locate configuration  
**Task:** Type `ls /etc/nginx/`  
**Concept:** Config file locations  
**Expected:** Shows nginx.conf and other files

**Exercise 143: View Nginx Config**  
**Goal:** Read web server configuration  
**Task:** Type `cat /etc/nginx/nginx.conf`  
**Concept:** Configuration inspection  
**Expected:** Shows nginx settings

**Exercise 144: Create HTML File**  
**Goal:** Make a web page  
**Task:** Create `index.html` with basic HTML in `/var/www/html/`  
**Concept:** Web content creation  
**Expected:** File created

**Exercise 145: Set File Permissions for Web**  
**Goal:** Make file web-accessible  
**Task:** Type `sudo chmod 644 /var/www/html/index.html`  
**Concept:** Web file permissions  
**Expected:** File readable by web server

**Exercise 146: Test Custom HTML**  
**Goal:** View your page  
**Task:** Visit `http://localhost` in browser  
**Concept:** Testing web changes  
**Expected:** Your HTML displays

**Exercise 147: Check Nginx Logs** ⭐  
**Goal:** View web server logs  
**Task:** Type `sudo tail -f /var/log/nginx/access.log`  
**Concept:** Web server logging  
**Expected:** Shows access requests

**Exercise 148: View Error Logs**  
**Goal:** Check for errors  
**Task:** Type `sudo tail -f /var/log/nginx/error.log`  
**Concept:** Error monitoring  
**Expected:** Shows error messages

**Exercise 149: Reload Nginx Config**  
**Goal:** Apply config changes without restart  
**Task:** Type `sudo systemctl reload nginx`  
**Concept:** Graceful reload  
**Expected:** New config loaded

**Exercise 150: Configure Firewall** ⭐🎯  
**Goal:** Control network access  
**Task:** Type `sudo ufw allow 80/tcp`  
**Concept:** Firewall configuration  
**Expected:** Port 80 allowed

---

## 🐳 PHASE 4: Containers & Docker (Exercises 151-225)

### Week 7: Docker Fundamentals

**Exercise 151: What is a Container?** 💡  
**Goal:** Understand containerization  
**Task:** Read: Container is like a lightweight VM - isolated environment with app and dependencies  
**Concept:** Container concept  
**No Action:** Just understanding

**Exercise 152: Why Docker?** 💡  
**Goal:** Understand Docker benefits  
**Task:** Read: Docker ensures "it works on my machine" = "it works everywhere"  
**Concept:** Docker advantages  
**No Action:** Just understanding

**Exercise 153: Install Docker** ⭐  
**Goal:** Set up Docker  
**Task:** Follow docs.docker.com installation for your OS  
**Concept:** Docker installation  
**Expected:** Docker installed

**Exercise 154: Verify Docker Installation**  
**Goal:** Check Docker works  
**Task:** Type `docker --version`  
**Concept:** Installation verification  
**Expected:** Shows Docker version

**Exercise 155: Run First Container** ⭐  
**Goal:** Start a container  
**Task:** Type `docker run hello-world`  
**Concept:** Running containers  
**Expected:** Downloads and runs hello-world image

**Exercise 156: List Running Containers**  
**Goal:** See active containers  
**Task:** Type `docker ps`  
**Concept:** Container listing  
**Expected:** Shows running containers (might be empty)

**Exercise 157: List All Containers**  
**Goal:** See all containers including stopped  
**Task:** Type `docker ps -a`  
**Concept:** Complete container list  
**Expected:** Shows all containers

**Exercise 158: Run Container in Background** ⭐  
**Goal:** Detached mode  
**Task:** Type `docker run -d nginx`  
**Concept:** Background containers with `-d`  
**Expected:** Returns container ID

**Exercise 159: Run Container with Name**  
**Goal:** Give container a name  
**Task:** Type `docker run -d --name my-nginx nginx`  
**Concept:** Named containers  
**Expected:** Container named "my-nginx"

**Exercise 160: View Container Logs** ⭐  
**Goal:** See container output  
**Task:** Type `docker logs my-nginx`  
**Concept:** Container logging  
**Expected:** Shows nginx logs

**Exercise 161: Follow Container Logs**  
**Goal:** Monitor logs in real-time  
**Task:** Type `docker logs -f my-nginx`  
**Concept:** Log streaming  
**Expected:** Shows logs as they happen

**Exercise 162: Stop Container**  
**Goal:** Stop running container  
**Task:** Type `docker stop my-nginx`  
**Concept:** Container stopping  
**Expected:** Container stops gracefully

**Exercise 163: Start Stopped Container**  
**Goal:** Restart existing container  
**Task:** Type `docker start my-nginx`  
**Concept:** Container restarting  
**Expected:** Container starts again

**Exercise 164: Remove Container** ⭐  
**Goal:** Delete container  
**Task:** Type `docker rm my-nginx`  
**Concept:** Container removal  
**Expected:** Container deleted (must be stopped first)

**Exercise 165: Force Remove Running Container**  
**Goal:** Delete without stopping  
**Task:** Type `docker rm -f my-nginx`  
**Concept:** Forced removal  
**Expected:** Running container removed

**Exercise 166: List Docker Images** ⭐  
**Goal:** See downloaded images  
**Task:** Type `docker images`  
**Concept:** Image listing  
**Expected:** Shows available images

**Exercise 167: Pull an Image**  
**Goal:** Download image without running  
**Task:** Type `docker pull ubuntu`  
**Concept:** Image pulling  
**Expected:** Ubuntu image downloaded

**Exercise 168: Run Interactive Container** ⭐💡  
**Goal:** Get shell access  
**Task:** Type `docker run -it ubuntu bash`  
**Concept:** Interactive mode with `-it`  
**Expected:** Inside Ubuntu container shell

**Exercise 169: Exit Container**  
**Goal:** Leave container shell  
**Task:** Type `exit` in container  
**Concept:** Exiting interactive mode  
**Expected:** Back to host system

**Exercise 170: Execute Command in Running Container** ⭐  
**Goal:** Run command in container  
**Task:** Type `docker exec my-nginx ls /etc/nginx`  
**Concept:** docker exec  
**Expected:** Lists nginx config files

**Exercise 171: Get Shell in Running Container**  
**Goal:** Access running container  
**Task:** Type `docker exec -it my-nginx bash`  
**Concept:** Interactive exec  
**Expected:** Shell inside running container

**Exercise 172: Inspect Container** ⭐  
**Goal:** See detailed info  
**Task:** Type `docker inspect my-nginx`  
**Concept:** Container inspection  
**Expected:** JSON with all details

**Exercise 173: View Container Stats**  
**Goal:** Monitor resource usage  
**Task:** Type `docker stats`  
**Concept:** Resource monitoring  
**Expected:** Live CPU/memory usage

**Exercise 174: Port Mapping** ⭐💡  
**Goal:** Expose container port  
**Task:** Type `docker run -d -p 8080:80 nginx`  
**Concept:** Port publishing with `-p`  
**Expected:** Access nginx at localhost:8080

**Exercise 175: Test Port Mapping**  
**Goal:** Verify port works  
**Task:** Open browser to `http://localhost:8080`  
**Concept:** Port accessibility  
**Expected:** See nginx welcome page

---

### Week 8: Docker Images & Dockerfiles

**Exercise 176: What is a Dockerfile?** 💡  
**Goal:** Understand Dockerfiles  
**Task:** Read: Dockerfile is a recipe to build a Docker image  
**Concept:** Dockerfile purpose  
**No Action:** Just understanding

**Exercise 177: Create First Dockerfile** ⭐  
**Goal:** Write image definition  
**Task:** Create file named `Dockerfile` with:
```dockerfile
FROM ubuntu:latest
RUN apt-get update
CMD ["echo", "Hello from my image!"]
```  
**Concept:** Dockerfile basics  
**Expected:** File created

**Exercise 178: Build Docker Image** ⭐  
**Goal:** Create image from Dockerfile  
**Task:** Type `docker build -t my-first-image .`  
**Concept:** Image building  
**Expected:** Image built successfully

**Exercise 179: Run Your Custom Image**  
**Goal:** Use your image  
**Task:** Type `docker run my-first-image`  
**Concept:** Running custom images  
**Expected:** Prints "Hello from my image!"

**Exercise 180: Understand FROM Instruction** 💡  
**Goal:** Learn base images  
**Task:** Read: FROM specifies the base image to start from  
**Concept:** Base images  
**No Action:** Just understanding

**Exercise 181: Understand RUN Instruction**  
**Goal:** Learn build commands  
**Task:** Read: RUN executes commands during image build  
**Concept:** Build-time commands  
**No Action:** Just understanding

**Exercise 182: Understand CMD Instruction**  
**Goal:** Learn default command  
**Task:** Read: CMD specifies the default command when container starts  
**Concept:** Container startup command  
**No Action:** Just understanding

**Exercise 183: COPY Files to Image** ⭐  
**Goal:** Add files to image  
**Task:** Create `app.txt`, add to Dockerfile: `COPY app.txt /app/`  
**Concept:** COPY instruction  
**Expected:** File included in image

**Exercise 184: Set Working Directory**  
**Goal:** Define default directory  
**Task:** Add to Dockerfile: `WORKDIR /app`  
**Concept:** WORKDIR instruction  
**Expected:** Commands run from /app

**Exercise 185: Expose Port in Dockerfile**  
**Goal:** Document port usage  
**Task:** Add to Dockerfile: `EXPOSE 8080`  
**Concept:** EXPOSE instruction  
**Expected:** Port documented (still need -p to publish)

**Exercise 186: Use ENV Variables** ⭐  
**Goal:** Set environment variables  
**Task:** Add to Dockerfile: `ENV APP_NAME=MyApp`  
**Concept:** ENV instruction  
**Expected:** Variable available in container

**Exercise 187: Multi-line RUN**  
**Goal:** Optimize build commands  
**Task:** Use `RUN apt-get update && apt-get install -y curl`  
**Concept:** Command chaining  
**Expected:** Single layer created

**Exercise 188: Understand Image Layers** 💡  
**Goal:** Learn layer concept  
**Task:** Read: Each Dockerfile instruction creates a layer. Layers are cached for faster builds  
**Concept:** Image layers  
**No Action:** Just understanding

**Exercise 189: Build with No Cache**  
**Goal:** Force fresh build  
**Task:** Type `docker build --no-cache -t my-image .`  
**Concept:** Cache control  
**Expected:** Rebuilds everything

**Exercise 190: Tag Image with Version** ⭐  
**Goal:** Version your images  
**Task:** Type `docker build -t my-image:v1.0 .`  
**Concept:** Image tagging  
**Expected:** Image tagged with version

**Exercise 191: Create Multiple Tags**  
**Goal:** Tag same image multiple times  
**Task:** Type `docker tag my-image:v1.0 my-image:latest`  
**Concept:** Image tagging  
**Expected:** Two tags point to same image

**Exercise 192: Remove Image**  
**Goal:** Delete image  
**Task:** Type `docker rmi my-image:v1.0`  
**Concept:** Image removal  
**Expected:** Image deleted

**Exercise 193: Create .dockerignore** ⭐  
**Goal:** Exclude files from build  
**Task:** Create `.dockerignore` file, add `*.log` and `node_modules/`  
**Concept:** Build context filtering  
**Expected:** Files ignored during build

**Exercise 194: Build Simple Web App Image**  
**Goal:** Create web app container  
**Task:** Dockerfile with nginx and custom HTML  
**Concept:** Web app containerization  
**Expected:** Working web app in container

**Exercise 195: Use ARG for Build Variables** ⭐  
**Goal:** Parameterize build  
**Task:** Add `ARG VERSION=1.0` to Dockerfile  
**Concept:** Build arguments  
**Expected:** Variable available during build only

**Exercise 196: Pass ARG at Build Time**  
**Goal:** Override ARG values  
**Task:** Type `docker build --build-arg VERSION=2.0 -t my-image .`  
**Concept:** Build-time arguments  
**Expected:** Custom value used

**Exercise 197: Multi-stage Build** ⭐💡  
**Goal:** Optimize image size  
**Task:** Create Dockerfile with multiple FROM statements  
**Concept:** Multi-stage builds  
**Expected:** Smaller final image

**Exercise 198: ENTRYPOINT vs CMD** 💡  
**Goal:** Understand difference  
**Task:** Read: ENTRYPOINT sets fixed command, CMD provides default arguments  
**Concept:** Startup command options  
**No Action:** Just understanding

**Exercise 199: Use ENTRYPOINT**  
**Goal:** Set fixed startup command  
**Task:** Add `ENTRYPOINT ["nginx", "-g", "daemon off;"]` to Dockerfile  
**Concept:** ENTRYPOINT instruction  
**Expected:** Container always runs nginx

**Exercise 200: Health Check** ⭐  
**Goal:** Monitor container health  
**Task:** Add `HEALTHCHECK --interval=30s CMD curl -f http://localhost/ || exit 1`  
**Concept:** Container health checking  
**Expected:** Docker monitors container health

---

### Week 9: Docker Compose

**Exercise 201: What is Docker Compose?** 💡  
**Goal:** Understand multi-container apps  
**Task:** Read: Docker Compose runs multiple containers together as one application  
**Concept:** Docker Compose purpose  
**No Action:** Just understanding

**Exercise 202: Install Docker Compose**  
**Goal:** Get Docker Compose  
**Task:** Usually comes with Docker Desktop, or install separately  
**Concept:** Tool installation  
**Expected:** `docker-compose --version` works

**Exercise 203: Create First docker-compose.yml** ⭐  
**Goal:** Define multi-container app  
**Task:** Create `docker-compose.yml`:
```yaml
version: '3'
services:
  web:
    image: nginx
    ports:
      - "8080:80"
```  
**Concept:** Compose file basics  
**Expected:** File created

**Exercise 204: Start Services with Compose** ⭐  
**Goal:** Launch all containers  
**Task:** Type `docker-compose up`  
**Concept:** Starting with Compose  
**Expected:** Services start, logs show

**Exercise 205: Run Compose in Background**  
**Goal:** Detached mode  
**Task:** Type `docker-compose up -d`  
**Concept:** Background execution  
**Expected:** Services start, terminal returns

**Exercise 206: View Compose Logs**  
**Goal:** See all service logs  
**Task:** Type `docker-compose logs`  
**Concept:** Aggregated logging  
**Expected:** Shows logs from all services

**Exercise 207: Follow Compose Logs**  
**Goal:** Monitor logs live  
**Task:** Type `docker-compose logs -f`  
**Concept:** Live log streaming  
**Expected:** Real-time logs from all services

**Exercise 208: Stop Compose Services**  
**Goal:** Stop all containers  
**Task:** Type `docker-compose stop`  
**Concept:** Stopping services  
**Expected:** All containers stopped

**Exercise 209: Remove Compose Services**  
**Goal:** Delete containers  
**Task:** Type `docker-compose down`  
**Concept:** Complete cleanup  
**Expected:** Containers removed

**Exercise 210: Define Multiple Services** ⭐  
**Goal:** Run related containers  
**Task:** Add database service to docker-compose.yml:
```yaml
services:
  web:
    image: nginx
  db:
    image: postgres
```  
**Concept:** Multi-service definition  
**Expected:** Both services defined

**Exercise 211: Environment Variables in Compose** ⭐  
**Goal:** Configure services  
**Task:** Add environment section:
```yaml
db:
  image: postgres
  environment:
    POSTGRES_PASSWORD: secret
```  
**Concept:** Container configuration  
**Expected:** Variable passed to container

**Exercise 212: Volume Mounting in Compose** ⭐💡  
**Goal:** Persist data  
**Task:** Add volumes:
```yaml
db:
  image: postgres
  volumes:
    - db-data:/var/lib/postgresql/data
volumes:
  db-data:
```  
**Concept:** Data persistence  
**Expected:** Data survives container restarts

**Exercise 213: Bind Mount in Compose**  
**Goal:** Mount local files  
**Task:** Add bind mount:
```yaml
web:
  image: nginx
  volumes:
    - ./html:/usr/share/nginx/html
```  
**Concept:** Local file mounting  
**Expected:** Local files accessible in container

**Exercise 214: Service Dependencies** ⭐  
**Goal:** Control startup order  
**Task:** Add depends_on:
```yaml
web:
  image: nginx
  depends_on:
    - db
```  
**Concept:** Service ordering  
**Expected:** db starts before web

**Exercise 215: Build Image in Compose**  
**Goal:** Use custom image  
**Task:** Replace `image:` with `build: .`  
**Concept:** Building with Compose  
**Expected:** Builds from Dockerfile

**Exercise 216: Specify Build Context**  
**Goal:** Custom build location  
**Task:** Use:
```yaml
build:
  context: ./app
  dockerfile: Dockerfile
```  
**Concept:** Build configuration  
**Expected:** Builds from specified path

**Exercise 217: Override Command in Compose**  
**Goal:** Change container command  
**Task:** Add `command: python app.py`  
**Concept:** Command override  
**Expected:** Custom command runs

**Exercise 218: Network Between Services** 💡  
**Goal:** Understand service communication  
**Task:** Read: Services can reach each other by service name (e.g., http://db:5432)  
**Concept:** Compose networking  
**No Action:** Just understanding

**Exercise 219: Scale Services**  
**Goal:** Run multiple instances  
**Task:** Type `docker-compose up --scale web=3`  
**Concept:** Service scaling  
**Expected:** 3 web containers run

**Exercise 220: View Compose Processes**  
**Goal:** See running services  
**Task:** Type `docker-compose ps`  
**Concept:** Service status  
**Expected:** Shows service states

**Exercise 221: Execute Command in Compose Service** ⭐  
**Goal:** Run command in service  
**Task:** Type `docker-compose exec web bash`  
**Concept:** Service interaction  
**Expected:** Shell in web container

**Exercise 222: Restart Single Service**  
**Goal:** Restart one service  
**Task:** Type `docker-compose restart web`  
**Concept:** Individual service control  
**Expected:** Only web restarts

**Exercise 223: Pull Images for Compose**  
**Goal:** Update images  
**Task:** Type `docker-compose pull`  
**Concept:** Image updating  
**Expected:** All images updated

**Exercise 224: Validate Compose File**  
**Goal:** Check syntax  
**Task:** Type `docker-compose config`  
**Concept:** Configuration validation  
**Expected:** Shows parsed config or errors

**Exercise 225: Full Stack Application** ⭐🎯  
**Goal:** Complete multi-tier app  
**Task:** Create compose file with web, API, and database services  
**Concept:** Real-world application  
**Expected:** Working full-stack app

## 🐧 PHASE 3: Linux & Servers (Continued)

### Week 6: Networking & Web Servers (Continued)

**Exercise 136: Download File with wget**  
**Goal:** Fetch file from web  
**Task:** Type `wget https://example.com/file.txt`  
**Concept:** File downloading  
**Expected:** File downloaded to current directory

**Exercise 137: Download with curl**  
**Goal:** Alternative download method  
**Task:** Type `curl -O https://example.com/file.txt`  
**Concept:** curl for downloads  
**Expected:** File downloaded

**Exercise 138: Make HTTP Request**  
**Goal:** Test web endpoint  
**Task:** Type `curl https://api.github.com`  
**Concept:** API testing  
**Expected:** Shows JSON response

**Exercise 139: Install Nginx** ⭐  
**Goal:** Set up web server  
**Task:** Type `sudo apt install nginx`  
**Concept:** Web server installation  
**Expected:** Nginx installed

**Exercise 140: Start Nginx**  
**Goal:** Launch web server  
**Task:** Type `sudo systemctl start nginx`  
**Concept:** Starting web services  
**Expected:** Nginx running

**Exercise 141: Test Nginx in Browser**  
**Goal:** Verify web server works  
**Task:** Open browser, go to `http://localhost`  
**Concept:** Web server verification  
**Expected:** See "Welcome to nginx" page

**Exercise 142: Find Nginx Config** ⭐💡  
**Goal:** Locate configuration  
**Task:** Type `ls /etc/nginx/`  
**Concept:** Config file locations  
**Expected:** Shows nginx.conf and other files

**Exercise 143: View Nginx Config**  
**Goal:** Read web server configuration  
**Task:** Type `cat /etc/nginx/nginx.conf`  
**Concept:** Configuration inspection  
**Expected:** Shows nginx settings

**Exercise 144: Create HTML File**  
**Goal:** Make a web page  
**Task:** Create `index.html` with basic HTML in `/var/www/html/`  
**Concept:** Web content creation  
**Expected:** File created

**Exercise 145: Set File Permissions for Web**  
**Goal:** Make file web-accessible  
**Task:** Type `sudo chmod 644 /var/www/html/index.html`  
**Concept:** Web file permissions  
**Expected:** File readable by web server

**Exercise 146: Test Custom HTML**  
**Goal:** View your page  
**Task:** Visit `http://localhost` in browser  
**Concept:** Testing web changes  
**Expected:** Your HTML displays

**Exercise 147: Check Nginx Logs** ⭐  
**Goal:** View web server logs  
**Task:** Type `sudo tail -f /var/log/nginx/access.log`  
**Concept:** Web server logging  
**Expected:** Shows access requests

**Exercise 148: View Error Logs**  
**Goal:** Check for errors  
**Task:** Type `sudo tail -f /var/log/nginx/error.log`  
**Concept:** Error monitoring  
**Expected:** Shows error messages

**Exercise 149: Reload Nginx Config**  
**Goal:** Apply config changes without restart  
**Task:** Type `sudo systemctl reload nginx`  
**Concept:** Graceful reload  
**Expected:** New config loaded

**Exercise 150: Configure Firewall** ⭐🎯  
**Goal:** Control network access  
**Task:** Type `sudo ufw allow 80/tcp`  
**Concept:** Firewall configuration  
**Expected:** Port 80 allowed

---

## 🐳 PHASE 4: Containers & Docker (Exercises 151-225)

### Week 7: Docker Fundamentals

**Exercise 151: What is a Container?** 💡  
**Goal:** Understand containerization  
**Task:** Read: Container is like a lightweight VM - isolated environment with app and dependencies  
**Concept:** Container concept  
**No Action:** Just understanding

**Exercise 152: Why Docker?** 💡  
**Goal:** Understand Docker benefits  
**Task:** Read: Docker ensures "it works on my machine" = "it works everywhere"  
**Concept:** Docker advantages  
**No Action:** Just understanding

**Exercise 153: Install Docker** ⭐  
**Goal:** Set up Docker  
**Task:** Follow docs.docker.com installation for your OS  
**Concept:** Docker installation  
**Expected:** Docker installed

**Exercise 154: Verify Docker Installation**  
**Goal:** Check Docker works  
**Task:** Type `docker --version`  
**Concept:** Installation verification  
**Expected:** Shows Docker version

**Exercise 155: Run First Container** ⭐  
**Goal:** Start a container  
**Task:** Type `docker run hello-world`  
**Concept:** Running containers  
**Expected:** Downloads and runs hello-world image

**Exercise 156: List Running Containers**  
**Goal:** See active containers  
**Task:** Type `docker ps`  
**Concept:** Container listing  
**Expected:** Shows running containers (might be empty)

**Exercise 157: List All Containers**  
**Goal:** See all containers including stopped  
**Task:** Type `docker ps -a`  
**Concept:** Complete container list  
**Expected:** Shows all containers

**Exercise 158: Run Container in Background** ⭐  
**Goal:** Detached mode  
**Task:** Type `docker run -d nginx`  
**Concept:** Background containers with `-d`  
**Expected:** Returns container ID

**Exercise 159: Run Container with Name**  
**Goal:** Give container a name  
**Task:** Type `docker run -d --name my-nginx nginx`  
**Concept:** Named containers  
**Expected:** Container named "my-nginx"

**Exercise 160: View Container Logs** ⭐  
**Goal:** See container output  
**Task:** Type `docker logs my-nginx`  
**Concept:** Container logging  
**Expected:** Shows nginx logs

**Exercise 161: Follow Container Logs**  
**Goal:** Monitor logs in real-time  
**Task:** Type `docker logs -f my-nginx`  
**Concept:** Log streaming  
**Expected:** Shows logs as they happen

**Exercise 162: Stop Container**  
**Goal:** Stop running container  
**Task:** Type `docker stop my-nginx`  
**Concept:** Container stopping  
**Expected:** Container stops gracefully

**Exercise 163: Start Stopped Container**  
**Goal:** Restart existing container  
**Task:** Type `docker start my-nginx`  
**Concept:** Container restarting  
**Expected:** Container starts again

**Exercise 164: Remove Container** ⭐  
**Goal:** Delete container  
**Task:** Type `docker rm my-nginx`  
**Concept:** Container removal  
**Expected:** Container deleted (must be stopped first)

**Exercise 165: Force Remove Running Container**  
**Goal:** Delete without stopping  
**Task:** Type `docker rm -f my-nginx`  
**Concept:** Forced removal  
**Expected:** Running container removed

**Exercise 166: List Docker Images** ⭐  
**Goal:** See downloaded images  
**Task:** Type `docker images`  
**Concept:** Image listing  
**Expected:** Shows available images

**Exercise 167: Pull an Image**  
**Goal:** Download image without running  
**Task:** Type `docker pull ubuntu`  
**Concept:** Image pulling  
**Expected:** Ubuntu image downloaded

**Exercise 168: Run Interactive Container** ⭐💡  
**Goal:** Get shell access  
**Task:** Type `docker run -it ubuntu bash`  
**Concept:** Interactive mode with `-it`  
**Expected:** Inside Ubuntu container shell

**Exercise 169: Exit Container**  
**Goal:** Leave container shell  
**Task:** Type `exit` in container  
**Concept:** Exiting interactive mode  
**Expected:** Back to host system

**Exercise 170: Execute Command in Running Container** ⭐  
**Goal:** Run command in container  
**Task:** Type `docker exec my-nginx ls /etc/nginx`  
**Concept:** docker exec  
**Expected:** Lists nginx config files

**Exercise 171: Get Shell in Running Container**  
**Goal:** Access running container  
**Task:** Type `docker exec -it my-nginx bash`  
**Concept:** Interactive exec  
**Expected:** Shell inside running container

**Exercise 172: Inspect Container** ⭐  
**Goal:** See detailed info  
**Task:** Type `docker inspect my-nginx`  
**Concept:** Container inspection  
**Expected:** JSON with all details

**Exercise 173: View Container Stats**  
**Goal:** Monitor resource usage  
**Task:** Type `docker stats`  
**Concept:** Resource monitoring  
**Expected:** Live CPU/memory usage

**Exercise 174: Port Mapping** ⭐💡  
**Goal:** Expose container port  
**Task:** Type `docker run -d -p 8080:80 nginx`  
**Concept:** Port publishing with `-p`  
**Expected:** Access nginx at localhost:8080

**Exercise 175: Test Port Mapping**  
**Goal:** Verify port works  
**Task:** Open browser to `http://localhost:8080`  
**Concept:** Port accessibility  
**Expected:** See nginx welcome page

---

### Week 8: Docker Images & Dockerfiles

**Exercise 176: What is a Dockerfile?** 💡  
**Goal:** Understand Dockerfiles  
**Task:** Read: Dockerfile is a recipe to build a Docker image  
**Concept:** Dockerfile purpose  
**No Action:** Just understanding

**Exercise 177: Create First Dockerfile** ⭐  
**Goal:** Write image definition  
**Task:** Create file named `Dockerfile` with:
```dockerfile
FROM ubuntu:latest
RUN apt-get update
CMD ["echo", "Hello from my image!"]
```  
**Concept:** Dockerfile basics  
**Expected:** File created

**Exercise 178: Build Docker Image** ⭐  
**Goal:** Create image from Dockerfile  
**Task:** Type `docker build -t my-first-image .`  
**Concept:** Image building  
**Expected:** Image built successfully

**Exercise 179: Run Your Custom Image**  
**Goal:** Use your image  
**Task:** Type `docker run my-first-image`  
**Concept:** Running custom images  
**Expected:** Prints "Hello from my image!"

**Exercise 180: Understand FROM Instruction** 💡  
**Goal:** Learn base images  
**Task:** Read: FROM specifies the base image to start from  
**Concept:** Base images  
**No Action:** Just understanding

**Exercise 181: Understand RUN Instruction**  
**Goal:** Learn build commands  
**Task:** Read: RUN executes commands during image build  
**Concept:** Build-time commands  
**No Action:** Just understanding

**Exercise 182: Understand CMD Instruction**  
**Goal:** Learn default command  
**Task:** Read: CMD specifies the default command when container starts  
**Concept:** Container startup command  
**No Action:** Just understanding

**Exercise 183: COPY Files to Image** ⭐  
**Goal:** Add files to image  
**Task:** Create `app.txt`, add to Dockerfile: `COPY app.txt /app/`  
**Concept:** COPY instruction  
**Expected:** File included in image

**Exercise 184: Set Working Directory**  
**Goal:** Define default directory  
**Task:** Add to Dockerfile: `WORKDIR /app`  
**Concept:** WORKDIR instruction  
**Expected:** Commands run from /app

**Exercise 185: Expose Port in Dockerfile**  
**Goal:** Document port usage  
**Task:** Add to Dockerfile: `EXPOSE 8080`  
**Concept:** EXPOSE instruction  
**Expected:** Port documented (still need -p to publish)

**Exercise 186: Use ENV Variables** ⭐  
**Goal:** Set environment variables  
**Task:** Add to Dockerfile: `ENV APP_NAME=MyApp`  
**Concept:** ENV instruction  
**Expected:** Variable available in container

**Exercise 187: Multi-line RUN**  
**Goal:** Optimize build commands  
**Task:** Use `RUN apt-get update && apt-get install -y curl`  
**Concept:** Command chaining  
**Expected:** Single layer created

**Exercise 188: Understand Image Layers** 💡  
**Goal:** Learn layer concept  
**Task:** Read: Each Dockerfile instruction creates a layer. Layers are cached for faster builds  
**Concept:** Image layers  
**No Action:** Just understanding

**Exercise 189: Build with No Cache**  
**Goal:** Force fresh build  
**Task:** Type `docker build --no-cache -t my-image .`  
**Concept:** Cache control  
**Expected:** Rebuilds everything

**Exercise 190: Tag Image with Version** ⭐  
**Goal:** Version your images  
**Task:** Type `docker build -t my-image:v1.0 .`  
**Concept:** Image tagging  
**Expected:** Image tagged with version

**Exercise 191: Create Multiple Tags**  
**Goal:** Tag same image multiple times  
**Task:** Type `docker tag my-image:v1.0 my-image:latest`  
**Concept:** Image tagging  
**Expected:** Two tags point to same image

**Exercise 192: Remove Image**  
**Goal:** Delete image  
**Task:** Type `docker rmi my-image:v1.0`  
**Concept:** Image removal  
**Expected:** Image deleted

**Exercise 193: Create .dockerignore** ⭐  
**Goal:** Exclude files from build  
**Task:** Create `.dockerignore` file, add `*.log` and `node_modules/`  
**Concept:** Build context filtering  
**Expected:** Files ignored during build

**Exercise 194: Build Simple Web App Image**  
**Goal:** Create web app container  
**Task:** Dockerfile with nginx and custom HTML  
**Concept:** Web app containerization  
**Expected:** Working web app in container

**Exercise 195: Use ARG for Build Variables** ⭐  
**Goal:** Parameterize build  
**Task:** Add `ARG VERSION=1.0` to Dockerfile  
**Concept:** Build arguments  
**Expected:** Variable available during build only

**Exercise 196: Pass ARG at Build Time**  
**Goal:** Override ARG values  
**Task:** Type `docker build --build-arg VERSION=2.0 -t my-image .`  
**Concept:** Build-time arguments  
**Expected:** Custom value used

**Exercise 197: Multi-stage Build** ⭐💡  
**Goal:** Optimize image size  
**Task:** Create Dockerfile with multiple FROM statements  
**Concept:** Multi-stage builds  
**Expected:** Smaller final image

**Exercise 198: ENTRYPOINT vs CMD** 💡  
**Goal:** Understand difference  
**Task:** Read: ENTRYPOINT sets fixed command, CMD provides default arguments  
**Concept:** Startup command options  
**No Action:** Just understanding

**Exercise 199: Use ENTRYPOINT**  
**Goal:** Set fixed startup command  
**Task:** Add `ENTRYPOINT ["nginx", "-g", "daemon off;"]` to Dockerfile  
**Concept:** ENTRYPOINT instruction  
**Expected:** Container always runs nginx

**Exercise 200: Health Check** ⭐  
**Goal:** Monitor container health  
**Task:** Add `HEALTHCHECK --interval=30s CMD curl -f http://localhost/ || exit 1`  
**Concept:** Container health checking  
**Expected:** Docker monitors container health

---

### Week 9: Docker Compose

**Exercise 201: What is Docker Compose?** 💡  
**Goal:** Understand multi-container apps  
**Task:** Read: Docker Compose runs multiple containers together as one application  
**Concept:** Docker Compose purpose  
**No Action:** Just understanding

**Exercise 202: Install Docker Compose**  
**Goal:** Get Docker Compose  
**Task:** Usually comes with Docker Desktop, or install separately  
**Concept:** Tool installation  
**Expected:** `docker-compose --version` works

**Exercise 203: Create First docker-compose.yml** ⭐  
**Goal:** Define multi-container app  
**Task:** Create `docker-compose.yml`:
```yaml
version: '3'
services:
  web:
    image: nginx
    ports:
      - "8080:80"
```  
**Concept:** Compose file basics  
**Expected:** File created

**Exercise 204: Start Services with Compose** ⭐  
**Goal:** Launch all containers  
**Task:** Type `docker-compose up`  
**Concept:** Starting with Compose  
**Expected:** Services start, logs show

**Exercise 205: Run Compose in Background**  
**Goal:** Detached mode  
**Task:** Type `docker-compose up -d`  
**Concept:** Background execution  
**Expected:** Services start, terminal returns

**Exercise 206: View Compose Logs**  
**Goal:** See all service logs  
**Task:** Type `docker-compose logs`  
**Concept:** Aggregated logging  
**Expected:** Shows logs from all services

**Exercise 207: Follow Compose Logs**  
**Goal:** Monitor logs live  
**Task:** Type `docker-compose logs -f`  
**Concept:** Live log streaming  
**Expected:** Real-time logs from all services

**Exercise 208: Stop Compose Services**  
**Goal:** Stop all containers  
**Task:** Type `docker-compose stop`  
**Concept:** Stopping services  
**Expected:** All containers stopped

**Exercise 209: Remove Compose Services**  
**Goal:** Delete containers  
**Task:** Type `docker-compose down`  
**Concept:** Complete cleanup  
**Expected:** Containers removed

**Exercise 210: Define Multiple Services** ⭐  
**Goal:** Run related containers  
**Task:** Add database service to docker-compose.yml:
```yaml
services:
  web:
    image: nginx
  db:
    image: postgres
```  
**Concept:** Multi-service definition  
**Expected:** Both services defined

**Exercise 211: Environment Variables in Compose** ⭐  
**Goal:** Configure services  
**Task:** Add environment section:
```yaml
db:
  image: postgres
  environment:
    POSTGRES_PASSWORD: secret
```  
**Concept:** Container configuration  
**Expected:** Variable passed to container

**Exercise 212: Volume Mounting in Compose** ⭐💡  
**Goal:** Persist data  
**Task:** Add volumes:
```yaml
db:
  image: postgres
  volumes:
    - db-data:/var/lib/postgresql/data
volumes:
  db-data:
```  
**Concept:** Data persistence  
**Expected:** Data survives container restarts

**Exercise 213: Bind Mount in Compose**  
**Goal:** Mount local files  
**Task:** Add bind mount:
```yaml
web:
  image: nginx
  volumes:
    - ./html:/usr/share/nginx/html
```  
**Concept:** Local file mounting  
**Expected:** Local files accessible in container

**Exercise 214: Service Dependencies** ⭐  
**Goal:** Control startup order  
**Task:** Add depends_on:
```yaml
web:
  image: nginx
  depends_on:
    - db
```  
**Concept:** Service ordering  
**Expected:** db starts before web

**Exercise 215: Build Image in Compose**  
**Goal:** Use custom image  
**Task:** Replace `image:` with `build: .`  
**Concept:** Building with Compose  
**Expected:** Builds from Dockerfile

**Exercise 216: Specify Build Context**  
**Goal:** Custom build location  
**Task:** Use:
```yaml
build:
  context: ./app
  dockerfile: Dockerfile
```  
**Concept:** Build configuration  
**Expected:** Builds from specified path

**Exercise 217: Override Command in Compose**  
**Goal:** Change container command  
**Task:** Add `command: python app.py`  
**Concept:** Command override  
**Expected:** Custom command runs

**Exercise 218: Network Between Services** 💡  
**Goal:** Understand service communication  
**Task:** Read: Services can reach each other by service name (e.g., http://db:5432)  
**Concept:** Compose networking  
**No Action:** Just understanding

**Exercise 219: Scale Services**  
**Goal:** Run multiple instances  
**Task:** Type `docker-compose up --scale web=3`  
**Concept:** Service scaling  
**Expected:** 3 web containers run

**Exercise 220: View Compose Processes**  
**Goal:** See running services  
**Task:** Type `docker-compose ps`  
**Concept:** Service status  
**Expected:** Shows service states

**Exercise 221: Execute Command in Compose Service** ⭐  
**Goal:** Run command in service  
**Task:** Type `docker-compose exec web bash`  
**Concept:** Service interaction  
**Expected:** Shell in web container

**Exercise 222: Restart Single Service**  
**Goal:** Restart one service  
**Task:** Type `docker-compose restart web`  
**Concept:** Individual service control  
**Expected:** Only web restarts

**Exercise 223: Pull Images for Compose**  
**Goal:** Update images  
**Task:** Type `docker-compose pull`  
**Concept:** Image updating  
**Expected:** All images updated

**Exercise 224: Validate Compose File**  
**Goal:** Check syntax  
**Task:** Type `docker-compose config`  
**Concept:** Configuration validation  
**Expected:** Shows parsed config or errors

**Exercise 225: Full Stack Application** ⭐🎯  
**Goal:** Complete multi-tier app  
**Task:** Create compose file with web, API, and database services  
**Concept:** Real-world application  
**Expected:** Working full-stack app

---

## ☁️ PHASE 5: Cloud Basics & AWS (Exercises 226-300)

### Week 10: Cloud Computing Fundamentals

**Exercise 226: What is Cloud Computing?** 💡  
**Goal:** Understand the cloud  
**Task:** Read: Cloud = renting computers/storage/services over internet instead of owning hardware  
**Concept:** Cloud computing basics  
**No Action:** Just understanding

**Exercise 227: Cloud Service Models** 💡  
**Goal:** Learn IaaS, PaaS, SaaS  
**Task:** Read: IaaS=rent VMs, PaaS=rent platform (no server management), SaaS=use app (Gmail, Slack)  
**Concept:** Service models  
**No Action:** Just understanding

**Exercise 228: Major Cloud Providers** 💡  
**Goal:** Know the players  
**Task:** Read: AWS (Amazon), Azure (Microsoft), GCP (Google) are the big three  
**Concept:** Cloud vendors  
**No Action:** Just understanding

**Exercise 229: Create AWS Free Tier Account** ⭐  
**Goal:** Get AWS access  
**Task:** Sign up at aws.amazon.com  
**Concept:** Cloud account setup  
**Expected:** AWS account created  
**Warning:** Requires credit card (free tier available)

**Exercise 230: AWS Management Console**  
**Goal:** Navigate AWS UI  
**Task:** Log into AWS Console, explore the dashboard  
**Concept:** Cloud console  
**Expected:** See AWS services

**Exercise 231: Understand AWS Regions** 💡  
**Goal:** Learn geographic distribution  
**Task:** Read: Regions are geographic locations with multiple data centers  
**Concept:** AWS regions  
**No Action:** Just understanding

**Exercise 232: Select a Region**  
**Goal:** Choose working region  
**Task:** In console, select region closest to you (top-right dropdown)  
**Concept:** Region selection  
**Expected:** Region set

**Exercise 233: What is EC2?** ⭐💡  
**Goal:** Understand virtual servers  
**Task:** Read: EC2 = Elastic Compute Cloud = virtual servers in the cloud  
**Concept:** AWS EC2  
**No Action:** Just understanding

**Exercise 234: Launch First EC2 Instance** ⭐  
**Goal:** Create virtual server  
**Task:** EC2 Console → Launch Instance → Choose Amazon Linux 2  
**Concept:** VM creation  
**Expected:** Instance launching

**Exercise 235: Choose Instance Type**  
**Goal:** Select server size  
**Task:** Select t2.micro (free tier)  
**Concept:** Instance sizing  
**Expected:** Free tier instance selected

**Exercise 236: Create Key Pair** ⭐💡  
**Goal:** Set up SSH access  
**Task:** Create new key pair, download .pem file  
**Concept:** SSH key authentication  
**Expected:** Key file downloaded  
**Warning:** Keep this file safe!

**Exercise 237: Configure Security Group** ⭐  
**Goal:** Set firewall rules  
**Task:** Allow SSH (port 22) from your IP  
**Concept:** Cloud firewall  
**Expected:** SSH access configured

**Exercise 238: Launch Instance**  
**Goal:** Start the server  
**Task:** Review and launch  
**Concept:** Instance provisioning  
**Expected:** Instance running

**Exercise 239: View Running Instances**  
**Goal:** See your servers  
**Task:** Go to EC2 → Instances  
**Concept:** Instance management  
**Expected:** See your instance

**Exercise 240: Get Instance Public IP**  
**Goal:** Find server address  
**Task:** Click instance, copy Public IPv4 address  
**Concept:** Public IP addresses  
**Expected:** IP address like 3.84.123.45

**Exercise 241: Set Key Permissions** ⭐  
**Goal:** Secure SSH key  
**Task:** Type `chmod 400 your-key.pem` (Mac/Linux)  
**Concept:** Key security  
**Expected:** Key permissions restricted

**Exercise 242: SSH to EC2 Instance** ⭐  
**Goal:** Connect to server  
**Task:** Type `ssh -i your-key.pem ec2-user@YOUR-IP`  
**Concept:** Remote server access  
**Expected:** Connected to EC2 instance

**Exercise 243: Update EC2 Packages**  
**Goal:** Update server software  
**Task:** On EC2, type `sudo yum update -y`  
**Concept:** Server maintenance  
**Expected:** Packages updated

**Exercise 244: Install Software on EC2**  
**Goal:** Add tools to server  
**Task:** Type `sudo yum install -y git`  
**Concept:** Server configuration  
**Expected:** Git installed

**Exercise 245: Stop EC2 Instance**  
**Goal:** Pause server (saves money)  
**Task:** In Console, select instance → Actions → Stop  
**Concept:** Instance lifecycle  
**Expected:** Instance stopped  
**Note:** No charges while stopped

**Exercise 246: Start Stopped Instance**  
**Goal:** Resume server  
**Task:** Actions → Start  
**Concept:** Instance management  
**Expected:** Instance running  
**Note:** Public IP may change

**Exercise 247: Elastic IP** ⭐💡  
**Goal:** Get permanent IP  
**Task:** EC2 → Elastic IPs → Allocate  
**Concept:** Static IP addresses  
**Expected:** Fixed IP allocated  
**Warning:** Charged if not attached to running instance

**Exercise 248: Associate Elastic IP**  
**Goal:** Attach IP to instance  
**Task:** Select EIP → Actions → Associate → Choose instance  
**Concept:** IP assignment  
**Expected:** Instance has permanent IP

**Exercise 249: Terminate EC2 Instance**  
**Goal:** Delete server  
**Task:** Actions → Terminate  
**Concept:** Resource cleanup  
**Expected:** Instance deleted  
**Warning:** Cannot be undone!

**Exercise 250: What is S3?** ⭐💡  
**Goal:** Understand object storage  
**Task:** Read: S3 = Simple Storage Service = unlimited file storage in the cloud  
**Concept:** AWS S3  
**No Action:** Just understanding

**Exercise 251: Create S3 Bucket** ⭐  
**Goal:** Make storage container  
**Task:** S3 Console → Create bucket → Enter unique name  
**Concept:** Bucket creation  
**Expected:** Bucket created  
**Note:** Bucket names must be globally unique

**Exercise 252: Upload File to S3**  
**Goal:** Store a file  
**Task:** Click bucket → Upload → Select file  
**Concept:** Object storage  
**Expected:** File uploaded

**Exercise 253: Download from S3**  
**Goal:** Retrieve file  
**Task:** Click file → Download  
**Concept:** Object retrieval  
**Expected:** File downloaded

**Exercise 254: Make S3 Object Public** ⭐  
**Goal:** Allow public access  
**Task:** Click file → Make public  
**Concept:** Access control  
**Expected:** File accessible via URL  
**Warning:** Anyone can access!

**Exercise 255: S3 Bucket Permissions**  
**Goal:** Configure bucket access  
**Task:** Bucket → Permissions → Review settings  
**Concept:** Bucket policies  
**Expected:** Understand access rules

**Exercise 256: Delete S3 Object**  
**Goal:** Remove file  
**Task:** Select object → Delete  
**Concept:** Object management  
**Expected:** File deleted

**Exercise 257: S3 Versioning** ⭐  
**Goal:** Track file versions  
**Task:** Bucket → Properties → Enable versioning  
**Concept:** Version control for files  
**Expected:** Versioning enabled

**Exercise 258: AWS CLI Installation** ⭐  
**Goal:** Install command-line tool  
**Task:** Download and install AWS CLI from aws.amazon.com/cli  
**Concept:** CLI tools  
**Expected:** `aws --version` works

**Exercise 259: Configure AWS CLI** ⭐  
**Goal:** Set up credentials  
**Task:** Type `aws configure`, enter access key, secret key, region  
**Concept:** CLI configuration  
**Expected:** Credentials stored

**Exercise 260: List S3 Buckets via CLI**  
**Goal:** Use CLI for S3  
**Task:** Type `aws s3 ls`  
**Concept:** CLI commands  
**Expected:** Shows your buckets

**Exercise 261: Upload to S3 via CLI**  
**Goal:** Copy file with CLI  
**Task:** Type `aws s3 cp file.txt s3://your-bucket/`  
**Concept:** CLI file operations  
**Expected:** File uploaded

**Exercise 262: Sync Folder to S3**  
**Goal:** Batch upload  
**Task:** Type `aws s3 sync ./folder s3://your-bucket/`  
**Concept:** Bulk operations  
**Expected:** Entire folder uploaded

**Exercise 263: What is IAM?** ⭐💡  
**Goal:** Understand access management  
**Task:** Read: IAM = Identity and Access Management = control who can do what in AWS  
**Concept:** AWS IAM  
**No Action:** Just understanding

**Exercise 264: View IAM Users**  
**Goal:** See user accounts  
**Task:** IAM Console → Users  
**Concept:** User management  
**Expected:** See users (including yourself)

**Exercise 265: Create IAM User**  
**Goal:** Add new user  
**Task:** Users → Add user → Set name  
**Concept:** User creation  
**Expected:** New user created

**Exercise 266: Enable Console Access**  
**Goal:** Allow web login  
**Task:** When creating user, check "AWS Console access"  
**Concept:** Access types  
**Expected:** User can log in

**Exercise 267: Enable Programmatic Access**  
**Goal:** Generate access keys  
**Task:** Check "Programmatic access" when creating user  
**Concept:** API access  
**Expected:** Access key and secret generated

**Exercise 268: IAM Groups** ⭐  
**Goal:** Organize users  
**Task:** IAM → Groups → Create group  
**Concept:** Group management  
**Expected:** Group created

**Exercise 269: Add User to Group**  
**Goal:** Assign group membership  
**Task:** Select user → Add to group  
**Concept:** Group assignment  
**Expected:** User in group

**Exercise 270: IAM Policies** ⭐💡  
**Goal:** Understand permissions  
**Task:** Read: Policies define what actions are allowed (JSON documents)  
**Concept:** Policy-based access  
**No Action:** Just understanding

**Exercise 271: Attach Policy to User**  
**Goal:** Grant permissions  
**Task:** User → Add permissions → Attach policies directly  
**Concept:** Permission assignment  
**Expected:** User has new permissions

**Exercise 272: Managed Policies**  
**Goal:** Use pre-made policies  
**Task:** Attach "AmazonS3ReadOnlyAccess" policy  
**Concept:** AWS-managed policies  
**Expected:** User can read S3

**Exercise 273: Principle of Least Privilege** 💡  
**Goal:** Security best practice  
**Task:** Read: Only grant minimum permissions needed for the job  
**Concept:** Security principle  
**No Action:** Just understanding

**Exercise 274: MFA for Root Account** ⭐  
**Goal:** Secure root access  
**Task:** IAM Dashboard → Activate MFA on root  
**Concept:** Multi-factor authentication  
**Expected:** MFA enabled

--be continued
