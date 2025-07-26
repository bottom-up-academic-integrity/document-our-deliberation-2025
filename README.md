# # Open Letter 

This repository contains the required information to compile a pdf version of the text specified in `content.typ`. It uses Typst to compile the pdf.

All the technical stuff and styling is handled by `main.typ`.

### How to edit / use

To make a new version of the document, make a change in the [content.typ](content.typ) and push that to GitHub. (or make an edit in the web interface and save it).

GitHub workflows will then spin up a virtual machine and use that to run typst and generate a fresh pdf that reflects the latest change you made in `content.typ`.

The new pdf can be found under the `Actions` tab in the GitHub web interface for this repository. On that page, open the most recent workflow run. On the page of the latest workflow, you can download an 'Artifact' that contains the latest pdf.

![screenshot of github interface showing the artifact page and download button](media/github-explanation.JPG)

To summarise

1. Change `contents.typ`
2. Save and push to server (done automatically if you change via web interface)
3. Wait for GitHub workflow to run (typically < 3min)
4. Download the new pdf from the `Actions` page.

> [!NOTE] 
>
> GitHub workflow currently broken as the template submodule is private. Use the local approach outlined below.

### Compiling locally

If you have Typst installed, you can also compile the document by running/inspecting the scripts in the [template/utils](template/utils) folder.

