# NSDF-OpenViSUS Cookbook

<img src="./thumbnails/nsdf.png" alt="NSDF Logo" width="300"/>

This Project Pythia Cookbook covers **working with large-scale scientific data using OpenViSUS**.

## Motivation

OpenViSUS enables interactive analysis and visualization of petabyte-scale scientific datasets on any device, from supercomputers to personal laptops. This cookbook will help you learn how to store, query, and visualize big data efficiently using OpenViSUS tools and formats.

### Hierarchical Z-Order Data Storage

The NSDF-OpenVISUS framework leverages hierarchical Z-order curve for efficient data storage and access. This method organizes data to preserve spatial locality, enabling fast multi-resolution queries and scalable visualization.

Below is an illustration of hierarchical Z-order refinement:

<img src="./thumbnails/data_layout_OV.png" alt="Hierarchical Z-order refinement" width="350"/>

**Panels:**
* (a) Initial coarse data points (green) and new level data (red).
* (b), (c) Progressive subdivision, adding new data points in Z-order.
* (d) Fully refined grid, showing efficient hierarchical access.

**Note:** This cookbook is part of the larger OSDF Cookbook, which can be found at <https://projectpythia.org/osdf-cookbook/>.


## Authors

[Aashish Panta](https://github.com/aashishpanta0), Valerio Pascucci,  Amy Gooch, [Giorgio Scorzelli](https://github.com/scrgiorgio)

### Contributors

<a href="https://github.com/sci-visus/OpenVisus/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=sci-visus/openvisuspy" />
</a>

## Structure

This cookbook is organized into sections, which you can select from the sidebar on the left (see image above). Each section covers a different topic or dataset relevant to NSDF-OpenVISUS:


### Preamble
Information on citing this NSDF-OpenVISUS Cookbook.

### Introduction to NSDF-OpenVISUS
Overview of the NSDF-OpenVISUS framework, its motivation, and its role in scientific data visualization.

### NASA DYAMOND Datasets (C1440–LLC2160)
Workflows for visualizing and analyzing NASA DYAMOND atmospheric and ocean datasets.

### ECCO LLC4320 Datasets
Visualization and analysis of the ECCO LLC4320 ocean dataset, including data access, processing, and interactive exploration.


## Running the Notebooks

You can either run the notebook using [Project Pythia Binder](https://binder.projectpythia.org/) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through [Binder](https://binder.projectpythia.org/), which enables the execution of a [Jupyter Book](https://jupyterbook.org) in the cloud. To launch a Pythia Cookbooks chapter via Binder, click the rocket ship icon at the top right corner of the book chapter and select “launch Binder.” After a moment, you should be presented with a notebook that you can interact with. You’ll be able to execute and even change the example programs. Code cells have no output at first, until you execute them by pressing {kbd}`Shift`+{kbd}`Enter`. See [Getting Started with Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter) for more details.

Note: Not all Cookbook chapters are executable. If you do not see the rocket ship icon, you are not viewing an executable book chapter.

### Running on Your Own Machine

If you are interested in running this material locally on your computer, follow this workflow:

1. Clone the `https://github.com/ProjectPythia/nsdf-openvisus-cookbook` repository:

   ```bash
   git clone https://github.com/ProjectPythia/nsdf-openvisus-cookbook
   ```

2. Move into the `OpenVisus` directory:
   ```bash
   cd nsdf-openvisus-cookbook
   ```
3. Create and activate your conda environment from the `environment.yml` file:
   ```bash
   conda env create -f environment.yml
   conda activate nsdf-cookbook
   ```
4. Move into the `Samples/jupyter` directory and start up JupyterLab:
   ```bash
   cd notebooks
   jupyter lab
   ```

## References
- <a href="https://nationalsciencedatafabric.org/" target="_blank">National Science Data Fabric</a>
- <a href="https://github.com/sci-visus/OpenVisus" target="_blank">OpenVisus</a>
- <a href="https://github.com/sci-visus/OpenVisuspy" target="_blank">OpenVisuspy</a>

---
Please consult these papers for technical details and use cases:

- <a href="https://arxiv.org/abs/2408.11831v1" target="_blank"> Web-based Visualization and Analytics of Petascale data: Equity as a Tide that Lifts All Boats </a>
- <a href="https://arxiv.org/abs/2009.03254" target="_blank"> Interactive Visualization of Terascale Data in the Browser: Fact or Fiction?  </a>
- <a href="https://sci.utah.edu/publications/Kum2014a/KumarISC2014.pdf" target="_blank">Fast Multiresolution Reads of Massive Simulation Datasets</a>

 *Please reach out to Aashish Panta, Giorgio Scorzelli or Valerio Pascucci for any concerns about the notebook. Thank you!*
- Aashish Panta (aashishpanta0@gmail.com)
- Giorgio Scorzelli (scrgiorgio@gmail.com)
- Valerio Pascucci (pascucci.valerio@gmail.com)
