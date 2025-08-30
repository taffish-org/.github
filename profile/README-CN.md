# 欢迎来到 TAFFISH-ORG 👋

<p align="center"><strong>[ <a href="./README.md">English</a> | 简体中文 ]</strong></p>

TAFFISH（Tools And Flows Framework Intensify SHell）让您无需担心软件安装、环境冲突、容器管理……让您可以像编写 shell 脚本一样构建、使用和分享您自己的可移植、可重现的科学工具和工作流程。
> TAFFISH 仍然在开发中……



## ⛓️‍💥 Links
- taffish 官网: [https://taffish.com](https://taffish.com/taffish-cn.html)
- [github: taffish 仓库](https://github.com/taffish-org/taffish-hub)



## 📥 安装

### 正式安装 TAFFISH 前的准备工作：
在安装 TAFFISH 之前您需要先安装以下的软件与依赖：
- (MacOS 用户) homebrew & zstd
  - 如果您使用的是 MacOS，那么您需要先安装 [homebrew](https://brew.sh/zh-cn/)
  - 然后使用 homebrew 来安装 zstd: `brew install zstd`
- curl & git
  - Debian/Ubuntu: `sudo apt-get update; sudo apt-get install -y curl git`
  - MacOs: `brew install curl git`
- 至少一个容器管理软件: ([Docker](https://www.docker.com/)/[Podman](https://podman.io/)/[Apptainer(Singularity)](https://apptainer.org/index.html))，我们的建议是：
  - Windows(WSL)/Mac: [Docker](https://www.docker.com/) :: 适合于有 root 权限的个人用户；
  - Linux : [Apptainer](https://apptainer.org/index.html)/[Podman](https://podman.io/) :: 对于没有 root 用户的 linux 多用户系统（不过您需要先使用 root 用户或权限来全局安装 apptainer 和 podman，以便于所有非 root 用户可以正常使用这些容器管理软件）
    > 如果你需要的命令行工具每次都只是运行一次，那么选择 Apptainer 可能会更快；但如果你需要更改对应的环境设置，例如在 taf-app 中安装一些 python/R 包，或者使用 GUI 这种交互式软件，那么您应该安装使用 podman/docker，因为 Apptainer 只运行一次，并不能更改环境等。

> 如果你想为您计算机上的所有用户安装 taffish，你应该使用 root 来安装 taffish，例如在以下的安装命令前添加 'sudo'

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



## 快速开始

```bash
taf update
taf install -y hello
taf-hello --to $USER
```



## 🏠 TAFFISH-HUB (taf-apps) (68)

### ⚙️ BASE 基础 (8)
1. [debian :: v12](https://github.com/taffish-org/debian)
2. [python :: v3.13.2](https://github.com/taffish-org/python)
3. [conda :: v24.9.2](https://github.com/taffish-org/conda)
4. [sbcl :: v2.5.2](https://github.com/taffish-org/sbcl)
5. [R :: v4.4.3](https://github.com/taffish-org/R)
6. [intel-oneapi :: v2025.0.2-0-devel-ubuntu24.04](https://github.com/taffish-org/intel-oneapi)
7. [hello :: v1.0.0](https://github.com/taffish-org/hello)
8. [gui :: v1.0.0](https://github.com/taffish-org/gui) (支持 gui)

### 🛠️ TOOLs 工具 (59)
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
22. [hisat2 :: v2.2.1](https://github.com/taffish-org/hisat2) (仅 amd64 架构可用)
23. [mafft :: v7.525](https://github.com/taffish-org/mafft)
24. [clustal-omega :: v1.2.4](https://github.com/taffish-org/clustal-omega)
25. [bwa :: v0.7.18](https://github.com/taffish-org/bwa)
26. [gatk :: v4.6.1.0](https://github.com/taffish-org/gatk)
27. [salmon :: v1.10.3](https://github.com/taffish-org/salmon)
28. [Trinity :: v2.15.2](https://github.com/taffish-org/Trinity)
29. [freebayes :: v1.3.9](https://github.com/taffish-org/freebayes)
30. [pymol :: v3.1.0.gui](https://github.com/taffish-org/pymol) (支持 gui)
31. [hifiasm :: v0.25.0](https://github.com/taffish-org/hifiasm) (仅 amd64 架构可用)
32. [haphic :: v1.0.7](https://github.com/taffish-org/haphic)
33. [autodock-vina :: v1.2.7](https://github.com/taffish-org/autodock-vina)
34. [rosetta :: v378.ml](https://github.com/taffish-org/rosetta) (仅 amd64 架构可用 & 需要 avx2)
35. [gromacs :: v2025.1](https://github.com/taffish-org/gromacs)
36. [MMseqs2 :: v17](https://github.com/taffish-org/MMseqs2) (amd64 架构会需要 avx2)
37. [foldseek :: v10](https://github.com/taffish-org/foldseek) (amd64 架构会需要 avx2)
38. [esm-fold :: v1.0.3](https://github.com/taffish-org/esm-fold) (仅 amd64 架构可用)
    > 这个 taf-app 需要 GPU，所以你可能需要在 config.container.taf 中为 Docker 设置 '--gpus all' 或为 Apptainer 设置 '--nv'，你可以在 [TAFFISH-MANUAL](https://taffish.com/docs.html) 上查看详细信息。
39. [jellyfish :: v2.3.1](https://github.com/taffish-org/jellyfish)
40. [genomescope :: v2.0.1](https://github.com/taffish-org/genomescope)
41. [kmc :: v3.2.4](https://github.com/taffish-org/kmc) (没有 py_kmc_api)
42. [bamtools :: v2.5.2](https://github.com/taffish-org/bamtools)
43. [gfatools :: v0.5](https://github.com/taffish-org/gfatools)
44. [quast :: v5.3.0](https://github.com/taffish-org/quast) (仅 amd64 架构可用)
45. [minimap2 :: v2.29](https://github.com/taffish-org/minimap2)
46. [tgsgapcloser :: v1.2.1](https://github.com/taffish-org/tgsgapcloser)
47. [juicebox :: v3.1.4](https://github.com/taffish-org/juicebox) (支持 gui)
48. [busco :: v5.8.2](https://github.com/taffish-org/busco)
49. [trf :: v4.09.1](https://github.com/taffish-org/trf)
50. [augustus :: v3.5.0](https://github.com/taffish-org/augustus)
51. [EVidenceModeler :: v2.1.0](https://github.com/taffish-org/EVidenceModeler)
52. [RepeatMasker :: v4.1.8](https://github.com/taffish-org/RepeatMasker)
53. [samblaster :: v0.1.26](https://github.com/taffish-org/samblaster)
54. [NGenoemeSyn :: v1.43](https://github.com/taffish-org/NGenomeSyn)
55. [syri :: v1.7.1](https://github.com/taffish-org/syri)
56. [plotsr :: v1.1.1](https://github.com/taffish-org/plotsr)
57. [compleasm :: v0.2.7](https://github.com/taffish-org/compleasm)
58. [pandepth :: v2.26](https://github.com/taffish-org/pandepth)
59. [craq :: v1.0.9-alpha](https://github.com/taffish-org/craq)

### 🪢 FLOWs 流程 (1)
1. [gene-family-search :: v1.0.0](https://github.com/taffish-org/gene-family-search)

> 有时候，taf-flow 可能会使用一些不在 taf-hub 中的工具，因为有些工具需要 License，我们无法为它们制作 docker 镜像，但您可以自己安装它们并确保它在您的 PATH 环境变量中，这样 taffish 就可以使用它们了。
