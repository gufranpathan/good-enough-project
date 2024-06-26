# Good Enough Project

A cookiecutter project structure based on the [Reproducible Science Cookiecutter](https://github.com/mkrapp/cookiecutter-reproducible-science) template by [Mario Krapp](https://github.com/mkrapp), and with close resemblances to the philosophy of [Cookiecutter Data Science](https://github.com/drivendata/cookiecutter-data-science): *A logical, reasonably standardized, but flexible project structure for doing and sharing data science work.*

The name (and most of the structure) are derived from the paper [Good Enough Practices in Scientific Computing](https://doi.org/10.1371/journal.pcbi.1005510), Wilson _et al._, PLOS Computational Biology (2017).

## Requirements

Install `cookiecutter` on the command line: `pip install cookiecutter`    

## Usage

To start a new science project:

`cookiecutter gh:bvreede/good-enough-project`

## Project Structure

The project structure distinguishes three kinds of folders:
- read-only (RO): not edited by either code or researcher
- human-writeable (HW): edited by the researcher only.
- project-generated (PG): folders generated when running the code; these folders can be deleted or emptied and will be completely reconstituted as the project is run.


```
.
├── .gitignore
├── README.md
├── requirements.txt
├── data               <- All project data, ignored by git
│   ├── raw            <- The original, immutable data dump
│   ├── processed      <- Intermediate data that has been transformed
│   └── output         <- Outputs used in manuscript or reports 
│        ├── figures   <- Figures for the manuscript or reports
│        └── tables    <- Tables for the manuscript or reports 
└── src                <- Source code for this project

```


## License

This project is licensed under the terms of the [MIT License](/LICENSE.md).
