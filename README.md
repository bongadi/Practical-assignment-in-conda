# Practical-assignment-in-conda

**Practical Assignment in preparation for next class**

1.	Run wsl to access a **new terminal**.
    By default, when you install Conda, a base environment is created and often activated unless you deactivate it or switch to another Conda environment. Therefore, you are     likely to see that that the base Conda environment is currently active e.g.  (base) 

2.	Identify the **path to the directory** you are currently in by using the command:  

  	       pwd
      You should be able see the path e.g.    /home/bongadi

4.	Verify your **Conda installation** by running the command:     

  	      Conda --version 
	 You should see the installed version of Conda e.g. conda 24.7.1
 
6.	Create a **new environment** in conda: called **sra**.

  	     conda create -n sra
8.	**Activate** the sra environment.
               
          conda activate sra

9.	**Install the sra-tools** package from the bioconda channel using Conda

         conda install –c bioconda sra-tools

10.	Download sequencing data from the **NCBI Sequence Read Archive (SRA)**, via the terminal (Use the accession number you identified in the previous assignment e.g. 
    ERR1149319)

  	      prefetch ERR1149319

11.	List (ls) to check if your file is **downloaded successfully **(This requires very stable network and will take time depending on the size)

12.	Convert the. sra file to a more usable format in our case let’s use **FASTQ**.


   	    fastq-dump --split-files ERR1149319

14. **NOTE: Troubleshoot appropriately and document any challenges,**
