# Dynamic Pacing for Real-time Satellite Traffic

This repository contains the official artifacts and instructions to reproduce the experiments in our paper, "Dynamic Pacing for Real-time Satellite Traffic."

Our work integrates imitation learning with network pacing to stabilize video calls over LEO satellite networks. Reproducing our results relies on network emulation and is best performed using our **CloudLab** profile.

## Project Status & Reproducibility

**Repository Status: Archived**: This project is now archived. Please be aware that this repository is provided as a research artifact to accompany our paper. While the repository will remain public, please note that support is not available, and issues or pull requests may not be reviewed.

**A Note on Stochasticity**: Due to the inherent stochasticity in the emulated constellations, you can expect minor variations in the results on each run. For the most consistent results, we recommend averaging metrics over a few hundred videoconferencing calls.

## Getting Started: How to Reproduce

The most reliable way to run our experiments is with the provided CloudLab profile, which handles all dependencies and configuration.

1.  **Access the Profile**: Navigate to our profile page on CloudLab.
    > **☁️ [Dynamic Pacing Experiment Profile](https://www.cloudlab.us/p/c691f036f0356409824c168ed4b1f9034a7ab9c7)**
2.  **Start the Experiment**: Click "Instantiate" on the profile page. You must select the **Emulab cluster** due to hardware dependencies. The profile will automatically set up part of the environment on the requested nodes.
3.  **Run the Code**: Once the experiment is active, you can log in to the nodes. The core implementation code will be pre-loaded, and you can follow the instructions in that profile's README to configure the environment and run the evaluation scripts.

## Repository Links

  * **📘 Paper**: [Link to paper](https://arxiv.org/pdf/2507.09798)
  * **💻 Core Implementation**: The project is composed of two main repositories: [AlphaRTC](https://github.com/agottipati9/AlphaRTC/tree/starry_net_offline_queue) for the real-time communication framework and [StarryNet](https://github.com/agottipati9/StarryNet) for the satellite network emulation. The linked repositories contain the primary source code and evaluation scripts. *This is included automatically in the CloudLab profile.*
  * **☁️ CloudLab Profile**: [Link to CloudLab profile](https://www.cloudlab.us/p/c691f036f0356409824c168ed4b1f9034a7ab9c7)- The configuration files for automatically deploying the experiment environment.

## Environment Requirements

The CloudLab profile automatically configures this environment. The key technologies are:

  * **OS**: Ubuntu 22.04
  * **Core**: Python 3.10, PyTorch 2.x, AlphaRTC
  * **Emulator**: StarryNet

## Citation

If you use this work in your research, please cite our paper:

```bibtex
@article{gottipati2025towards,
  title={Dynamic Pacing for Real-time Satellite Traffic},
  author={Gottipati, Aashish and Qiu, Lili},
  journal={arXiv preprint arXiv:2507.09798},
  year={2025}
}
```
