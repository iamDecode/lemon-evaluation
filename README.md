🍋 LEMON evaluation
=================================

This repository hosts the code to run the evaluation of the LEMON explainer technique.

## Setup

This assumes you have got the python virtualenv package installed (`pip install virtualenv`).

1. Create a virtual environment:

        $ virtualenv venv

2. Activate the virtual environment:

        $ source venv/bin/activate

   Or in the fish shell:

        $ source venv/bin/activate.fish

3. Install the dependencies:

        $ pip install -r requirements.txt

4. Make sure jupyter uses the virtualenv:

	$ python -m ipykernel install --user --name=venv


## Running

To execute the notebook, run:

        $ jupyter lab

You may have to switch the kernel to the one we created in setup step 4.

## Content

- `01-samples` contains code to generate samples using arbitrary distance kernels (the basis of LEMON), and code to generate the figures used in the paper.
- `02-evaluation-synthetic` contains the full code for LEMON and for the synthetic data evaluation in the paper, and 
- `03-evaluation-uci` the code for the UCI dataset evaluation in the paper (this may take a while to run).