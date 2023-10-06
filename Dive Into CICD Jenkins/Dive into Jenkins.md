## Jenkins Tasks

* Create an EC2 instance and install jenkins
* Connect the jenkins server to a static site available on github
* Create 3 branches and parameterize jenkins
# Step 1

* Spine up an EC2 Aws instance
* On my terminal create a file with the "touch" command
* sudo vi into the file
* paste the Jenkins installation script
* Jenkins is actively enabled
<img width="845" alt="jenkins installation script" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/2b152c0c-407d-4ec6-a606-1263e7c8b1ed">

* TCP/Port 8080 inbound rules open to anywhere
<img width="740" alt="jenkins listens on port 8080" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/c0aa2a4e-5ce6-428e-a7e0-845c86c33a9c">

*  Paste the IP:8080 on my browser to access Jenkins page
* Copy the Jenkins password from the Jenkins installations to unlock Jenkins
<img width="801" alt="add password" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/53f0d6e0-cbd9-4363-ba54-4d9b260a3449">


# Step 2
* On my Jenkins dashboard
* Click on new item 
* 
<img width="847" alt="jenkins to github 2" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/9e2dcef6-ed28-453b-b5f7-6a56db296a39">

<img width="960" alt="jenkins to github 3" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/b11b75e8-116d-4232-adf2-a1a1be9282a4">

<img width="872" alt="jenkins to github 4" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/b3442dab-27d7-4559-9af1-c98cc06940c1">
