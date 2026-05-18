# A Multimodal Driver behavior Evaluation System: Combining Telematics, VLMs and LLMs

This repository contains the code for my MSc Data Science thesis:

The project combines telematics events, anonymised dashcam clip evidence, Vision Language Model outputs, driver behaviour rankings, and a Large Language Model query layer.

## Notebooks

The notebooks are designed to run in order:

1. `1. Internal Fleet.ipynb`  
   Runs the VLM processing pipeline on raw dashcam clips.

2. `2. Anonymisation.ipynb`  
   Anonymises extracted driver-facing frames.

3. `3. Driver Analysis.ipynb`  
   Runs the driver behaviour ranking and analysis using the processed data.

4. `4. LLM_Query_Layer.ipynb`  
   Runs the LLM query layer using the processed rankings and anonymised clip evidence.

## Important data note

Notebooks 1 and 2 require raw clips or intermediate raw frame outputs. These are not provided publicly.

The public dataset only includes processed and anonymised data. This means:

- Notebook 3 should run from the provided processed outputs.
- Notebook 4 should run from the provided processed outputs and anonymised clips.
- Notebooks 1 and 2 are included for method transparency.

## Data

Large processed and anonymised files are hosted separately on Zenodo:

**Zenodo dataset:** https://zenodo.org/records/20160369

**Zenodo DOI:** https://doi.org/10.5281/zenodo.20160369

## License and citation

Code in this repository is released under the MIT License.

The processed and anonymised dataset is released under the Creative Commons Attribution 4.0 International License (CC BY 4.0), unless stated otherwise on the Zenodo record.

If you use this repository or dataset, please cite the thesis project and Zenodo dataset.

## Disclaimer

This repository is academic research code and a proof of concept. It is not a production driver scoring system.
