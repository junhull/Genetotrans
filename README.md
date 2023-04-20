# Genetotrans
## 目的
该脚本致力于实现单碱基的基因组坐标到转录本坐标的转换

## Input
```
usage: Genetotrans.py [-h] -g GENEPRED -b BED -d INDEX -o OUTPUT

This script aim to transform a single genome position to the transcript position

optional arguments:
  -h, --help            show this help message and exit
  -g GENEPRED, --genepred GENEPRED
                        The genepred format file which cat transform from the gtf file
  -b BED, --bed BED     The bed format file for a single position of the genome ,such as SNP,and must have six columns
  -d INDEX, --index INDEX
                        The transcript fasta index file which you can generate with the samtools
  -o OUTPUT, --output OUTPUT
                        The output filename
```
## output
![image](https://user-images.githubusercontent.com/89201740/233291999-eb4e52a3-d197-4174-9b0a-0fc82f977f42.png)
最终输出的文件总共有三列，第一列为转录本fasta文件中的名字，第二列为1 base 的转录本坐标，第三列为转录本id，之所以设置成这个样子是为了方便和一些比对到转录本中的数据进行比较
