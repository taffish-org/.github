# Welcom to TAFFISH-ORG 👋

<p align="center"><strong>[ English | <a href="./README_CN.md">简体中文</a> ]</strong></p>

TAFFISH(Tools And Flows Framework Intensify SHell) allows you to avoid worrying about software installation, environment conflicts, container management, cluster operations, ...... Build, use, and share your own portable, reproducible scientific tools and workflows just like shell commands.
> TAFFISH is still on build ...



## ⛓️‍💥 Links
- [taffish-official-website](https://taffish.com)
- [github: taffish-hub](https://github.com/taffish-org/taffish-hub)



## 📥 Install

### Container Apps before TAFFISH:
You need to install these apps before installing TAFFISH:
- (for MacOS) homebrew & zstd
  - If you use MacOS, you may need to install [homebrew](https://brew.sh/) first
  - And then use homebrew to install zstd: `brew install zstd`
- curl & git
  - Debian/Ubuntu: `sudo apt-get update; sudo apt-get install -y curl git`
  - MacOs: `brew install curl git`
- At least one Container App([Docker](https://www.docker.com/)/[Podman](https://podman.io/)/[Apptainer(Singularity)](https://apptainer.org/index.html)) for taffish. And we suggest:
  - Windows(WSL)/Mac: [Docker](https://www.docker.com/) :: for people who are root users
  - Linux : [Apptainer](https://apptainer.org/index.html)/[Podman](https://podman.io/) :: for people who are not root users (but you may need root to install them to make sure all non-root users can use these container apps)
    > If you just need the command line tool for once run, Apptainer may be faster, but if you need to change some environment sets such like installing some python/R packages in the taf-app, maybe podman/docker will be better, because Apptainer just for once running without enviroment changing.

> If you want to install taffish for all users on your computer, you shold use root to install taffish, such like add 'sudo' before the install command ⬇️.

### ![tiny-Debian-OpenLogo](https://github.com/user-attachments/assets/fc2e8de9-fbfc-4675-8d37-5181474be5b3) Debian12 (Linux)

```bash
sh -c "$(curl -fsSL https://github.com/taffish-org/taffish-install/releases/download/latest/install-taffish-debian12-amd64-beta.sh)" -n
```

### ![tiny-Ubuntu-logo-2022](https://github.com/user-attachments/assets/fcdbcd66-0fe8-42a9-bf44-714c24d0fbdf) Ubuntu (Linux) (>=18.04.1-LTS)

```bash
sh -c "$(curl -fsSL https://github.com/taffish-org/taffish-install/releases/download/latest/install-taffish-ubuntu-amd64-beta.sh)" -n
```

### ![tiny-CentOS-logo](https://github.com/user-attachments/assets/676ffdc2-2f42-4fe1-b6b7-334b84b155f3) CentOS 8 (Linux)

```bash
sh -c "$(curl -fsSL https://github.com/taffish-org/taffish-install/releases/download/latest/install-taffish-centos8-amd64-beta.sh)" -n
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



## 🏠 TAFFISH-HUB (taf-apps) (62)

### ⚙️ BASE (8)
1. [debian :: v12](https://github.com/taffish-org/debian)
2. [python :: v3.13.2](https://github.com/taffish-org/python)
3. [conda :: v24.9.2](https://github.com/taffish-org/conda)
4. [sbcl :: v2.5.2](https://github.com/taffish-org/sbcl)
5. [R :: v4.4.3](https://github.com/taffish-org/R)
6. [intel-oneapi :: v2025.0.2-0-devel-ubuntu24.04](https://github.com/taffish-org/intel-oneapi)
7. [hello :: v1.0.0](https://github.com/taffish-org/hello)
8. [gui :: v1.0.0](https://github.com/taffish-org/gui) (support gui)

### 🛠️ TOOLs (53)
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
30. [pymol :: v3.1.0.gui](https://github.com/taffish-org/pymol) (support gui)
31. [hifiasm :: v0.25.0](https://github.com/taffish-org/hifiasm) (amd64 only)
32. [haphic :: v1.0.7](https://github.com/taffish-org/haphic)
33. [autodock-vina :: v1.2.7](https://github.com/taffish-org/autodock-vina)
34. [rosetta :: v378.ml](https://github.com/taffish-org/rosetta) (amd64 only & need avx2)
35. [gromacs :: v2025.1](https://github.com/taffish-org/gromacs)
36. [MMseqs2 :: v17](https://github.com/taffish-org/MMseqs2) (amd64 may need avx2)
37. [foldseek :: v10](https://github.com/taffish-org/foldseek) (amd64 may need avx2)
38. [esm-fold :: v1.0.3](https://github.com/taffish-org/esm-fold) (amd64 only)
    > This taf-app need GPU, so you may need to set '--gpus all' for Docker or '--nv' for Apptainer in your config.container.taf, you can see details on [TAFFISH-MANUAL](https://taffish.com/docs.html)
39. [jellyfish :: v2.3.1](https://github.com/taffish-org/jellyfish)
40. [genomescope :: v2.0.1](https://github.com/taffish-org/genomescope)
41. [kmc :: v3.2.4](https://github.com/taffish-org/kmc) (no py_kmc_api)
42. [bamtools :: v2.5.2](https://github.com/taffish-org/bamtools)
43. [gfatools :: v0.5](https://github.com/taffish-org/gfatools)
44. [quast :: v5.3.0](https://github.com/taffish-org/quast) (amd64 only)
45. [minimap2 :: v2.29](https://github.com/taffish-org/minimap2)
46. [tgsgapcloser :: v1.2.1](https://github.com/taffish-org/tgsgapcloser)
47. [juicebox :: v3.1.4](https://github.com/taffish-org/juicebox) (support gui)
48. [busco :: v5.8.2](https://github.com/taffish-org/busco)
49. [trf :: v4.09.1](https://github.com/taffish-org/trf)
50. [augustus :: v3.5.0](https://github.com/taffish-org/augustus)
51. [EVidenceModeler :: v2.1.0](https://github.com/taffish-org/EVidenceModeler)
52. [RepeatMasker :: v4.1.8](https://github.com/taffish-org/RepeatMasker)
53. [samblaster :: v0.1.26](https://github.com/taffish-org/samblaster)

### 🪢 FLOWs (1)
1. [gene-family-search :: v1.0.0](https://github.com/taffish-org/gene-family-search)

> Sometimes, a taf-flow could use some tools which are not in taf-hub, because some tools need Licence, we can't make docker images for them, but you can install them by yourselves and make sure it's in your PATH, so that taffish can use it.
