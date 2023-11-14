<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>

<div>
  <h2 align="center">nt</h2>
  
  <p align="center"> 
    Terminal Note Organization Application 💻 
  </p>
    
  <p align="center">
    <br />
    <a href="https://github.com/lukaflores/nt/issues">Report Bug</a>
    ·
    <a href="https://github.com/lukaflores/nt/issues">Request Feature</a>
  </p>
</div>

![result](https://github.com/LukaFlores/nt/assets/85141937/b9a0e78b-eb14-434f-9cfd-7342c12426f7)

<!-- ABOUT THE PROJECT -->
## About The Project

This project is a system to organize my latex notes and assigments for school and personal study. The tool allows me to open notes quickly as well as track completion of assignments.

- ❌ represents that the assignment hasn't been started
- 🔶 represents that the assignment has been started
- ✅ represents that the assignment has been completed

Note: Current version has not been updated to be compatible with linux (works with MacOS)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Config

At the top of the file there are changeable variables

```
fileType=".tex"
subDir="agnDir" # Directory Containing Notes / Assignments for Specifc Application
homeDirectory=~/notes/edu # Directory Containing all Applications of "nt"
databaseTXT="completed-assignments.txt" # Name of File to Store Complete Assignments / Notes
IPdatabaseTXT="inprogress-assignments.txt" # Name of File to Store Assignments / Notes that are In Progress
```
For example I currently have two commands for two different directories 
``
ag # Responsible for all School Assignment
``
``
nt # Responsible for all Personal Study Notes
``
Example of the way I have structure my personal system

```
~/notes
  └── edu
     ├── dir # Dirctory for Personal Notes
     |    ├── Computer Science # Subject of Personal Study
     |    |       └── Compresssion Reading # First Reading of Subject Computer Science
     |    └── Philosphy # Second Subject of Personal Study
     |            ├── Ethics Reading  # First Reading of Subject Philosphy
     |            └── Metaphysics Reading # Second Reading of Subject Philosphy
     |
     ├── agnDir # Dirctory for School Assignments
     |    ├── Discrete Math # Subject of School
     |    |       └── Homework 1 # HW1 of Discrete Math 
     |    └── English # Second Subject of School
     |            ├── Essay 1  # First Assignment of Subject English
     |            └── Essay 2  # Second Assignment of Subject English
     |
     ├── completed-assignments.txt # To Store Complete Assignments (Sub-Directory: agnDir)
     |
     ├── inprogress-assignments.txt # To Store Assignments that are In Progress (Sub-Directory: agnDir)
     |
     ├── completed-notes.txt # To Store Complete Notes (Sub-Directory: dir)
     |
     └── inprogress-notes.txt # To Store Notes that are In Progress (Sub-Directory: dir)
```


Example of Assignment / Reading in the Compression Reading
```
CompressionReading
     ├── source 
     |    └── compressionReading.pdf 
     ├── compresssionReading.tex
     └── compressionReading.pdf
```

Note: When the script opens the directory it opens:
  - the ".tex" file in `nvim`
  - the ".pdf" file associate with ".tex" file in `Preview (Mac)` or `Zathura (Linux)`
  - the ".pdf" or ".html" file in `/source` using `Preview (Mac)` or `Zathura (Linux)` or `qutebrowser (linux)`

The note taking file can be change from ".tex" at the top of the file `fileType=""`
The file opening commands can be change in `openFiles()` 

<p align="right">(<a href="#readme-top">back to top</a>)</p>


### Installation (With My Dotfiles)

1. Clone the repo
   ```sh
   git clone https://github.com/lukaflores/dotfiles.git
   ```
2. Move Repository to `~/code` 
   ```sh
    mv dotfiles ~/code 
   ```
3. Use install script (Don't provide a parameter to see options) 
   ```sh
   ./install.sh all
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->
## Usage

Depending on the bin command associated with the file it as simple as calling it, in the video example above I use "ag" but within my dotfiles I also use "nt" for my personal notes directory 

```
  ag
```
or
```
  nt
```

<!-- CONTACT -->
## Contact

Luka Flores - [@LukaFlores12](https://twitter.com/LukaFlores12)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

