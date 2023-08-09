# Quantitative Image Analysis
## Overview
This Jupyter Notebook is a complete image analysis workflow. It includes optimization steps for common image analysis tasks:
* Grayscale conversion
* Noise removal
* Edge/object detection with thresholding and contours

This notebook also addresses some challenges relevant to biological data:
* RGB image decomposition to address fluorescence bleed-through
* Dynamic ROI creation and heirarchical masking to isolate biologically relevant regions that cannot be identified with standard image analysis methods
* Background subtraction
* Comparing different methods of data collection and analysis

A streamlined Jupyter notebook for statistical analysis is also included. 

This is still developing project; if you have any questions or suggestions, please reach out!

## Dependencies
This notebook works with the following module versions. More recent versions may work, and will be updated as they are tested. Be sure to use the indicated versions of Matplotlib, as Roipoly is not compatible with version 3.7.0. Modules were install with Anaconda unless otherwise indicated.

    Python==3.9.16 # Includes itertools, math, os, shutil, and sys modules
    glob2==0.7
    matplotlib==3.5.1
    matplotlib-inline==0.1.6
    numpy==1.23.5 
    opencv-contrib-python==4.6.0.66 # pip install
    pandas==1.5.3
    regex==2022.7.9
    roipoly==0.5.4 # pip install
    scikit-image==0.19.3
    scipy==1.10.0
    seaborn==0.12.2
    statannotations==0.4.4 # pip install

## Planned Improvements
* Create an Embryo class object to store and call up all relevant information and associated images for each embryo or subject
* Tie the initial steps to a .db file to limit processing time for repeated runs
* Improve compatibility with TIFF images
* Adjust code to collect image metadata


## Citation
If you use or adapt this notebook for your research please cite:

"An Open-Source Image Analysis Method for Quantifying Reporter Fluorescence"

Ball, KF, Perez, JA, Cooper, AM, Pira, CU, Oberg, KC, Wilson, CG.

Frontiers in Imaging -Coding (in review)

## License
    Quantitative Image Analysis 
    Copyright (C) 2023  Kate Ball

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <https://www.gnu.org/licenses/>.
