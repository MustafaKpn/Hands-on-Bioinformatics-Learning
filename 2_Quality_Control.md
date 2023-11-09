## Quality Control of Reads
#### FastQC Installation
1. Install software
```
$ wget http://www.bioinformatics.babraham.ac.uk/projects/fastqc/fastqc_v0.11.4.zip
```
2. Unzip file:
```
$ unzip fastqc_v0.11.4.zip
```
3. Navigate to FastQc folder
```
$ cd FastQC/
```
4. Change permissions
```
$ chmod fastqc
```
5. Finally, it can be ran using the command:
```
$ ./fastqc
```
#### Notes on the result of FastQC
* The FastQC program is capable of detecting problems regarding base and sequence quality, base content, Kmer frequency, GC content, sequence length and duplication and contaminant/adapter. Undeniably, all of these problems will affect the quality of assembly of mapping, but the two main problems are the base quality and adapter.
* Usually, the quality of the bases deteriorates towards the end of the read, with the forward read showing better quality than the reverse read.
* A good dataset will have a single peak located around score 30. Warning is given when the mean quality is <27, failure at <20.
* Most of the time, overrepresented sequences are either primers or adapters.

#### Fastx-toolkit & FASTQ Processing Utilities
Upon quality check of your dataset, the next step would be to get the data ready for further mapping work. Fastx-toolkit2 is a collection tools for FASTQ files preprocessing.
##### installation:
