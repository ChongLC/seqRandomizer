# seqRandomizer: A tool to generate random viral protein sequence datasets
[![Run in Google Colab](https://img.shields.io/badge/Colab-Run_in_Google_Colab-blue?logo=Google&logoColor=FDBA18)](https://colab.research.google.com/drive/1IwNPKaRKGgPzqiOBuEo8S0VbUpe3XqVh?usp=sharing) <br>

A random protein sequence dataset can be useful for various sequence analysis, in particular to evaluate and correct the analysis for background noise. Herein, we offer a tool that can generate a dataset of random viral protein sequences. 

---

### Usage
`python seqRandomizer.py [-h] [-o OUTPUT] [-l SEQLEN] [-n SEQNUM]`

In the usage case below, the `seqRandomizer` tool is applied to generate a random viral protein sequence dataset in the folder `result`, named `random_vprot.fasta` consisting of 1,000 sequences of length 1,000 amino acids. The amino acid composition of the random sequences is based on all reported viral sequence retrieved from the NCBI Protein database (as of May 2021; `allVirus080521.fasta`). <br> 

```
python seqRandomizer.py -o random_vprot.fasta -l 1000 -n 1000
```

#### Command-line Arguments
| Argument | Parameter | Type    	| Required | Description                                             |           
|:--------:|-----------|---------	|:--------:|-------------------------------------------------------  |
| -h       | help      | N/A     	|FALSE	   | Show this help message and exit                         |
| -o       | output    | String  	|TRUE      | Path of the output file to be created                   |
| -l       | seqlen    | Integer 	|TRUE      | The length of random protein sequences to be generated  |
| -n       | seqnum    | Integer 	|TRUE      | The number of random protein sequences to be generated  |

---

### Important Note for Users
* This seqRandomizer is specific to the [protocol describing the step-by-step utility of UNIQmin](https://www.biorxiv.org/content/10.1101/2022.08.09.503271v2.full).

---

### Found a bug?
Or would like a feature added? Or maybe drop some feedback? Just open a new issue or send an email to us (lichuinchong@gmail.com).
