<img align="right" width="50" height="50" src="images/logo.128px.png">

# Binding Scanner

DESCRIPTION

## Table of Contents

- [Binding Scanner](#binding-scanner)
  - [Table of Contents](#table-of-contents)
  - [General information](#general-information)
  - [Installation instructions](#installation-instructions)
    - [Step 1: Download and install Miniconda3](#step-1-download-and-install-miniconda3)
    - [Step 2: Clone the repository](#step-2-clone-the-repository)
    - [Step 3: Build and activate virtual environment for MAPP](#step-3-build-and-activate-virtual-environment-for-mapp)
  - [Optional: Download and parse PWMs from ATtRACT database](#optional-download-and-parse-pwms-from-attract-database)
  - [Workflow execution](#workflow-execution)
  - [Contributing](#contributing)
  - [Contact](#contact)

## General information

Binding Scanner is implemented as a [Snakemake] computational workflow.

[INSERT RULEGRAPH]

## Installation instructions

Snakemake is a workflow management system that helps to create and execute data processing pipelines. It requires [Python 3] and can be most easily installed via the [bioconda] channel from the [anaconda cloud] service.

### Step 1: Download and install Miniconda3

To install the latest version of [miniconda] please execute:  
  
[Linux]:
```bash
wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
source .bashrc
```

[macOS]:
```bash
wget https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
bash Miniconda3-latest-MacOSX-x86_64.sh
source .bashrc
```

### Step 2: Clone the repository

Please clone this git repository into a desired location (here: binding_scanner_git) with the following command:

```bash
git clone https://github.com/zavolanlab/binding-scanner.git binding_scanner_git
```

Cloning repositories requires [git] to be installed.

### Step 3: Build and activate virtual environment for MAPP

To ease the users in the installation process we have prepared a recipe for a *conda* virtual environment which contains all the software needed in order to run Binding Scanner. This environment might be created by the following script:

```bash
bash binding_scanner_git/scripts/create-conda-environment-main.sh
```

Following the built *conda* environment may be activated with:

```bash
conda activate binding-scanner
```

## Optional: Download and parse PWMs from ATtRACT database

## Workflow execution

## Contributing

This project lives off your contributions, be it in the form of bug reports,
feature requests, discussions, or fixes and other code changes. Please refer
to the [contributing guidelines](CONTRIBUTING.md) if you are interested to
contribute. Please mind the [code of conduct](CODE_OF_CONDUCT.md) for all
interactions with the community.

## Contact

For questions or suggestions regarding the code, please use the
[issue tracker][res-issue-tracker]. For any other inquiries, please contact us
by email: <zavolab-biozentrum@unibas.ch>

(c) 2020 [Zavolan lab, Biozentrum, University of Basel][res-zavolab]


[Snakemake]: https://snakemake.readthedocs.io/en/stable/
[Python 3]: https://www.python.org/download/releases/3.0/
[bioconda]: https://bioconda.github.io/
[anaconda cloud]: https://anaconda.org/
[miniconda]: https://docs.conda.io/en/latest/miniconda.html
[git]: https://git-scm.com/
[ATtRACT]: https://attract.cnic.es/index
[res-issue-tracker]: <https://github.com/zavolanlab/binding-scanner/issues>
[res-zavolab]: <https://zavolan.biozentrum.unibas.ch/>
