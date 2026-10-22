# COMP3104_Group29_Assignment

## Group Members
- **Leader:** Hooman Abedi (101570367) - [GitHub](https://github.com/hooman-abedi)
- **Member 2:** Martins Maduabuchi Ihechu (101496696) - [GitHub](https://github.com/martinsmaduabuchi)

## Project Description
This repository hosts the Group 29 assignment for the COMP3104 DevOps course at George Brown Polytechnic. The project focuses on collaborative Git workflows, a per-developer branching strategy, pull requests, merge conflict resolution, and continuous integration using GitHub Actions.

Each member created three files in the root of the repository:
- `STUDENTID_gb.txt` – information about George Brown College
- `STUDENTID_devops.txt` – information about the COMP3104 DevOps course
- `STUDENTID_sdlc.txt` – the importance of DevOps in the software development lifecycle

## Setup Instructions
1. Clone the repository:
```bash
   git clone https://github.com/hooman-abedi/COMP3104_Group29_Assignment.git
   cd COMP3104_Group29_Assignment
```
2. Create and switch to your own branch:
```bash
   git checkout -b STUDENTID-Name
   git push -u origin STUDENTID-Name
```
3. Keep your branch up to date with master:
```bash
   git pull origin master
```
4. No dependencies are required; all files are plain text and Markdown.

## CI/CD Pipeline
The project uses **GitHub Actions** for continuous integration. The workflow is defined in `.github/workflows/ci.yml` and:
- Runs automatically on every **push** and **pull request**, on any branch
- Uses the `ubuntu-latest` runner hosted by GitHub
- Checks out the repository code and lists the files to confirm the pipeline is working

The status of each run can be viewed in the **Actions** tab of the repository.

## Branching Strategy
The team uses a **per-developer** branching strategy:
- Each member works on their own branch named `STUDENTID-Name` (for example, `101570367-Hooman`).
- No one commits directly to `master`; it holds the reviewed, final version of the project.
- Members pull the latest `master` into their branch regularly to avoid conflicts.
- Changes are merged into `master` through **Pull Requests**, using the template in `.github/PULL_REQUEST_TEMPLATE.md`.
- Merge conflicts (for example, in `README.md`) are resolved by keeping all members' changes and removing the conflict markers.

## Pull Request Template
All pull requests use the template in `.github/PULL_REQUEST_TEMPLATE.md`, which includes a description, the type of change, and a review checklist.