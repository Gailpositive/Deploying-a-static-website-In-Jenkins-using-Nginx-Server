## Jenkins Tasks

* Create an EC2 instance and install jenkins
* Connect the jenkins server to a static site available on github
* Create 3 branches and parameterize jenkins
* 
# Step 1

* Spine up an EC2 Aws instance
* On my terminal create a file with the "touch" command
* sudo vi into the file
* paste the Jenkins installation script
* Jenkins is actively enabled
<img width="845" alt="jenkins installation script" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/2b152c0c-407d-4ec6-a606-1263e7c8b1ed">

* TCP/Port 8080 inbound rules open to anywhere
<img width="740" alt="jenkins listens on port 8080" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/c0aa2a4e-5ce6-428e-a7e0-845c86c33a9c">

* Paste the IP:8080 on my browser to access Jenkins page
* As an admin, Copy the Jenkins password from the Jenkins installations to unlock Jenkins
<img width="801" alt="add password" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/53f0d6e0-cbd9-4363-ba54-4d9b260a3449">


# Step 2: connecting Jenkins To Github config.
* On my Jenkins dashboard
* Click on new item to create a job
* Give the job a description
* Tick Github project and fill in the created github repo url
<img width="847" alt="jenkins to github 2" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/9e2dcef6-ed28-453b-b5f7-6a56db296a39">

* On source code management
* Tick Git
* On Repository url, type in the github HTTP url
<img width="960" alt="jenkins to github 3" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/b11b75e8-116d-4232-adf2-a1a1be9282a4">

* Scroll down to Branches to build,
* On build specifier, specify */main, which is the github main branch
* Apply and save
<img width="872" alt="jenkins to github 4" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/b3442dab-27d7-4559-9af1-c98cc06940c1">

* Click on Build Now
* Notice Github Logo installed  on the left side navigation plane
<img width="634" alt="see git hub logo has added on the navigation plane on the left 5" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/88046bc6-39ea-41d4-98a7-fae9550b96a5">

