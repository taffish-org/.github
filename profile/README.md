# Welcom to TAFFISH-ORG 👋

TAFFISH(Tools And Flows Framework Intensify SHell) allows you to avoid worrying about software installation, environment conflicts, container management, cluster operations, ...... Build, use, and share your own portable, reproducible scientific workflows just like shell commands.



## ⛓️‍💥 Links
- [taffish-official-website](https://taffish.com)
- [github: taffish-install](https://github.com/taffish-org/taffish-install)
- [github: taffish-hub](https://github.com/taffish-org/taffish-hub)



## 📥 Install

### Container Apps before TAFFISH:
You need to install at least one Container App([Docker](https://www.docker.com/)/[Podman](https://podman.io/)/[Apptainer(Singularity)](https://apptainer.org/index.html)) for taffish. And we suggest:

  - Windows(WSL)/Mac: [Docker](https://www.docker.com/) :: for people who are root users
  - Linux : [Apptainer](https://apptainer.org/index.html)/[Podman](https://podman.io/) :: for people who are not root users (but you may need root to install them to make sure all non-root users can use these container apps)

### ![tiny-Debian-OpenLogo](https://github.com/user-attachments/assets/fc2e8de9-fbfc-4675-8d37-5181474be5b3) Debian12 (Linux)

```bash
sh -c "$(curl -fsSL https://github.com/taffish-org/taffish-install/releases/download/latest/install-taffish-debian12-amd64-beta.sh)" -n
```

### ![tiny-Ubuntu-logo-2022](https://github.com/user-attachments/assets/fcdbcd66-0fe8-42a9-bf44-714c24d0fbdf) Ubuntu (Linux) (>=18.04.1-LTS)

```bash
sh -c "$(curl -fsSL https://github.com/taffish-org/taffish-install/releases/download/latest/install-taffish-ubuntu-amd64-beta.sh)" -n
```

### ![tiny-Apple_logo_white](https://github.com/user-attachments/assets/36d1ec28-1577-4cd0-a10a-cdaf08952771) MacOS (Darwin) (Apple Silicon, arm64)

```bash
sh -c "$(curl -fsSL https://github.com/taffish-org/taffish-install/releases/download/latest/install-taffish-darwin-arm64-beta.sh)" -n
```

### ![tiny-Apple_logo_white](https://github.com/user-attachments/assets/36d1ec28-1577-4cd0-a10a-cdaf08952771) MacOS (Darwin) (Intel Chip, x86_64)

```bash
sh -c "$(curl -fsSL https://github.com/taffish-org/taffish-install/releases/download/latest/install-taffish-darwin-amd64-beta.sh)" -n
```



## Quick Start

```bash
taf update
taf install -y hello
taf-hello --to $USER
```



## 🏠 TAFFISH-HUB (taf-apps) (42)

### ⚙️ BASE (6)
1. [debian :: v12](https://github.com/taffish-org/debian)
2. [python :: v3.13.2](https://github.com/taffish-org/python)
3. [sbcl :: v2.5.2](https://github.com/taffish-org/sbcl)
4. [R :: v4.4.3](https://github.com/taffish-org/R)
5. [intel-oneapi :: v2025.0.2-0-devel-ubuntu24.04](https://github.com/taffish-org/intel-oneapi)
6. [hello :: v1.0.0](https://github.com/taffish-org/hello)

### 🛠️ TOOLs (35)
1. [muscle :: v5.3](https://github.com/taffish-org/muscle)
2. [MCScanX :: v1.0.0](https://github.com/taffish-org/MCScanX)
3. [uniprot-idmapping :: v1.0.0](https://github.com/taffish-org/uniprot-idmapping)
4. [juicer :: v2.20.00](https://github.com/taffish-org/juicer)
5. [blast :: v2.16.0](https://github.com/taffish-org/blast)
6. [cdhit :: v4.8.1](https://github.com/taffish-org/cdhit)
7. [hmmer :: v3.4](https://github.com/taffish-org/hmmer)
8. [get-seqs-from-ids :: v1.0.0](https://github.com/taffish-org/get-seqs-from-ids)
9. [sra-tools :: v3.2.0](https://github.com/taffish-org/sra-tools)
10. [seqtk :: v1.4](https://github.com/taffish-org/seqtk)
11. [fastqc :: v0.11.9](https://github.com/taffish-org/fastqc)
12. [trim_galore :: v0.6.10](https://github.com/taffish-org/trim_galore)
13. [STAR :: v2.7.11b](https://github.com/taffish-org/STAR)
14. [subread :: v2.0.2](https://github.com/taffish-org/subread)
15. [bedtools :: v2.31.1](https://github.com/taffish-org/bedtools)
16. [samtools :: v1.21](https://github.com/taffish-org/samtools)
17. [bcftools :: v1.21](https://github.com/taffish-org/bcftools)
18. [bowtie2 :: v2.5.4](https://github.com/taffish-org/bowtie2)
19. [fastp :: v0.24.0](https://github.com/taffish-org/fastp)
20. [kallisto :: v0.51.1](https://github.com/taffish-org/kallisto)
21. [bustools :: v0.44.1](https://github.com/taffish-org/bustools)
22. [hisat2 :: v2.2.1](https://github.com/taffish-org/hisat2) (amd64 only)
23. [mafft :: v7.525](https://github.com/taffish-org/mafft)
24. [clustal-omega :: v1.2.4](https://github.com/taffish-org/clustal-omega)
25. [bwa :: v0.7.18](https://github.com/taffish-org/bwa)
26. [gatk :: v4.6.1.0](https://github.com/taffish-org/gatk)
27. [salmon :: v1.10.3](https://github.com/taffish-org/salmon)
28. [Trinity :: v2.15.2](https://github.com/taffish-org/Trinity)
29. [freebayes :: v1.3.9](https://github.com/taffish-org/freebayes)
30. [pymol :: v3.1.0](https://github.com/taffish-org/pymol)
31. [hifiasm :: v0.25.0](https://github.com/taffish-org/hifiasm) (amd64 only)
32. [haphic :: v1.0.6](https://github.com/taffish-org/haphic)
33. [autodock-vina :: v1.2.7](https://github.com/taffish-org/autodock-vina)
34. [rosetta :: vml-378](https://github.com/taffish-org/rosetta) (amd64 only & need avx2)
35. [gromacs :: 2025.1](https://github.com/taffish-org/gromacs)
36. [MMseqs2 :: 17](https://github.com/taffish-org/MMseqs2) (amd64 may need avx2)

### 🪢 FLOWs (1)
1. [gene-family-search :: v1.0.0](https://github.com/taffish-org/gene-family-search)
