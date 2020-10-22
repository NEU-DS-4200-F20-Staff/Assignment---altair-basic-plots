# Assignment — Altair Basic Plots
​
This repository is your starting point for the assignment and includes the instructions below.

Unlike the D3 assignments, we will not be using GitHub pages so there is no link to update here.

# Aim of the assignment

[Altair](https://altair-viz.github.io/) is a declarative statistical visualization library for Python, based on [Vega](http://vega.github.io/vega) and [Vega-Lite](http://vega.github.io/vega-lite). In this assignment, you are going to learn to create two basic visualizations using Altair.

If you run into problems see the **Tips, tricks, and troubleshooting** section below.

# Instructions

## Setup instructions

1. Clone the repo.

1. `CD` to the repo directory. Create and activate a virtual environment for this project. You may need to modify the code you use depending on what Python you have installed and how your machine is configured.

1. Run the setup commands below.

    * On macOS or Linux, run these three commands *separately* in case there are errors:
        ```
        python3 -m venv env
        ```
        ```
        source env/bin/activate
        ```
        ```
        which python
        ```
    * On Windows, run these three commands *separately* in case there are errors:
        ```
        python -m venv env
        ```
        ```
        .\env\Scripts\activate.bat
        ```
        ```
        where.exe python
        ```
    Check the path(s) provided by `which python` or `where.exe python` — the first one listed *should* be inside the `env` folder you just created.

1. Install necessary packages. Note that you should install the exact versions of the packages.
    ```
    pip install -r requirements.txt
    ```
    This may take a few minutes.

If you have trouble running any of these steps, see the [Troubleshooting section](#troubleshooting) below.

## Run Jupyter Lab and create a notebook

1. Run `jupyter lab`. It should open your default browser and let you select select any Jupyter Notebook .ipynb file.
1. Create a new Jupyter Notebook .ipynb file and give it a descriptive title.

Once you have written code in a cell you can run it with `ctrl+enter`. In the menu you can run all cells and restart the kernel to clear variables.

## Load the Dataset
We will be using the [Netflix Movies and TV Shows](https://www.kaggle.com/shivamb/netflix-shows) dataset on Kaggle.
This dataset includes all the TV Shows and Movies that have been uploaded on Netflix before January 17, 2020.
It is included here as `netflix_titles.csv`.

1. In your notebook, load the CSV file [into a Pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html#pandas.read_csv).
1. Create a simple visualization in Altair using that DataFrame. See the documentation on [specifying data in Altair](https://altair-viz.github.io/user_guide/data.html).

## Create Two Interesting Visualizations

1. Using Altair, create two visualizations using the Netflix Movies and TV Shows trying to find interesting insights in the dataset. 
    * Here are some possible questions you can answer:
        * Does the distribution of movie lengths appear gaussian?
        * Who are the directors with the highest average movie rating?
        * Has the rate at which Netflix adds new movies changed through the years?
    * The visualizations must be created by separate code cells in the notebook.
    * Each visualization must be accompanied by a Markdown cell that explains the visualization, your choices, and the point you are trying to convey.
    * You are free to create any visualization that you like. However, you must explain the reasoning behind your choices and the visualization must be appropriate for the information you are attempting to learn or convey.

## Include Your Visualizations in this `README.md`

1. **Include both of your images here so that it will show as part of `README.md` on GitHub.** (Not a GitHub Pages site.) If, for whatever reason, we are unable to run your notebook we can at least see the output.

    Please see the [GitHub Markdown documentation](https://guides.github.com/features/mastering-markdown/) for how to include an image.
    Note that Altair lets you save a PNG (recommended) or SVG file directly using the ⋯ menu in the top-right of a visualization.
    It will likely be easier to include a PNG file correctly than an SVG.
    However, SVGs are advantageous for publication as they allow futher editing using Inkscape or Illustrator.

## Quit instructions
1. Make sure to save your .ipynb file and shutdown Jupyter Lab properly through the file menu. Otherwise you need to use `jupyter notebook stop`.
​
1. Deactivate the venv to return to your terminal using `deactivate`.

## Commit and push your code (but first...)

1. Only if you have made any changes to the required packages you should export a list of all installed packages and their versions:
   ```
   pip freeze > requirements.txt
   ```

1. **Before you commit a Jupyter Notebook .ipynb file, clear the outputs of all cells.** This decreases file size, removes unnecessary metadata, and makes diffs easier to understand. In Jupyter Lab you can use the GUI: Edit->Clear All Outputs.

1. Make sure to add all your required files, including the .ipynb file and any images.

1. Finally, commit all your local files and push them to the remote repository on GitHub which was generated by GitHub Classroom.

# Submission instructions

1. Ensure that:
    - both visualizations and prose are present in your notebook,
    - both visualizations are present in `README.md`,
    - all of your required files including the .ipynb file and any images are pushed to the remote repository on GitHub which was generated by GitHub Classroom.
    
    We will grade based on what is available in that repository.

1. Submit the URL of **your GitHub Classroom-generated repository** (not a GitHub Page — we're not using it for this assignment anyway) to [the associated assignment on Canvas](https://northeastern.instructure.com/courses/18721/assignments/573831). **Do not submit a link to a personal repository. It must be within our class GitHub organization.**

# Tips, tricks, and troubleshooting

See https://github.com/NEU-DS-4200-F20-Staff/General_Course_Information/blob/master/altair.md

# Assignment setup (for instructors only)

See https://github.com/NEU-DS-4200-F20-Staff/General_Course_Information/blob/master/assignment-setup.md