# Trimming
Once you have checked for quality control, you must trim sequences if certain regions vary greatly from data in order to not distort sequence assembly. Trimming is done through Trim Galore which will quality filter and trim the reads. You must use a script and signify the phred score and number of base pairs wanted at the end of the command line.

- In data directory, make new directory: 
```
mkdir trim_sequences
```
- move sequence files (.gz)  from “sequences” to “trim_sequences” directory 
```
mv *.gz ../trim_sequences
```
- Check trim_galore_directory.sh script to make sure it’s linked to the correct script (trim_galore.sh) before loading the following. 
```
sh /”absolute pathway for trim_galore_directory.sh” /”absolutepathwayfor‘sequences’directory 30 75”
```
If trimming NextSeq data, Run: 
```
sh /”absolute pathway for trim_galore_directory.sh” /”absolutepathwayfor‘sequences’directory 30 50”
```
- Check if trimming is done
```
qstat | grep “username” (if done, nothing will show)
```
- When trimming is complete, check FastQC reports.
