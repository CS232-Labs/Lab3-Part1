# Lab3-Part1

VIVA will be conducted for this Lab.

## Instructions for Mac Users:
* Install Rosetta:
```
/usr/sbin/softwareupdate --install-rosetta --agree-to-license
```
* Open Docker desktop and start the CS251 container
``` 
sudo docker start cs251
sudo docker exec -it cs251 /bin/bash
```
* Navigate to the `host` Directory, which is a shared folder for your local machine and the docker container.
* Download the `spim` binary and `exceptions.s` file in the repo, to the `Lab3` directory.
* Navigate to the `Lab3` directory inside the docker container.
* For Q1, just run the binaries(`./program1`, `./program2`)
## For Q2, to use spim inside docker: 
* Run the following:
```
    chmod +x spim
    ./spim -exception_file exceptions.s -f <filename>.s
```
## Installation Instructions for Linux Users:

### spim
```
sudo apt-get install spim
```
## Tutorial Videos:
* [Youtube Tutorial 1](https://www.youtube.com/watch?v=tzkwW2SXWmQ)
* [Youtube Tutorial 2](https://www.youtube.com/watch?v=9sumRfIgaHs)
* [Youtube Tutorial 3](https://www.youtube.com/watch?v=9if9kS92Ha8)

## Reading Material:
* [Presentation from the video](https://docs.google.com/presentation/d/16KDDNamMbnK1UpsAikwRhXRHEFm2Guj8dgiY6tPH8Kk/edit?usp=sharing)
* [System calls in MIPS](https://courses.missouristate.edu/kenvollmar/mars/help/syscallhelp.html)
* [MIPS Cheat Sheet](https://inst.eecs.berkeley.edu/~cs61c/resources/MIPS_Green_Sheet.pdf)
* [Factorial Program in x86](https://abnerrjo.github.io/blog/2016/02/21/factorial-function-in-assembly/)
* [Regsiters & Memory in x86](https://en.wikibooks.org/wiki/X86_Assembly/X86_Architecture)
* [System calls for Linux in x86](https://blog.rchapman.org/posts/Linux_System_Call_Table_for_x86_64/)
* [x86 Instruction cheatsheet](https://www.felixcloutier.com/x86/)

## Questions:
* [Q1](Q1/README.md)
* [Q2](Q2/README.md)

## Submission Instructions:
* Clone this repo, name it as `{roll_number}_cs232_lab3`
* <span style="color:red">Make sure to keep your repo as `private` (It's your responsibility to keep it private, we will not be responsible for any plagiarism/loss of marks due to this)</span>
* Final submission structure should look like this:
```
{roll_number}_cs232_lab3
├── Q2
│   ├── inverse.s
├── Q3
│   ├── inplacemergesort.s
├── Q4
│   ├── io.asm
│   ├── Makefile
│   ├── matrix-multiplication-testbench.asm
│   ├── matrix-multiplication-ijk.asm
│   ├── matrix-multiplication-ikj.asm
│   ├── matrix-multiplication-jik.asm
│   ├── matrix-multiplication-jki.asm
│   ├── matrix-multiplication-kij.asm
│   ├── matrix-multiplication-kji.asm
│   ├── memory-test.asm
├── {roll_number}-report.pdf
```
* You need to submit a pdf report named `{roll_number}-report.pdf` containing the details required by the questions.
* Submit a compressed file `{roll_number}_cs232_lab3.tar.gz`
* Here, `{roll_number}` is your roll number.
