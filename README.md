# Geospatial Data Processing in Python: A Comprehensive Tutorial

https://github.com/martinchristen/EP2023Tutorial


Part I (90 min)
13:45 - 15:15 Club A

Coffee Break:
15:15 - 15:30

Part II (90 min)
15:30 - 17:00 Club A


## Installation

### Step 1: Conda

#### Variant 1: Install using Anaconda

Get the latest Version for Windows/MacOS/Linux here:

[https://www.anaconda.com/products/distribution#Downloads](https://www.anaconda.com/products/distribution#Downloads)

Install the latest Version for your operating system. This will take a while.

<hr/>

#### Variant 2: Install using Miniconda (recommended)

Download the Windows/MacOS/Linux installer here: [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)

<hr/>

### Step 2: Mamba

#### Install Mamba


Follow instructions here: [https://mamba.readthedocs.io/en/latest/installation.html](https://mamba.readthedocs.io/en/latest/installation.html)

You can also install mamba in an existing Anaconda/Miniconda installation: 

    conda install mamba -n base -c conda-forge
    
After installation use the "mamba" instead of "conda" command.


### Step 3: Create Geospatial Environment


Let's create our environment where we will install all the modules we need in this course.

    
    mamba create --name geopython310 python=3.10 jupyterlab –c conda-forge -y    
    
    mamba activate geopython310          

    mamba install gdal rasterio matplotlib geopandas geoplot folium osmnx pystac-client scikit-image pymongo geojson -c conda-forge -y  
    folium

Do this everytime from now on before starting Jupyter Lab:

    mamba activate geopython310
    jupyter lab
