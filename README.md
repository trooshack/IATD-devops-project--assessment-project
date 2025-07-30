This is the Project Submission for IATD - Intro to DevOps Course, TP3 - by Trushik Tekwani.

**Task 5 – RESUBMISSION**

I have made changes to the folder structure such that my build context is now root directory. Both dockerfiles are triggered using the '-f' file name action on the 'docker build' command in MainCI. 
Both the dockerfiles i.e. docker.test and docker.user are re-written to only include folders and files required.
Note that docker.user file does not copy 'tests' folder.
This meets the objective of only copying required files to the docker images. See screenshots below:

Updated folder structure:

<img width="940" height="719" alt="image" src="https://github.com/user-attachments/assets/e5fbc39c-9a0d-4929-a9aa-51680bc8896f" />

docker.test file which only copies required files and folder, excludes files not required

<img width="940" height="491" alt="image" src="https://github.com/user-attachments/assets/fbdada69-a0a2-4976-bda9-fc94b4fbf2ff" />

docker.user file copies required files and also exlcudes 'tests' directory as per instructions. It runs CMD 'start' and not 'test'.

<img width="895" height="533" alt="image" src="https://github.com/user-attachments/assets/d4f7d6cb-630c-4ae3-8bff-3c8239e63f51" />




**Task 1 – Git Best Practices**
There has been an effort to detail what is happening in each commit.
Note, I learnt about the ‘git commit –amend’ command after completion of the project. Hence, could not incorporate it in the project.
 

<img width="963" height="830" alt="image" src="https://github.com/user-attachments/assets/84bfc390-d94d-40bf-83fd-63cb8412efa0" />


**Task 2 – Issue Fixing**
Below are the issues in test files.
i.	Utilities.js

<img width="951" height="626" alt="image" src="https://github.com/user-attachments/assets/a787db6b-685d-4ab3-beb1-fbdc0b0445a7" />


ii.	Index.js
 
<img width="701" height="625" alt="image" src="https://github.com/user-attachments/assets/6232054c-9ead-47bb-ad95-53e020d43b40" />

 <img width="888" height="722" alt="image" src="https://github.com/user-attachments/assets/976ca4b8-3d7e-4898-a0b3-f9d78a6aa26b" />


Pipeline output for Task 2
 
<img width="829" height="477" alt="image" src="https://github.com/user-attachments/assets/725c4f8e-823a-438d-9f93-3f5a36f90fac" />


**Task 3 – Unit Testing**
Unit tests added per the instructions 

 <img width="887" height="854" alt="image" src="https://github.com/user-attachments/assets/17a81986-546f-4026-ac8e-50fb98c84ad5" />

<img width="916" height="688" alt="image" src="https://github.com/user-attachments/assets/9ad4f7ef-6da0-43de-869c-f74669fddcf0" />






**Task 4 – Pipeline Configuration**
YAML file with Docker image build, login to Docker Hub and push the image.
 
 <img width="940" height="541" alt="image" src="https://github.com/user-attachments/assets/513c23e0-0041-45f9-98fb-d1b9eda58f4b" />

<img width="823" height="668" alt="image" src="https://github.com/user-attachments/assets/d67eb027-c275-4de3-b31b-5b5ce7a38ecc" />


	
**Task 5 – Advanced Docker Configuration**
This task requires some folders to be excluded from being copied to the GitHub runner using the Dockerfile. This was achieved by creating  ‘.dockerignore’ folder for each of the images.
As shown below, the ‘test.Dockerfile’ and ‘user.Dockerfile’ are placed in separate folders with their respective ‘.dockerignore’ files. Snapshot of dockerhub is also included at the end.
 

<img width="950" height="892" alt="image" src="https://github.com/user-attachments/assets/7a6b8c65-9e9c-431a-83c4-ce068b2c6e7e" />

<img width="940" height="824" alt="image" src="https://github.com/user-attachments/assets/7705295b-4128-470b-b312-4bd37c318854" />

<img width="940" height="481" alt="image" src="https://github.com/user-attachments/assets/8d78cf5c-9944-4cbf-abba-6706e77a8f0b" />




 

 








