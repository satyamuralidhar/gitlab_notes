## **Package and Container Registry**
1. Package Registry
2. Container Registry
3. Infrastructure Registry

**Container Registry:**
* will store the docker images into gitlab conatiner registry.
* for login into gitlab registry create a **Personal Access Token(PAT)** give **read/write** permission to **registry** and login with username passord is Access token

        $ docker tag alphine registry.gitlab.com/user/gitlab-container-registry-demo/alphinegl.test

        $ docker login registry.gitlab.com -u username -p <pat token>

        $ docker push registry.gitlab.com/user/gitlab-container-registry-demo/alphinegl.test
        
**CleanUp Images:**
* to save the memory we can use cleanup images enable which are present in setting of the project . we can also set the retention how many days will store images which tags needs to remove.remove tags older than 90days.