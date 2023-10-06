# Jenkins Tasks

* Create an EC2 instance and install jenkins
* Connect the jenkins server to a static site available on github
* Create 3 branches and parameterize jenkins


## Step 1
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


## Step 2: connecting Jenkins To Github config.

* Open a github repo
* <img width="926" alt="cicd 1" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/c28c55ff-ad7d-42ba-b301-04b8e21ac93e">

*  On my Jenkins dashboard
* Click on new item to create a job
* Give the job a name
* click on freestyle project
* Apply and save
<img width="948" alt="cicd 12 create a Jenkins job" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/f9275bbc-572f-4baa-a3be-7c6638c64318">

* To solve this error,
* Click Dashboard,
* Click manage jenkins
* Scroll to security down to CSRF protection
* Tick Enable proxy capacity
* Apply and save
* Refresh the page
<img width="418" alt="cicd 13 to solve this error, click Dashboard, manage jenkins,security,scroll down CSRF protection,tick Enable proxy capacity,apply and save" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/4f536d74-990c-479b-b07d-fb92226867a1">


* On General
* Tick Github project and fill in the created github repo url
  <img width="931" alt="cicd 16" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/2cc0514f-92d3-4794-ad17-d13d4b283dbb">

* On source code management
* Tick Git
* On Repository url, type in the github HTTP url
<img wid
<img width="934" alt="cicd 17 git https" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/58b503d0-c653-4a7f-a650-0e7605ebbe84">

* Scroll down to Branches to build,
* On build specifier, specify */main, which is the github main branch
* Apply and save
<img width="872" alt="jenkins to github 4" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/b3442dab-27d7-4559-9af1-c98cc06940c1">

* Click on Build Now
* Notice Github Logo installed and visible on the left side navigation plane
<img width="634" alt="see git hub logo has added on the navigation plane on the left 5" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/88046bc6-39ea-41d4-98a7-fae9550b96a5">

## Step 3: Create a static web page

* To navigate to the online vscode on github repo
* click on code
* click on coldspaces
<img width="926" alt="cicd 1" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/17b61831-d976-4d78-a0b2-661a4919f7c7">

* Online Vscode 
<img width="947" alt="cicd 3" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/8ade576f-e7b3-480e-bab1-6b32f4cc6a76">

* I download the zip file with the "wget" command
<img width="937" alt="cicd 4" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/7a9ee737-0a9f-499d-bbb1-6a4528dc7fb9">

* ls the file
<img width="942" alt="cicd 5" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/c5a5c994-0925-47ce-b942-305ec97820f7">

* To unzip the file, I execute the "unzip" command
<img width="956" alt="cicd 6" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/87f8e98a-befd-4970-a3cc-ab93a73a1598">

* I execute the "rm" command  the unzip file
<img width="938" alt="cicd 7" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/5e9bbfbd-b99b-4b74-8bc5-767d30cd3a31">

* ls the file
<img width="939" alt="cicd 9" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/c536c3d5-a669-454a-a606-9ec67eee5e72">

* With the "mv" command, I move the file to a new file name "code"
<img width="945" alt="cicd 10 rename" src="https://github.com/Gailpositive/Jenkins-CICD-pipeline/assets/111061512/e896d0e3-f171-4b90-a478-8091e5734099">

