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

# 🚀 DevOps Tiny Steps: 600 Exercises (Continued - Local DevOps Focus)

---

## 🔄 PHASE 5: CI/CD & Automation (Exercises 226-300)

### Week 10: Continuous Integration Basics

**Exercise 226: What is CI/CD?** ⭐💡  
**Goal:** Understand automation  
**Task:** Read: CI = Continuous Integration (auto-test code changes), CD = Continuous Delivery (auto-deploy)  
**Concept:** CI/CD fundamentals  
**No Action:** Just understanding

**Exercise 227: What is Jenkins?** 💡  
**Goal:** Learn CI/CD tools  
**Task:** Read: Jenkins is an automation server for building, testing, and deploying code  
**Concept:** Jenkins overview  
**No Action:** Just understanding

**Exercise 228: Install Java** ⭐  
**Goal:** Jenkins prerequisite  
**Task:** Install Java JDK 11 or later  
**Concept:** Dependency management  
**Expected:** `java -version` works

**Exercise 229: Download Jenkins**  
**Goal:** Get Jenkins  
**Task:** Download Jenkins WAR file from jenkins.io  
**Concept:** Tool acquisition  
**Expected:** jenkins.war downloaded

**Exercise 230: Start Jenkins** ⭐  
**Goal:** Launch Jenkins server  
**Task:** Type `java -jar jenkins.war`  
**Concept:** Server startup  
**Expected:** Jenkins running on localhost:8080

**Exercise 231: Access Jenkins UI**  
**Goal:** Open Jenkins interface  
**Task:** Open browser to `http://localhost:8080`  
**Concept:** Web-based tools  
**Expected:** Jenkins setup wizard

**Exercise 232: Unlock Jenkins**  
**Goal:** Initial setup  
**Task:** Copy password from terminal or file, paste in UI  
**Concept:** Initial authentication  
**Expected:** Jenkins unlocked

**Exercise 233: Install Suggested Plugins**  
**Goal:** Get essential plugins  
**Task:** Click "Install suggested plugins"  
**Concept:** Plugin management  
**Expected:** Plugins installing

**Exercise 234: Create Admin User**  
**Goal:** Set up admin account  
**Task:** Fill in username, password, email  
**Concept:** User management  
**Expected:** Admin user created

**Exercise 235: Jenkins Dashboard**  
**Goal:** Navigate UI  
**Task:** Explore Jenkins dashboard  
**Concept:** Jenkins interface  
**Expected:** See main dashboard

**Exercise 236: Create First Jenkins Job** ⭐  
**Goal:** Make automation task  
**Task:** New Item → Freestyle project → Name: "hello-world"  
**Concept:** Job creation  
**Expected:** Job created

**Exercise 237: Add Build Step**  
**Goal:** Define what job does  
**Task:** Add build step → Execute shell → Type `echo "Hello from Jenkins!"`  
**Concept:** Build steps  
**Expected:** Command configured

**Exercise 238: Save and Build Job** ⭐  
**Goal:** Run your first job  
**Task:** Save → Click "Build Now"  
**Concept:** Job execution  
**Expected:** Job runs successfully

**Exercise 239: View Build Console Output**  
**Goal:** See job results  
**Task:** Click build number → Console Output  
**Concept:** Build logs  
**Expected:** See "Hello from Jenkins!"

**Exercise 240: View Build History**  
**Goal:** Track executions  
**Task:** Look at Build History section  
**Concept:** Job history  
**Expected:** See past builds

**Exercise 241: Trigger Build with Parameters** ⭐  
**Goal:** Parameterized jobs  
**Task:** Configure → This project is parameterized → Add String Parameter "NAME"  
**Concept:** Build parameters  
**Expected:** Parameter added

**Exercise 242: Use Parameter in Build**  
**Goal:** Reference parameter  
**Task:** In shell command: `echo "Hello $NAME"`  
**Concept:** Variable usage  
**Expected:** Parameter value used

**Exercise 243: Build with Parameter Value**  
**Goal:** Pass parameter  
**Task:** Build with Parameters → Enter name → Build  
**Concept:** Parameterized execution  
**Expected:** Custom message printed

**Exercise 244: Connect Jenkins to Git** ⭐  
**Goal:** Source code integration  
**Task:** Job → Source Code Management → Git → Enter repo URL  
**Concept:** SCM integration  
**Expected:** Git repo configured

**Exercise 245: Build from Git Repository**  
**Goal:** Auto-fetch code  
**Task:** Build job → Check workspace → Code pulled from Git  
**Concept:** Code checkout  
**Expected:** Repo cloned in workspace

**Exercise 246: Add Build Trigger - Poll SCM** ⭐  
**Goal:** Auto-detect changes  
**Task:** Build Triggers → Poll SCM → Schedule: `H/5 * * * *` (every 5 min)  
**Concept:** Automated triggers  
**Expected:** Jenkins checks for changes

**Exercise 247: Understanding Cron Syntax** 💡  
**Goal:** Learn scheduling  
**Task:** Read: `* * * * *` = minute hour day month weekday  
**Concept:** Cron expressions  
**No Action:** Just understanding

**Exercise 248: Test SCM Polling**  
**Goal:** Verify auto-trigger  
**Task:** Push commit to repo, wait 5 minutes  
**Concept:** SCM polling  
**Expected:** Jenkins auto-builds

**Exercise 249: Build After Another Job** ⭐  
**Goal:** Chain jobs  
**Task:** Create job2 → Build after other projects → Enter job1 name  
**Concept:** Job dependencies  
**Expected:** job2 triggers after job1

**Exercise 250: Install Additional Plugin**  
**Goal:** Extend Jenkins  
**Task:** Manage Jenkins → Plugins → Available → Search and install  
**Concept:** Plugin installation  
**Expected:** New plugin installed

---

### Week 11: Build Automation & Testing

**Exercise 251: What is a Build Tool?** 💡  
**Goal:** Understand build automation  
**Task:** Read: Build tools compile code, run tests, create deployable packages  
**Concept:** Build automation  
**No Action:** Just understanding

**Exercise 252: Install Maven** ⭐  
**Goal:** Get Java build tool  
**Task:** Download and install Maven from maven.apache.org  
**Concept:** Build tool setup  
**Expected:** `mvn -version` works

**Exercise 253: Create Simple Maven Project**  
**Goal:** Set up Java project  
**Task:** Type `mvn archetype:generate -DgroupId=com.example -DartifactId=my-app`  
**Concept:** Project scaffolding  
**Expected:** Project structure created

**Exercise 254: Understand pom.xml** 💡  
**Goal:** Learn Maven config  
**Task:** Read: pom.xml defines project dependencies and build configuration  
**Concept:** Build configuration  
**No Action:** Just understanding

**Exercise 255: Build Maven Project** ⭐  
**Goal:** Compile project  
**Task:** In project folder, type `mvn clean install`  
**Concept:** Build execution  
**Expected:** JAR file created in target/

**Exercise 256: Run Maven Tests**  
**Goal:** Execute unit tests  
**Task:** Type `mvn test`  
**Concept:** Test automation  
**Expected:** Tests run

**Exercise 257: Jenkins Maven Job** ⭐  
**Goal:** Build Java in Jenkins  
**Task:** New Item → Maven project → Configure Git → Build: `clean install`  
**Concept:** CI for Java  
**Expected:** Jenkins builds Maven project

**Exercise 258: Install Node.js and npm** ⭐  
**Goal:** Get JavaScript tools  
**Task:** Download and install Node.js from nodejs.org  
**Concept:** Runtime installation  
**Expected:** `node -v` and `npm -v` work

**Exercise 259: Create Node.js Project**  
**Goal:** Initialize JS project  
**Task:** Type `npm init -y`  
**Concept:** Package initialization  
**Expected:** package.json created

**Exercise 260: Install npm Package**  
**Goal:** Add dependency  
**Task:** Type `npm install express`  
**Concept:** Dependency management  
**Expected:** express installed, listed in package.json

**Exercise 261: Create npm Script** ⭐  
**Goal:** Define custom command  
**Task:** In package.json, add scripts: `"start": "node app.js"`  
**Concept:** Script definition  
**Expected:** Can run `npm start`

**Exercise 262: Run npm Script**  
**Goal:** Execute defined script  
**Task:** Type `npm start`  
**Concept:** Script execution  
**Expected:** Script runs

**Exercise 263: Add Test Script**  
**Goal:** Define test command  
**Task:** Add script: `"test": "echo 'Running tests'"`  
**Concept:** Test automation  
**Expected:** `npm test` works

**Exercise 264: Jenkins Node.js Job** ⭐  
**Goal:** Build JS in Jenkins  
**Task:** Freestyle job → Execute shell: `npm install && npm test`  
**Concept:** CI for Node.js  
**Expected:** Jenkins runs npm commands

**Exercise 265: Install Python pip** ⭐  
**Goal:** Get Python package manager  
**Task:** Install pip (usually comes with Python)  
**Concept:** Package manager setup  
**Expected:** `pip --version` works

**Exercise 266: Create requirements.txt**  
**Goal:** Define Python dependencies  
**Task:** Create file with package names (e.g., `flask==2.0.1`)  
**Concept:** Dependency specification  
**Expected:** requirements.txt created

**Exercise 267: Install from requirements.txt**  
**Goal:** Install all dependencies  
**Task:** Type `pip install -r requirements.txt`  
**Concept:** Batch installation  
**Expected:** All packages installed

**Exercise 268: Create Virtual Environment** ⭐💡  
**Goal:** Isolate Python dependencies  
**Task:** Type `python -m venv venv`  
**Concept:** Virtual environments  
**Expected:** venv/ folder created

**Exercise 269: Activate Virtual Environment**  
**Goal:** Use isolated environment  
**Task:** Type `source venv/bin/activate` (Mac/Linux) or `venv\Scripts\activate` (Windows)  
**Concept:** Environment activation  
**Expected:** (venv) in prompt

**Exercise 270: Deactivate Virtual Environment**  
**Goal:** Exit isolated environment  
**Task:** Type `deactivate`  
**Concept:** Environment management  
**Expected:** (venv) disappears

**Exercise 271: Jenkins Python Job** ⭐  
**Goal:** Build Python in Jenkins  
**Task:** Execute shell: `python -m venv venv && source venv/bin/activate && pip install -r requirements.txt`  
**Concept:** CI for Python  
**Expected:** Dependencies installed in Jenkins

**Exercise 272: What is pytest?** 💡  
**Goal:** Learn testing framework  
**Task:** Read: pytest is a popular Python testing framework  
**Concept:** Unit testing  
**No Action:** Just understanding

**Exercise 273: Install pytest**  
**Goal:** Get testing tool  
**Task:** Type `pip install pytest`  
**Concept:** Test framework setup  
**Expected:** pytest installed

**Exercise 274: Create Simple Test**  
**Goal:** Write first test  
**Task:** Create `test_sample.py`: `def test_addition(): assert 1 + 1 == 2`  
**Concept:** Test creation  
**Expected:** Test file created

**Exercise 275: Run pytest** ⭐  
**Goal:** Execute tests  
**Task:** Type `pytest`  
**Concept:** Test execution  
**Expected:** Tests pass

**Exercise 276: Jenkins Test Execution**  
**Goal:** Run tests in CI  
**Task:** Add to Jenkins: `pytest --verbose`  
**Concept:** Automated testing  
**Expected:** Tests run in Jenkins

**Exercise 277: Publish Test Results** ⭐  
**Goal:** Visualize test results  
**Task:** pytest with JUnit output: `pytest --junitxml=results.xml`  
**Concept:** Test reporting  
**Expected:** XML results generated

**Exercise 278: Jenkins Test Report**  
**Goal:** Display test results  
**Task:** Post-build action → Publish JUnit test result → `results.xml`  
**Concept:** Test visualization  
**Expected:** Test results in Jenkins UI

**Exercise 279: Code Coverage Basics** 💡  
**Goal:** Understand coverage  
**Task:** Read: Code coverage measures how much of your code is tested  
**Concept:** Quality metrics  
**No Action:** Just understanding

**Exercise 280: Install coverage.py**  
**Goal:** Get coverage tool  
**Task:** Type `pip install coverage`  
**Concept:** Coverage tooling  
**Expected:** coverage installed

**Exercise 281: Run Tests with Coverage** ⭐  
**Goal:** Measure coverage  
**Task:** Type `coverage run -m pytest`  
**Concept:** Coverage measurement  
**Expected:** Coverage data collected

**Exercise 282: View Coverage Report**  
**Goal:** See coverage results  
**Task:** Type `coverage report`  
**Concept:** Coverage reporting  
**Expected:** Shows coverage percentage

**Exercise 283: Generate HTML Coverage**  
**Goal:** Visual coverage report  
**Task:** Type `coverage html`  
**Concept:** Coverage visualization  
**Expected:** htmlcov/ folder created

**Exercise 284: Jenkins Coverage Report**  
**Goal:** Show coverage in Jenkins  
**Task:** Add to build: `coverage run -m pytest && coverage xml`  
**Concept:** CI coverage reporting  
**Expected:** Coverage tracked in Jenkins

**Exercise 285: Static Code Analysis** 💡  
**Goal:** Understand code quality  
**Task:** Read: Static analysis checks code without running it (style, bugs, security)  
**Concept:** Code quality tools  
**No Action:** Just understanding

**Exercise 286: Install pylint**  
**Goal:** Get Python linter  
**Task:** Type `pip install pylint`  
**Concept:** Linting tools  
**Expected:** pylint installed

**Exercise 287: Run pylint** ⭐  
**Goal:** Check code quality  
**Task:** Type `pylint yourfile.py`  
**Concept:** Code linting  
**Expected:** Shows code quality score

**Exercise 288: Jenkins Linting**  
**Goal:** Automate code checks  
**Task:** Add to Jenkins: `pylint *.py || true` (|| true prevents failure)  
**Concept:** Automated quality checks  
**Expected:** Linting runs in Jenkins

**Exercise 289: Create .pylintrc**  
**Goal:** Configure linter  
**Task:** Type `pylint --generate-rcfile > .pylintrc`  
**Concept:** Tool configuration  
**Expected:** Config file created

**Exercise 290: Customize Linting Rules**  
**Goal:** Adjust rules  
**Task:** Edit .pylintrc, disable some warnings  
**Concept:** Quality standards  
**Expected:** Custom rules applied

**Exercise 291: Install pre-commit** ⭐💡  
**Goal:** Git hooks automation  
**Task:** Type `pip install pre-commit`  
**Concept:** Git hooks  
**Expected:** pre-commit installed

**Exercise 292: Create .pre-commit-config.yaml**  
**Goal:** Define pre-commit hooks  
**Task:** Create file with hooks (trailing whitespace, etc.)  
**Concept:** Automated checks  
**Expected:** Config file created

**Exercise 293: Install Git Hooks**  
**Goal:** Enable pre-commit  
**Task:** Type `pre-commit install`  
**Concept:** Hook installation  
**Expected:** Hooks installed in .git/

**Exercise 294: Test Pre-commit Hooks** ⭐  
**Goal:** Verify hooks work  
**Task:** Try to commit bad code (trailing spaces)  
**Concept:** Pre-commit validation  
**Expected:** Commit blocked, issues shown

**Exercise 295: Artifact Archiving** ⭐  
**Goal:** Save build outputs  
**Task:** Jenkins → Post-build Actions → Archive artifacts: `target/*.jar`  
**Concept:** Artifact management  
**Expected:** Build artifacts saved

**Exercise 296: Workspace Cleanup**  
**Goal:** Clean between builds  
**Task:** Build Environment → Delete workspace before build  
**Concept:** Build hygiene  
**Expected:** Clean workspace each build

**Exercise 297: Build Timeout**  
**Goal:** Prevent hanging builds  
**Task:** Build Environment → Abort if stuck → Set timeout  
**Concept:** Build constraints  
**Expected:** Build times out if too long

**Exercise 298: Email Notifications** ⭐  
**Goal:** Alert on build status  
**Task:** Post-build → Email notification → Enter recipient  
**Concept:** Build notifications  
**Expected:** Emails sent on failure

**Exercise 299: Jenkins Pipeline Preview** 💡  
**Goal:** Introduction to pipelines  
**Task:** Read: Pipelines define CI/CD as code in a Jenkinsfile  
**Concept:** Pipeline as code  
**No Action:** Just understanding

**Exercise 300: First Jenkinsfile** ⭐🎯  
**Goal:** Create declarative pipeline  
**Task:** Create Jenkinsfile:
```groovy
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
    }
}
```  
**Concept:** Pipeline definition  
**Expected:** Pipeline runs in Jenkins

---

## 🔧 PHASE 6: Configuration Management (Exercises 301-375)

### Week 12: Ansible Basics

**Exercise 301: What is Configuration Management?** ⭐💡  
**Goal:** Understand CM  
**Task:** Read: Configuration Management = automated setup and maintenance of servers  
**Concept:** CM fundamentals  
**No Action:** Just understanding

**Exercise 302: What is Ansible?** 💡  
**Goal:** Learn Ansible  
**Task:** Read: Ansible automates server configuration using simple YAML files  
**Concept:** Ansible overview  
**No Action:** Just understanding

**Exercise 303: Install Ansible** ⭐  
**Goal:** Get Ansible  
**Task:** Type `pip install ansible` (Mac/Linux)  
**Concept:** Tool installation  
**Expected:** `ansible --version` works

**Exercise 304: Create Inventory File**  
**Goal:** Define target hosts  
**Task:** Create `inventory.ini`:
```ini
[local]
localhost ansible_connection=local
```  
**Concept:** Ansible inventory  
**Expected:** Inventory file created

**Exercise 305: Test Ansible Connection** ⭐  
**Goal:** Verify setup  
**Task:** Type `ansible all -i inventory.ini -m ping`  
**Concept:** Ad-hoc commands  
**Expected:** Success response

**Exercise 306: Run Shell Command via Ansible**  
**Goal:** Execute command remotely  
**Task:** Type `ansible all -i inventory.ini -m shell -a "echo Hello"`  
**Concept:** Command module  
**Expected:** "Hello" printed

**Exercise 307: What is a Playbook?** 💡  
**Goal:** Understand playbooks  
**Task:** Read: Playbook = YAML file describing desired server state  
**Concept:** Playbook concept  
**No Action:** Just understanding

**Exercise 308: Create First Playbook** ⭐  
**Goal:** Write automation  
**Task:** Create `playbook.yml`:
```yaml
---
- hosts: local
  tasks:
    - name: Print message
      debug:
        msg: "Hello from Ansible!"
```  
**Concept:** Playbook creation  
**Expected:** Playbook file created

**Exercise 309: Run Playbook** ⭐  
**Goal:** Execute playbook  
**Task:** Type `ansible-playbook -i inventory.ini playbook.yml`  
**Concept:** Playbook execution  
**Expected:** Message printed

**Exercise 310: Install Package with Ansible**  
**Goal:** Use package module  
**Task:** Add task:
```yaml
- name: Install curl
  apt:
    name: curl
    state: present
  become: yes
```  
**Concept:** Package management  
**Expected:** curl installed

**Exercise 311: Understand become** 💡  
**Goal:** Learn privilege escalation  
**Task:** Read: `become: yes` = run with sudo  
**Concept:** Privilege escalation  
**No Action:** Just understanding

**Exercise 312: Create File with Ansible** ⭐  
**Goal:** File module  
**Task:** Add task:
```yaml
- name: Create file
  file:
    path: /tmp/ansible-test.txt
    state: touch
```  
**Concept:** File manipulation  
**Expected:** File created

**Exercise 313: Copy File with Ansible**  
**Goal:** Copy module  
**Task:** Add task:
```yaml
- name: Copy file
  copy:
    src: local-file.txt
    dest: /tmp/remote-file.txt
```  
**Concept:** File transfer  
**Expected:** File copied

**Exercise 314: Template Files** ⭐  
**Goal:** Dynamic file generation  
**Task:** Create Jinja2 template, use template module  
**Concept:** Templates  
**Expected:** File generated from template

**Exercise 315: Use Variables in Playbook** ⭐  
**Goal:** Parameterize playbooks  
**Task:** Add:
```yaml
vars:
  my_var: "Hello"
tasks:
  - debug:
      msg: "{{ my_var }}"
```  
**Concept:** Variables  
**Expected:** Variable value printed

**Exercise 316: Register Task Output**  
**Goal:** Capture command output  
**Task:** Add:
```yaml
- name: Run command
  shell: echo "test"
  register: result
- debug:
    var: result.stdout
```  
**Concept:** Output registration  
**Expected:** Command output displayed

**Exercise 317: Conditional Tasks** ⭐  
**Goal:** Run tasks conditionally  
**Task:** Add:
```yaml
- name: Only on Ubuntu
  debug:
    msg: "This is Ubuntu"
  when: ansible_distribution == "Ubuntu"
```  
**Concept:** Conditionals  
**Expected:** Task runs only on Ubuntu

**Exercise 318: Loops in Ansible** ⭐  
**Goal:** Iterate over items  
**Task:** Add:
```yaml
- name: Install packages
  apt:
    name: "{{ item }}"
    state: present
  loop:
    - git
    - curl
    - vim
```  
**Concept:** Loops  
**Expected:** Multiple packages installed

**Exercise 319: Handlers** ⭐💡  
**Goal:** Triggered tasks  
**Task:** Add:
```yaml
tasks:
  - name: Copy config
    copy:
      src: nginx.conf
      dest: /etc/nginx/nginx.conf
    notify: restart nginx
handlers:
  - name: restart nginx
    service:
      name: nginx
      state: restarted
```  
**Concept:** Handlers  
**Expected:** Service restarts only if config changes

**Exercise 320: Service Management**  
**Goal:** Control services  
**Task:** Add task:
```yaml
- name: Ensure nginx running
  service:
    name: nginx
    state: started
    enabled: yes
```  
**Concept:** Service module  
**Expected:** Service started and enabled

**Exercise 321: Check Mode (Dry Run)** ⭐  
**Goal:** Test without changes  
**Task:** Type `ansible-playbook playbook.yml --check`  
**Concept:** Dry run mode  
**Expected:** Shows what would change

**Exercise 322: Verbose Output**  
**Goal:** Debug playbook  
**Task:** Type `ansible-playbook playbook.yml -v` (or -vv, -vvv)  
**Concept:** Verbosity levels  
**Expected:** More detailed output

**Exercise 323: Tags in Playbooks** ⭐  
**Goal:** Selective execution  
**Task:** Add tags to tasks:
```yaml
- name: Task 1
  debug:
    msg: "One"
  tags: group1
```
Run: `ansible-playbook playbook.yml --tags group1`  
**Concept:** Task tagging  
**Expected:** Only tagged tasks run

**Exercise 324: Include Variables File**  
**Goal:** External variables  
**Task:** Create `vars.yml`, include with:
```yaml
vars_files:
  - vars.yml
```  
**Concept:** Variable files  
**Expected:** Variables loaded

**Exercise 325: Ansible Vault** ⭐💡  
**Goal:** Encrypt sensitive data  
**Task:** Type `ansible-vault create secret.yml`  
**Concept:** Secret management  
**Expected:** Encrypted file created

---

### Week 13: Infrastructure as Code

**Exercise 326: What is IaC?** ⭐💡  
**Goal:** Understand IaC  
**Task:** Read: Infrastructure as Code = define infrastructure in files (version controlled, repeatable)  
**Concept:** IaC fundamentals  
**No Action:** Just understanding

**Exercise 327: Ansible Roles** ⭐💡  
**Goal:** Organize playbooks  
**Task:** Read: Roles group related tasks, variables, handlers into reusable units  
**Concept:** Ansible roles  
**No Action:** Just understanding

**Exercise 328: Create Role Structure**  
**Goal:** Initialize role  
**Task:** Type `ansible-galaxy init my-role`  
**Concept:** Role creation  
**Expected:** Role directory structure created

**Exercise 329: Explore Role Directories**  
**Goal:** Understand role layout  
**Task:** View tasks/, handlers/, templates/, defaults/, vars/  
**Concept:** Role organization  
**Expected:** See role structure

**Exercise 330: Use Role in Playbook** ⭐  
**Goal:** Apply role  
**Task:** In playbook:
```yaml
roles:
  - my-role
```  
**Concept:** Role usage  
**Expected:** Role tasks executed

**Exercise 331: Install Role from Galaxy**  
**Goal:** Use community roles  
**Task:** Type `ansible-galaxy install geerlingguy.nginx`  
**Concept:** Ansible Galaxy  
**Expected:** Role downloaded

**Exercise 332: Create requirements.yml**  
**Goal:** Define role dependencies  
**Task:** Create file:
```yaml
roles:
  - name: geerlingguy.nginx
    version: 3.1.0
```  
**Concept:** Dependency management  
**Expected:** Requirements file created

**Exercise 333: Install from requirements**  
**Goal:** Batch install roles  
**Task:** Type `ansible-galaxy install -r requirements.yml`  
**Concept:** Bulk installation  
**Expected:** All roles installed

**Exercise 334: Idempotency Concept** ⭐💡  
**Goal:** Understand idempotency  
**Task:** Read: Idempotent = running multiple times produces same result, no duplicate changes  
**Concept:** Idempotency  
**No Action:** Just understanding

**Exercise 335: Test Idempotency**  
**Goal:** Verify idempotent playbook  
**Task:** Run playbook twice, second run shows no changes  
**Concept:** Idempotent automation  
**Expected:** Second run: "changed=0"

**Exercise 336: Setup Module** ⭐  
**Goal:** Gather system facts  
**Task:** Type `ansible all -i inventory.ini -m setup`  
**Concept:** Facts gathering  
**Expected:** Shows system information

**Exercise 337: Use Facts in Playbook**  
**Goal:** Reference system info  
**Task:** Use `{{ ansible_distribution }}` in task  
**Concept:** Facts usage  
**Expected:** Distribution-specific logic

**Exercise 338: Disable Facts Gathering**  
**Goal:** Speed up playbooks  
**Task:** Add `gather_facts: no` to playbook  
**Concept:** Performance optimization  
**Expected:** Faster playbook execution

**Exercise 339: Group Variables**  
**Goal:** Per-group configuration  
**Task:** Create `group_vars/webservers.yml`  
**Concept:** Group variables  
**Expected:** Variables apply to group

**Exercise 340: Host Variables**  
**Goal:** Per-host configuration  
**Task:** Create `host_vars/hostname.yml`  
**Concept:** Host variables  
**Expected:** Variables apply to host

**Exercise 341: Ansible Configuration File** ⭐  
**Goal:** Customize Ansible behavior  
**Task:** Create `ansible.cfg`:
```ini
[defaults]
inventory = ./inventory.ini
host_key_checking = False
```  
**Concept:** Ansible configuration  
**Expected:** Config applied

**Exercise 342: Dynamic Inventory** 💡  
**Goal:** Programmatic inventory  
**Task:** Read: Dynamic inventory scripts generate host lists programmatically  
**Concept:** Dynamic inventory  
**No Action:** Just understanding

**Exercise 343: Test Strategy**  
**Goal:** Control execution order  
**Task:** Add to playbook: `strategy: free`  
**Concept:** Execution strategies  
**Expected:** Tasks run as fast as possible

**Exercise 344: Serial Execution** ⭐  
**Goal:** Control parallelism  
**Task:** Add: `serial: 2` (runs on 2 hosts at a time)  
**Concept:** Rolling deployments  
**Expected:** Limited parallelism

**Exercise 345: Max Fail Percentage**  
**Goal:** Abort on failures  
**Task:** Add: `max_fail_percentage: 20`  
**Concept:** Failure handling  
**Expected:** Stops if >20% hosts fail

**Exercise 346: Install Vagrant** ⭐  
**Goal:** VM management tool  
**Task:** Download and install Vagrant from vagrantup.com  
**Concept:** Development environments  
**Expected:** `vagrant --version` works

**Exercise 347: Create Vagrantfile**  
**Goal:** Define VM  
**Task:** Type `vagrant init ubuntu/focal64`  
**Concept:** VM definition  
**Expected:** Vagrantfile created

**Exercise 348: Start Vagrant VM** ⭐  
**Goal:** Launch VM  
**Task:** Type `vagrant up`  
**Concept:** VM provisioning  
**Expected:** VM running

**Exercise 349: SSH to Vagrant VM**  
**Goal:** Access VM  
**Task:** Type `vagrant ssh`  
**Concept:** VM access  
**Expected:** Inside VM

**Exercise 350: Provision with Ansible** ⭐🎯  
**Goal:** Automate VM setup  
**Task:** Add to Vagrantfile:
```ruby
config.vm.provision "ansible" do |ansible|
  ansible.playbook = "playbook.yml"
end
```  
**Concept:** Provisioning integration  
**Expected:** Ansible runs during vagrant up

---

### Week 14: Monitoring & Logging

**Exercise 351: What is Monitoring?** ⭐💡  
**Goal:** Understand monitoring  
**Task:** Read: Monitoring = tracking system health, performance, and availability  
**Concept:** Monitoring fundamentals  
**No Action:** Just understanding

**Exercise 352: Install Prometheus** ⭐  
**Goal:** Get monitoring system  
**Task:** Download Prometheus from prometheus.io  
**Concept:** Monitoring installation  
**Expected:** Prometheus binary downloaded

**Exercise 353: Create Prometheus Config**  
**Goal:** Configure Prometheus  
**Task:** Create `prometheus.yml`:
```yaml
global:
  scrape_interval: 15s
scrape_configs:
  - job_name: 'prometheus'
    static_configs:
      - targets: ['localhost:9090']
```  
**Concept:** Monitoring configuration  
**Expected:** Config file created

**Exercise 354: Start Prometheus** ⭐  
**Goal:** Launch monitoring  
**Task:** Type `./prometheus --config.file=prometheus.yml`  
**Concept:** Service startup  
**Expected:** Prometheus running on :9090

**Exercise 355: Access Prometheus UI**  
**Goal:** View metrics  
**Task:** Open browser to `http://localhost:9090`  
**Concept:** Monitoring UI  
**Expected:** Prometheus dashboard

**Exercise 356: Run PromQL Query**  
**Goal:** Query metrics  
**Task:** In Prometheus UI, query: `up`  
**Concept:** Query language  
**Expected:** Shows target status

**Exercise 357: Install Node Exporter** ⭐  
**Goal:** Collect system metrics  
**Task:** Download and run node_exporter  
**Concept:** Metric exporters  
**Expected:** Metrics on :9100/metrics

**Exercise 358: Add Node Exporter to Prometheus**  
**Goal:** Scrape system metrics  
**Task:** Add to scrape_configs:
```yaml
- job_name: 'node'
  static_configs:
    - targets: ['localhost:9100']
```  
**Concept:** Target configuration  
**Expected:** Node metrics in Prometheus
be continued ...
