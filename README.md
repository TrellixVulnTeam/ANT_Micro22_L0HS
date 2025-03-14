# Artifact Evaluation for ANT [MICRO'22]
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7002115.svg)](https://doi.org/10.5281/zenodo.7002115)

This repository contains the source code for reproducing the experiments in the paper "ANT: Exploiting Adaptive Numerical Data Type for Low-bit Deep Neural Network Quantization" at MICRO'22.

`ant_quantization` contains the ANT framework with PyTorch.

`ant_simulator` contains the performance and energy evaluation of ANT. 

## Project Structure

```
├── ant_quantization                        # The ANT framework with PyTorch.
│   ├── antquant                            # Quantization framework of ANT.
│   ├── BERT
│   │   ├── download_glue_data.py           # Download for GLUE data.
│   │   └── scripts                         # Reproduce the experiment data in Figure 12.
│   ├── ImageNet
│   │   └── scripts                         # Download checkpoints and reproduce the experimental data in Figure 12.
│   ├── quant                               # Quantization CUDA kernel.
│   └── result                              # Our test results.
├── ant_simulator                           # The performance and energy evaluation of ANT.
│   ├── results                             # Our test results.
│   └── run_ant.py                          # The scripts are for reproducing the experiment data in Figure 13.
```

## License
Licensed under an Apache-2.0 license.
