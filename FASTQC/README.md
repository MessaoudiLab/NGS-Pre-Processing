# FastQC Files
- After sequences are downloaded, generate fastqc files using fastqc_dir.sh script found in    /bigdata/messaoudilab/arivera/Scripts/fastqc/fastqc_dir.sh
- Run the script 
```
sh “absolute path for fastqc_dir.sh” /”absolute pathway  for the ‘sequences’ directory” /”absolute pathway for the output directory”
```

Example: sh /bigdata/messaoudilab/abotr002/Scripts/fastqc_dir.sh /bigdata/messaoudilab/abotr002/data/sequences/ /bigdata/messaoudilab/abotr002/data/sequences/

- Analyze generated fastQC; check total sequences, sequence length (101 or 75 for NextSeq), %GC (low 40s)
- Check quality control (Phred score: 30 or higher)
