Welcome to the oresat-structure wiki! This is the go-to guide for contributing to the OreSat project. Everything you may need to download the repository and contribute can be found here! Below you can find the necessary info to get started!

### Why GitHub?

The OreSat Project is an open-source project. Therefore, the source files are hosted in GitHub so ANYONE can access these files if needed. Git, the version control system that powers GitHub, allows us to revisit old versions of files if necessary.

The contribution instructions for OreSat all are written for use in the Git Bash command line. This is because the command-line interface provides the necessary flexibility to manage a repository as complex as oresat-structure.

## Downloading the Repository

1. Clone the repository to your system<be>

`git clone https://github.com/oresat/oresat-structure.git`

> **NOTE:** The repository is around 9GB in size. If you would not like to download the entire repository history, use the following command instead<be>
> 
> `git clone --depth 1 https://github.com/oresat/oresat-structure.git`
> * The --depth 1 flag indicates that only the most recent commit will be cloned
> 
> To also clone all branches, use the following command<be>
> 
> `git clone --depth 1 --no-single-branch https://github.com/oresat/oresat-structure.git`
> * the --no-single-branch flag indicates that all branches should be cloned (since --depth automatically runs --single-branch)

2. Download Solidworks

3. Open up the files to get started!

## Contributing to the Project

Currently, contributed to the projects operate in their own branches, labeled "dev_[Insert First Name]". For example, a branch for Marvin would be labeled "dev_marvin". However, before you can contribute, you must join the GitHub Organization

To join, please message Joe or Andrew on Slack to get added! To learn how to join the OreSat Project, check out [our website](https://www.oresat.org)!

After you have joined, go to "Version Control For Structure (Git)" to learn how to create a branch, add to the project, and update your files!