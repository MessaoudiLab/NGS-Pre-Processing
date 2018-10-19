# Downloading Data to Terminal
Libraries are sequenced through the website http://illumina.bioinfo.ucr.edu/ht/

- Once in the parent directory, change directories to the sub-directory “data” 
```
cd data
```
- In the data directory create a download script
```
nano “projectname”_download.sh
```
- Use the wget command to link sequence addresses from the illumina.bioinfo website to the terminal

Example:
wget http://illumina.bioinfo.ucr.edu/illumina_runs/358/flowcell34_lane99_pair1_CGATGT.fastq.gz

- Run the download script
```
sh“projectname”_download.sh
```
