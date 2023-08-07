**devops_assignment1_part1**


**Step 1**
Done in code

**Step 2**
Dependencies in requirements.txt file

**Step 3**
Docker file created and is present in the repo

**Step 4**
Command: docker build -t greeting-app .
Output: [+] Building 204.3s (9/9) FINISHED
 => [internal] load build definition from Dockerfile                                                               0.1s
 => => transferring dockerfile: 239B                                                                               0.0s
 => [internal] load .dockerignore                                                                                  0.1s
 => => transferring context: 2B                                                                                    0.0s
 => [internal] load metadata for docker.io/library/python:latest                                                   4.5s
 => [internal] load build context                                                                                  0.4s
 => => transferring context: 40.31kB                                                                               0.3s
 => [1/4] FROM docker.io/library/python:latest@sha256:9a1b705aecedc76e8bf87dfca091d7093df3f2dd4765af6c250134ce4  188.0s
 => => resolve docker.io/library/python:latest@sha256:9a1b705aecedc76e8bf87dfca091d7093df3f2dd4765af6c250134ce429  0.0s
 => => sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c 49.56MB / 49.56MB                  40.6s
 => => sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f 24.03MB / 24.03MB                  40.8s
 => => sha256:0ad2659187130a5b7a8094996b4f240078b97be75a5395fa9869ca0a178fa676 2.01kB / 2.01kB                     0.0s
 => => sha256:608c79ebc6d50c0de774945744542f1ac114478446b0b35ad4a15c3198743113 7.53kB / 7.53kB                     0.0s
 => => sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603 64.11MB / 64.11MB                 124.0s
 => => sha256:9a1b705aecedc76e8bf87dfca091d7093df3f2dd4765af6c250134ce4298a584 2.14kB / 2.14kB                     0.0s
 => => sha256:4d207285f6d296b9806bd00340437406c25207412c52fcfcbf229a5ecff7bf94 211.03MB / 211.03MB               178.2s
 => => extracting sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c                          1.9s
 => => sha256:9402da1694b8dae94a0cb89a2719ce24a909e809b22c31d39edee8e18b3d300b 6.39MB / 6.39MB                    46.3s
 => => extracting sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f                          0.7s
 => => sha256:9bdbf45d01af5880bbab0120b825cc0f237835fd253f54a79b396519ea250daf 19.76MB / 19.76MB                  60.6s
 => => sha256:dd8b7ef87a9d8f73f1da40f467d7878182e591a6ab390005d401c4e59928c8e2 244B / 244B                        61.7s
 => => sha256:4de52e7027c53cdd2ad280aed34a7fb1b8ccb8143bd1ed4678f25a4d7020b5fa 3.09MB / 3.09MB                    64.4s
 => => extracting sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603                          2.6s
 => => extracting sha256:4d207285f6d296b9806bd00340437406c25207412c52fcfcbf229a5ecff7bf94                          7.6s
 => => extracting sha256:9402da1694b8dae94a0cb89a2719ce24a909e809b22c31d39edee8e18b3d300b                          0.3s
 => => extracting sha256:9bdbf45d01af5880bbab0120b825cc0f237835fd253f54a79b396519ea250daf                          0.7s
 => => extracting sha256:dd8b7ef87a9d8f73f1da40f467d7878182e591a6ab390005d401c4e59928c8e2                          0.0s
 => => extracting sha256:4de52e7027c53cdd2ad280aed34a7fb1b8ccb8143bd1ed4678f25a4d7020b5fa                          0.3s
 => [2/4] ADD . /devops_assignment1_part1                                                                          0.4s
 => [3/4] WORKDIR /devops_assignment1_part1                                                                        0.1s
 => [4/4] RUN pip install -r requirements.txt                                                                     10.8s
 => exporting to image                                                                                             0.4s
 => => exporting layers                                                                                            0.4s
 => => writing image sha256:7fa46e551755f98018092650e9c6c061cffb3846ddf1949813e9480415729aff                       0.0s
 => => naming to docker.io/library/greeting-app                                                                    0.0s



**Step 5**
Command: docker tag greeting-app abdul7235/greeting-app  (for tagging the image)


Command: docker login -u abdul7235
Output: Password:
Login Succeeded

Logging in with your password grants your terminal complete access to your account.
For better security, log in with a limited-privilege personal access token. Learn more at https://docs.docker.com/go/access-tokens/


Command: docker push abdul7235/greeting-app

Output: Sharing the following output since terminal closed after running above command, could not copy logs

Using default tag: latest
The push refers to repository [docker.io/abdul7235/greeting-app]
275b58222ead: Layer already exists
5f70bf18a086: Layer already exists
23c2b1fe1c61: Layer already exists
48091d4730a8: Layer already exists
8729b6a044ba: Layer already exists
5c0fbc8e3c3d: Layer already exists
c5f1d4dd95f0: Layer already exists
6a25221bdf24: Layer already exists
b578f477cd5d: Layer already exists
b298f9991a11: Layer already exists
c94dc8fa3d89: Layer already exists
latest: digest: sha256:fec35d5a8c459753458e4dde256ec34916db42c0c3734dd3888260ba6bca691a size: 2634


**Step 6**
Created remote repository on GitHub.
https://github.com/abdul7235/devops_assignment1_part1

**Step 7**
Created a README.md file on local repo and pushed it on remote

**Step 8**
Command: git init
Output: Initialized empty Git repository in D:/DevOps/devops_assignment1_part1/.git/

Command: git status
Output: git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        Dockerfile
        README.md
        app.py
        models/
        requirements.txt

nothing added to commit but untracked files present (use "git add" to track)

Command: git branch -M main
Command: git status
Output: On branch main

Command: git remote add origin https://github.com/abdul7235/devops_assignment1_part1.git
Command: git remote show origin
Output: * remote origin
  Fetch URL: https://github.com/abdul7235/devops_assignment1_part1.git
  Push  URL: https://github.com/abdul7235/devops_assignment1_part1.git
  HEAD branch: (unknown)

Command: git add .
Command: git status
Output: On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   .gitignore
        new file:   Dockerfile
        new file:   README.md
        new file:   app.py
        new file:   models/person_model.py
        new file:   requirements.txt


Command: git commit -m "Initial Commit"
Command: git status
Output: On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")


