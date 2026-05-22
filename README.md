# Final Project

This repository contains our final project for the course IELE756, Preparación y Análisis de Datos. The project focuses on one anomaly found during the work developed in Tarea 3, using the ENO model and the comuna-level residuals.

## Team communes

The communes assigned to our team were

- Colina
- Melipilla
- Talagante

However, the anomaly analyzed in this final project comes from the broader residual table produced in Tarea 3, where San Pedro appeared as the most unexpected case in the Negative Binomial ENO model.

## Anomaly

San Pedro is the comuna that surprised us the most. In the Negative Binomial ENO model, it had the highest positive Pearson residual. The model expected about 346.81 ENO cases, but the observed value was 731. In other words, San Pedro reported around 384 more cases than expected, even after considering population size and the variables included in the model.

## Main notebook and headline figure

The notebook that produces the headline figure is located in the `notebooks` folder.

The file is

`notebooks/Tareas/final_anomaly.ipynb`

This notebook produces the main figure used to show the anomaly. The figure is saved as

`notebooks/figs/headline.png`

The notebook takes less than 5 seconds to run all cells.

## How to run the notebook

First, we created a virtual environment using Anaconda Prompt. To do this, we wrote the name we wanted for the environment and the Python version.

```bash
conda create -n Datos python=3.11.14
```

After that, we activated the environment:
```bash
conda activate Datos
```

Then, we installed the required dependencies using the requirements.txt file:
```bash
pip install -r requirements.txt
```

Finally, we selected the Datos environment as the kernel in VS Code and ran all the cells in

`notebooks/Tareas/final_anomaly.ipynb.`

## AI-use disclosure
We used AI tools throughout the course, mainly to help us give more structure and formality to the code cells and written explanations. We also used AI support in Tarea 3, especially for the regression models, because we did not have enough previous knowledge to code those models completely on our own. Even so, the results, figures, and final interpretation were reviewed by us before being included in the final project.