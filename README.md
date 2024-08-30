# Genome-Assembly
This workflow is prepared for the assemble of PacBio HiFi long read sequences. The annotation and downstream analysis is also included.
-
Nie Jilu from lab. plant breeding, Kyoto University

2024/08/30
The step6.3 and Step7 is not well-done. I will continously update them
The Analysis_files are not done yet
The code has not been tested and integrated by 2024/08/30, the code after test will be in a file named **makefile.sh **


All details could be seen in the files of each step


A overview of the workflow of PacBio hifi long read assembly is as following:
![微信图片_20240830131136](https://github.com/user-attachments/assets/a7731e45-9c86-42f3-b1d1-05d45051ba8c)

For achieving your purposes, a conda environment is requied.

**To check details, please go to the files whose name are from step1 to step3**

After assemble, you may need evaluation of your genome, please check step 4 for details
Generally speaking, BUSCO is the software to do it

The annotation is a little bit complex, including gene prediction by augustus and other software, a mechine learning program 
would be needed if there is no training data for your speices.

The annotation usually begin from the masking of TE and repeat, which will help you to save a lot of computating time
Then you may need homolog genomes and RNA-seq data to help with your annotating.

An overview could be seen as following:
![Analysis](https://github.com/user-attachments/assets/9b599a27-a277-4831-b135-0d061342c1dc)
Check the details in the file after step 4.

Pan-genome analysis and downstream analysis is under releasing
