Installing ARIA-tools

This repository provides documentation and guidance for installing and using ARIA-tools, a Python toolkit for working with ARIA/Sentinel-1 geospatial and InSAR products.

Clone the ARIA-tools repository

git clone https://github.com/aria-tools/ARIA-tools.git
cd ARIA-tools


Create the Conda environment

conda env create -f environment.yml
conda activate aria-tools


Install ARIA-tools

python setup.py install


or for editable mode:

pip install -e .


Add ARIA-tools to PATH and PYTHONPATH

Add the following lines to your ~/.bashrc (update the path to your installation directory):

export PYTHONPATH="/path/to/ARIA-tools/tools/ARIAtools:$PYTHONPATH"
export PATH="/path/to/ARIA-tools/tools/bin:$PATH"


Reload your shell:

source ~/.bashrc


Verify the installation

python -c "import ARIAtools; print('ARIA-tools installed successfully')"

