# README

> **Note:** This readme template is based on one from the [Good Docs Project](https://thegooddocsproject.dev). You can find it and a guide to filling it out [here](https://gitlab.com/tgdp/templates/-/tree/main/readme). (_Erase this note after filling out the readme._)

<h1 align="center">
  <br>
  <a href="https://openpecha.org"><img src="https://avatars.githubusercontent.com/u/82142807?s=400&u=19e108a15566f3a1449bafb03b8dd706a72aebcd&v=4" alt="OpenPecha" width="150"></a>
  <br>
</h1>

## STT Combine Datasets

## Owner(s)
- [@spsither](https://github.com/spsither)
- [@TenzinGayche](https://github.com/TenzinGayche)

## RFXs
Requests for work (RFWs) and requests for comments (RFCs) associated with this project:
* [RFW0114: Recreate the benchmark dataset, ensuring a more balanced distribution across all departments](https://github.com/OpenPecha/Requests/issues/367)
* [RFW0125: Technical documentation about STT and TTS workflow for other developers](https://github.com/OpenPecha/Requests/issues/363)

## Table of contents
<p align="center">
  <a href="#project-description">Project description</a> •
  <a href="#who-this-project-is-for">Who this project is for</a> •
  <a href="#project-dependencies">Project dependencies</a> •
  <a href="#instructions-for-use">Instructions for use</a> •
  <a href="#contributing-guidelines">Contributing guidelines</a> •
  <a href="#additional-documentation">Additional documentation</a> •
  <a href="#how-to-get-help">How to get help</a> •
  <a href="#terms-of-use">Terms of use</a>
</p>
<hr>

## Project description

STT Combine Datasets helps you combine datasets from three different sources: stt.pecha.tools, prodigy and saymore for mv.
The data from  these sources are combined into a single 04_combine_all.tsv file. Benchmark dataset is created from this combined tsv. 


## Who this project is for
This project is intended for STT data pipeline maintainer who wants to update the aggrigate STT/TTS dataset. 


## Project dependencies
Before using STT Combine dataset, ensure you have:
* [saymore-report-generator](https://github.com/OpenPecha/saymore-report-generator)


## Instructions for use
Get started with STT Combine dataset by going through 
- 01_stt_pecha_tools.ipynb
  - Collect Data from stt.pecha.tools
- 02_prodigy.ipynb
  - Collect Data from legacy prodigy instance
- 03_mv_saymore.ipynb
  - Collect Data from STT Movie (MV). The data for Movie is collected from different repository in MonlamAI GitHub repository.
- 04_combine_all.ipynb
  - Combine all the data into one dataframe.
- 05_benchmark.ipynb
  - Create benchmark dataset using the highest quality grade of 3. Which means the task has been checked by the quality control team.


### Install STT Combine dataset
1. Clone the repository

    > git clone git@github.com:OpenPecha/stt-combine-datasets.git

2. Create a virtual environment
 
    a. Create a virtual environment
    > python3 -m venv .env

    b. Acticate the envronment
    > source .env/bin/activate
    
    b. _Substep 2_
3. Install required packages

  > pip install -r requirements.txt


## Contributing guidelines
If you'd like to help out, check out our [contributing guidelines](/CONTRIBUTING.md).


## Additional documentation

For more information:
* [Prodigy](https://prodi.gy/docs)
* [stt.pecha.tools](https://github.com/OpenPecha/pecha-tools-for-stt)
* [saymore](https://software.sil.org/saymore/)
* [saymore-report-generator](https://github.com/OpenPecha/saymore-report-generator)


## How to get help
* File an issue.
* Email us at openpecha[at]gmail.com.
* Join our [discord](https://discord.com/invite/7GFpPFSTeA).


## Terms of use
_Project Name_ is licensed under the [MIT License](/LICENSE.md).
