### How to install and use

1. install `conda`
2. `conda env create -f env.yml`
3. `conda activate QSBSA`
4. Should be able to go and run, but there are the following warnings need to be handeled


⚠️ Warning

1. `~/scripts/fetchSeq4fa2.pl` is not included.

2. There are hard coded path that should be changed, such as `home/CAM/`. 


### How to use these scripts?

Step 1: git clone this repository to your directory on server. 

```
cd /path/to/where/you/want/to/keep/the/scripts/
git clone git@github.com:qslin/Bulk-Segregation-Analysis.git
cd Bulk-Segregation-Analysis
```

Step 2: read the instruction

```sh QSBSA.sh```.

Step 3: prepare all necessary files, e.g. genome reference file.

Step 4: create and go to your working directory.

```
cd /path/to/where/you/want/the/result/files/go/
mkdir Mv00123
cd Mv00123
```

Step 5: submit the QSBSA.sh script with options to server. For example:

```
sbatch /path/to/the/Bulk-Segregation-Analysis/scripts/QSBSA.sh -r reference.fa -f reads.txt 
```

Step 6: result files will be generated in your working directory. Check them!

Step 7: delete the tmp directory
