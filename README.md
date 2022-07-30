
<p align="center">
  <img src="https://github.com/mahdieh1/KARAJ/blob/main/docs/karaj.jpg" />
</p>

=============================================================================================================================================================

## A command-line software to streamline acquiring biological data

We here developed KARAJ a fast and flexible command-line software for Linux that automate querying and streamline downloading of a wide range of file formats containing biological data. KARAJ has five main advantages over other similar tools; firstly, it gives a summary list of accessible datasets generated by or used in scientific articles and enables users to select whichever ones are willing to download; secondly, KARAJ calculates the size of files users willing to download and checks with the local driver to ensure the availability of adequate space in the local disk; thirdly, KARAJ generates the metadata table containing sample information and experimental design of the corresponding study; fourthly, this user-friendly pipeline automatically checks and installs all of the requirements, and lastly, it enables users to download supplementary data tables  attached to publications. We described the options of KARAJ and evaluated its performance by analyzing the data sets from three research papers. KARAJ and the instructions for local installation are publicly available at https://rdrr.io/github/mahdieh1/XXX.

<p align="center">
  <img src="https://github.com/mahdieh1/KARAJ/blob/main/docs/WhatsApp%20Image%202022-07-30%20at%209.16.35%20PM.jpeg" />
</p>
--------------------------------------------------------------------------------------------------------------------------------------------

## Table of Contents

- [Installation](#installation)
- [Required arguments](#required-arguments)
- [Common Error messages](#common-error-messages)
- [Examples](#examples)
- [How to use](#how-to-use)
- [Reference](#reference)
- [Author Info](#author-info)
- [Acknowledgements](#acknowledgements)
- [License](#license)

------------------------------------------------------------------------------------------------------------------------

## Installation

KARAJ runs on LINUX. Install the package from Github using the following commands.

```
cd /KARAJ
git clone https://github.com/Knowledge-Wisdom-Understanding/Auto-Recon.git
cd Auto-Recon
chmod +x setup.sh
./setup.sh
```
------------------------------------------------------------------------------------------------------------------------

### Required arguments

| Flags | Description | Default | Syntax | 
| :--- | :--- | :--- | :--- |  
| -l | The list of URL(s) | empty | `KARAJ -l [URL1 URL2 URL3 ... URLn ]` 
| -p	| The list of PMCID(s) | empty | `KARAJ -p [PMCID1 PMCID2 PMCID3 ... PMCIDn]`
| -o	| The output working directory | The current working directory | `KARAJ -o [working directory]`
| -t	| Type of files that user needs | KARAJ downloads all of file types | `KARAJ -t [bam/vcf/fastq ]`
| -s	| Specify the Suplemenatry data is necessary to download or not  | 0 | `KARAJ -l [1/0]`
| -f	| Specefiy file containing the URL(s) or PMCID(s) or Seqlist in the working direcory: For downloading: (1) URL(s): please use PMlist for the filename and 1 as the flag value with the file name (PMlist =1) and (Links = 0)   (2) PMCID(s): please use Links for the filename and 0 as the flag value with the file name (PMlist =1) and (Links = 0)   | KARAJ downloads based on the -l, -p or -i flags | `KARAJ -f [1/0]` (3) PMCID(s): please use Links for the filename and 0 as the flag value with the file name (PMlist =1) and (Links = 0)   | KARAJ downloads based on the -l, -p or -i flags | `KARAJ -f [1/2/3]`
| -i	| The accession IDs that user needs| KARAJ downloads all of accession IDs | `KARAJ -i [SRR/SRP/PRJ/PRJNA]`
| -d	| Specefiy KARAJ downloads all files or selected files: (1): downloads the selected files, (0): downloads all files | KARAJ downloads all of files associated to the -l, -p, -f or -i flags| `KARAJ -d [1/0]`
| -m	| Specefiy KARAJ downloads metadata or not | empty | `KARAJ -m [URL(s)]?`
| -h	| Help | empty | `KARAJ -h `
| -u	| The list of PMCID(s) | empty | `KARAJ -l [URL(s)]`
| -c	| The number of threads| (the number of cores accessible in the system -1) | `KARAJ -c [core]`

------------------------------------------------------------------------------------------------------------------------
## Common Error messages

| Error message | Description |
| :--- | :--- | :--- | 

------------------------------------------------------------------------------------------------------------------------
## Examples

```

```
------------------------------------------------------------------------------------------------------------------------
## How to use

Before using KARAJ, you need to run make file with the following commands:

```
./makebash.sh

```

------------------------------------------------------------------------------------------------------------------------

## Reference
```
Please consider citing the follow paper when you use this code.
  Title={KARAJ: a command-line software to streamline acquiring biological data},
  Authors={Mahdieh Labani, Amin Beheshti, Nigel Lovell, Hamid Alinejad-Rokny, Ali Afrasiabi}
}
```
------------------------------------------------------------------------------------------------------------------------

## Contacts

I will be pleased to address any question or concern about the KARAJ package:
In case of queries, please email: m.labani@unsw.edu.au or a.afrasiabi@unsw.edu.au


------------------------------------------------------------------------------------------------------------------------

## Author Info
### People who contributed to the KARAJ idea and code:
* Mahdieh Labani 
* Ali Afrasiabi
* Amin Beheshti
* Hamid Alinejad-Rokny
* Nigel Lovell

------------------------------------------------------------------------------------------------------------------------

## Acknowledgements
This work was funded by the UNSW Scientia Program Fellowship and the Australian Research Council Discovery Early Career Researcher Award (DECRA), Macquarie PhD Scholarship and Australian Government Research Training Program (RTP) scholarship. Analyses were made possible with High Performance Computing resources provided by the BioMedical Machine Learning Lab with funding from the Australian Government and the UNSW SYDNEY.

------------------------------------------------------------------------------------------------------------------------

## License

This package is free software; you can redistribute it and/or modify it under the terms of the , MIT License as published by the Free Software Foundation.


