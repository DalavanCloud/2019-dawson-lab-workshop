# Outline

**These notes are for the presenters.**

For the last two years the Jupyter team has been working on the new Jupyter
frontend: JupyterLab. While JupyterLab does of course allow the use of Jupyter
Notebooks, it goes beyond the classic Jupyter Notebook by providing a flexible
and extensible web application with a set of reusable components. Users can
arrange multiple notebooks, text editors, terminals, output areas, and custom
components using tabs and collapsible sidebars. These components are carefully
designed to enable the user to use them together or separately (for example, a
user can send code from a file to a console with a keystroke, or can pop out an
output from a notebook to work with it alone).

JupyterLab is based on a flexible application plugin system provided by
PhosphorJS that makes it easy to customize existing components or extend it
with new components. For example, users can install or write third-party
plugins to view custom file formats, such as GeoJSON, interact with external
services, such as Dask or Apache Spark, or display their data in effective and
useful ways, such as interactive maps, tables, or plots.

In this tutorial we’ll walk users thought the best way to make use of
JupyterLab, how to transition from the “classic” Jupyter Notebook frontend to
JupyterLab, and how to make the best use of the new powerful features of
JupyterLab.


## Overview of Jupyter and JupyterLab

###  8-8:10 (10 min) - introduction

By now you should have installed JupyterLab following the instructions in the
readme. For this tutorial, we are standardizing on a conda-based python
distribution (miniconda or Anaconda). We may not be able to help with
installation issues if you are using a different python distribution.

JupyterLab is in beta and that first time impression
are critical to usability of JupyterLab. We will show you what can be done, but
can still improve the usability quite a bit. When trying to do any task in the
exercise try to think first:
- How would I do that
- Then try to do the task.
    - Note what was intuitive, and what surprised you.
    - Tell it to us (via post it or issues)
- Feel free to interrupt with questions and clarification


- There will likely be a binder available, but do not rely on the conference
    wifi.

 - Introduction to JupyterLab (slides)

- Respond to FAQ:
  - Why JupyterLab ?
  - Can you get Lab and notebook at the same time: YES
  - No difference in file format; Notebooks files are the same

###  Tour of The User Interface
  - Following outline from https://github.com/jupyterlab/jupyterlab-demo/tree/master/narrative or https://gist.github.com/jasongrout/3039b5909734b1abf4544a8df68a8ace

###  Exercise 1 (and help installation issues if needed):

Look into the Exercise 1 folder, and follow the instruction in `Exercise-1.md`

### Q.A. 5 min

## Workflows around executing code

###  Minor Notebook UI interface difference - review from Exercise 1

  1. Arranging tabs through dragging
  2. How to author markdown and equations
  3. Collapsible cells
  4. drag cells, inside notebook and between views of files.
  5. Enable scrolling on outputs
  6. creating new view of outputs
  7. javascript rendering restrictions (removed in the next beta)

### Attaching kernels to multiple documents

  1. Executing code in a markdown file using an attached console.
  2. Developing libraries with notebook and Python files attached to same kernel
  3. Reloading modules?
  4. Create terminal, work with terminal next to code file and console. Maybe using ipython in terminal.
  5. Attaching a code console to the same kernel as a notebook.


### Exercise 2

- binding multiple documents to the same kernel
    - New Console for Notebook
    - Markdown file + console workflow
    - Python code file + console workflow
    - Open a notebook in classic notebook, modify, save and reopen in Lab.


## Customizing JupyterLab

###  MATTHIAS 10:25-10:35 (10min)

  1. Changing editor settings
  2. Changing theme
  3. Json config system overview
  4. Changing keyboard shortcuts

### Exercise 3 10:35-10:50 (15 min)
    1. change a keyboard shortcut
      1. Assign existing shortcut to new action.
      2. Assign new Keyboard shortcut to an existing action.
    2. add a keyboard shortcut (restart and run all)
    3. change an editor setting

## Extensions (10:50-11:30, 35 min)

1. Everything is an extension - show the package.json
2. Installing/listing/enabling/disabling plugins. `jupyter lab build`
3. `--core-mode`
4. Exercise 5 - writing your own extension

## What's new (11:30-11:40)

JupyterLab 0.33 prerelease out:
- Workspaces
- Extension manager
- Console show outputs
- Open in new browser tab
- Longer tabs
- Many, many upgrades

Extensions in the works:
- Keyboard shortcut editor
- Status bar
- Real-time collaboration


## Mention JupyterLab in a multiuser environment: point to jupyterlab docs
## Mention sprints!
## 11:40-12:00 QA, Question
