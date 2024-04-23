<div align="center" id="top"> 
  <!-- <img src="./.github/app.gif" alt="CWL Project" /> -->

  &#xa0;

  <!-- <a href="https://cwlproject.netlify.app">Demo</a> -->
</div>

<h1 align="center">CWL Project: Formal Verification of BFT Protocol Lumiere</h1>

<p align="center">
  <img alt="Github top language" src="https://img.shields.io/github/languages/top/Apeksha115908828/cwl-project?color=56BEB8">

  <img alt="Github language count" src="https://img.shields.io/github/languages/count/Apeksha115908828/cwl-project?color=56BEB8">

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/Apeksha115908828/cwl-project?color=56BEB8">

  <img alt="License" src="https://img.shields.io/github/license/Apeksha115908828/cwl-project?color=56BEB8">

  <!-- <img alt="Github issues" src="https://img.shields.io/github/issues/Apeksha115908828/cwl-project?color=56BEB8" /> -->

  <!-- <img alt="Github forks" src="https://img.shields.io/github/forks/Apeksha115908828/cwl-project?color=56BEB8" /> -->

  <!-- <img alt="Github stars" src="https://img.shields.io/github/stars/Apeksha115908828/cwl-project?color=56BEB8" /> -->
</p>

<!-- Status -->

<!-- <h4 align="center"> 
	🚧  CWL Project 🚀 Under construction...  🚧
</h4> 

<hr> -->

<p align="center">
  <a href="#dart-about">About</a> &#xa0; | &#xa0; 
  <a href="#white_check_mark-requirements">Requirements</a> &#xa0; | &#xa0;
  <a href="#checkered_flag-starting">Starting</a> &#xa0; | &#xa0;
  <a href="#memo-license">License</a> &#xa0; | &#xa0;
  <a href="https://github.com/Apeksha115908828" target="_blank">Author</a>
</p>

<br>

## :dart: About ##

Formal verification is a process of mathematically proving the correctness and the adherence of a consensus protocol to the specifications as described. It is crucial to ensure the properties such as correctness, safety, liveness and fault tolerance while working with consensus protocols in Distributed Systems, and formal verification guarantees the reliability of the consensus algorithms in presence of faulty processors. In this project, we have selected [Lumiere](https://arxiv.org/abs/2311.08091v2), a byzantine fault tolerant protocol to perform the runtime formal verification, wherein we will be writing the formal specifications of the algorithm and checker for verifying the correctness of the proposed protocol.

## :white_check_mark: Requirements ##

Before starting :checkered_flag:, you need to have [Git](https://git-scm.com) and [Python](https://www.python.org/) installed and [Distalgo](https://distalgo.cs.stonybrook.edu/).

## :checkered_flag: Starting ##

```bash
# Clone this project
$ git clone https://github.com/Apeksha115908828/cwl-project

# Access
$ cd cwl-project

Install python 3.78
then install distalgo using pip

\$ pip3 install pyDistAlgo
create virtual environment
go to cd . and activate the venv created:
\$ cd .
\$ source bin/activate

to execute, go to the folder pbft
\$ cd lumiere
\$ python -m da spec.da
to execute the checker
\$ python -m da checker.da
```

File: lumiere/spec.da has implementation for lumiere protocol using distalgo. Currently specs are only implemented to the extend I could understand the protocol, I shall continue working on the protocol and keep updating the github repository.

Documentation:
Tool used: pdoc(version=0.10.0)
File: [lumiere/build/spec.html](lumiere/build/spec.html)
File: src/spec.py is just a copy of spec.da to generate the documentation as pdoc doesn't allow other extensions for generating documentation.

## :memo: License ##

This project is under license from MIT. For more details, see the [LICENSE](LICENSE) file.


Made with :heart: by <a href="https://github.com/" target="_blank">Apeksha Bodade</a>

&#xa0;

<a href="#top">Back to top</a>
