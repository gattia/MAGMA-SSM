# MAGMA-SSM
## Background / Overview
This repository includes data to create the statistical shape model (SSM) from the publication: 

"Investigating Acute Changes in Osteoarthritic Cartilage by Integrating Biomechanics and Statistical Shape Models of Bone: Data from the Osteoarthritis Initiative"

Included in the jupyter notebook `load_and manipulate_statistical_shape_model.ipynb` are code and examples to load the SSM into python and to manipulate it. 

Included are the Principal Component vectors (PCs) and coinciding variances from statistical shape models built for the tibia and femur. These SSMs were built from 113 knee MRIs. 13 of the knees were acquired for the experimental study in the manuscript. The other 100 knees were sampled from the Osteoarthritis Initiative (OAI). All knees (local and OAI) were from women. The 100 knees from the OAI include 20 from each of the 5 Kellgren and Lawrence (KL) osteoarthritis grades (0-4). The OAI participants were randomly sampled to have demographics similar to the locally recruited participants - details on participant demographics provided in the manuscript. 

# Installation
## Basic notebook - manipulate SSM
The dependencies for the basic notebook `load_and manipulate_statistical_shape_model.ipynb` can be installed using:

 `pip install -r basic_requirements.txt`


## Advanced notebook - score new knees using SSM. 
Another jupyter notebook will be provided to enable scoring new knees using the Principal Components. Please make an issue request if this has not been done and you are looking for it. 

The additional dependencies for scoring new knees using the Principal Componnts of the SSM are: 
- `cycpd`
- `pyfocusr`

As of this writing, these additional libraries must be installed manually by cloning their repositories locally and installing. The instructions for installing `pyfocusr` and `cycpd` are described in the `pyfocusr` repository: https://github.com/gattia/pyfocusr 

For `cycpd`:

`git clone https://github.com/gattia/cycpd`

moving into the directory: 
`cd cycpd`

installing the library: 
`python setup.py install`

For `pyfocusr`:

`git clone https://github.com/gattia/pyfocusr`

moving into the directory: 
`cd pyfocusr`

installing the library: 
`python setup.py install`