# combineSNPfiles
A perl script to merge multiple files created by POPBAM SNP into a single file.



Input
=====
text file with list of files to be combined, one file per line


Formatting
==========

The snp files must be compressed with bgzip and indexed with tabix:

```bgzip -c myfile.snp > myfile.snp.bgz```

```tabix -b 2 -e 2 -s 1 myfile.snp.bgz```


Output
======
single snp file printed to STDOUT
