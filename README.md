# CV of Md. Mosfikur Rahman

This repository contains the LaTeX source files, citations, and other relevant materials required to generate the Curriculum Vitae (CV) of Md. Mosfikur Rahman. The CV is automatically built and deployed using GitHub Actions.

## Repository Structure

- **sections/**: Contains individual LaTeX files for different sections of the CV.
    - `career_objective.tex`: Career objective section.
    - `education.tex`: Education and extracurricular activities section.
    - `extracurricular_activities.tex`: Extra Curricular Activities section.
    - `projects.tex`: Projects section.
    - `publications.tex`: Publications section.
    - `references.tex`: References section.
    - `research_collaborations.tex`: Research Collaboration section.
    - `research_interest.tex`: Research Interest section.
    - `skills.tex`: Skills section.
    - `work_experience.tex`: Work experience section. 

- **citations/**: Contains the bibliography file in BibTeX format.
    - `citations.bib`: Bibliographic references used in the CV.

- **.github/workflows/**: Contains the GitHub Actions workflow files.
    - `build.yml`: Workflow to build and deploy the CV as a PDF and HTML file.

- **CV_Md-Mosfikur-Rahman.tex**: Main LaTeX file that compiles the entire CV.

- **index.html**: Responsible Page for Providing CV

- **Makefile**: Contains commands to build the CV manually.

## Building the CV

### Using GitHub Actions
The CV is automatically built and deployed on GitHub Pages whenever there is a push to the repository. The GitHub Actions workflow (`.github/workflows/build.yml`) takes care of:
1. Building the PDF version of the CV using LaTeX.
2. Uploading the PDF as a GitHub artifact.
3. Deploying the CV to the `build` branch as an orphan branch on GitHub Pages.
4. Copying the `index.html` file to the `build` branch for easy access.

### Manually Building the CV
If you prefer to build the CV locally, you can use the `Makefile`. Ensure you have a LaTeX distribution installed.

```sh
make
```

This command will generate the `CV_Md-Mosfikur-Rahman.pdf` file in the current directory.

## Viewing the CV

- **PDF Version**: Available as an artifact after the GitHub Action runs. It can also be generated locally by running the `make` command.
- **HTML Version**: Can be viewed directly [here](https://mdmosfikurrahman.github.io/cv/).
