# Open-PAV

Open-PAV (Open Production Automated Vehicle) is an open platform designed to facilitate **data collection, model calibration, and simulation** of production automated vehicle (PAV) behaviors. It integrates diverse datasets and calibrated vehicle models, making it an essential tool for researchers and developers aiming to study PAV dynamics and their impacts. The project encourages contributions from the research community and provides ready-to-use model parameters for seamless integration with simulation tools.

## Key Features

- **Comprehensive Dataset:**
  - A comprehensive trajectory dataset has been compiled by six research teams, including the CATS Lab at UW–Madison, the VECTOR Center at Vanderbilt University, the ITS Lab at Florida Atlantic University, the European Commission’s Joint Research Centre, the UCLA Mobility Lab and Transportation Research Center, Waymo, and Argo AI. This dataset encompasses trajectory data from 14 AV brands and 33 AV models, drawn from 13 open-source AV datasets. All data have been converted into a unified vectorized format to enable efficient access and analysis.  [[Paper]](https://www.nature.com/articles/s41597-024-03795-y) [[Data]](https://github.com/CATS-Lab/Filed-Experiment-Data-ULTra-AV)
  <img src="./docs/images/Dataset.png" alt="Major Components" width="600">
  
- **Kinematic Model Calibration:**
  - Supports linear models, IDM models (for SUMO), Wiedemann-99 (for Vissim), and machine learning-based models.
  - Includes pre-configured model parameters for direct use in traditional simulation software.

- **Simulation Integration:**
  - Enables rapid and accurate simulation of automated vehicle behavior and analysis of their impacts.

- **Community Collaboration:**
  - Designed to foster contributions and collaboration among researchers globally.

## Original Datasets

Thirteen open-source datasets provide diverse insights into AV behavior across various driving conditions and scenarios. These open-source datasets are from six providers:

- **Vanderbilt ACC Dataset**. Collected in Nashville, Tennessee by Vanderbilt University research group. [[Link]](https://acc-dataset.github.io/datasets/) [[Paper]](https://arxiv.org/abs/1911.06454).
  - [Two-vehicle ACC driving, Tennessee 2019](https://github.com/CATS-Lab/Filed-Experiment-Data-AV_Platooning_Data)
- **MircoSimACC Dataset**. Collected in four cities in Florida, including Delray Beach, Loxahatchee, Boca Raton, and Parkland by the Florida Atlantic University research group. [[Link]](https://github.com/microSIM-ACC/ICE) [[Paper]](https://ieeexplore.ieee.org/document/10421910)
  - [ICE](https://github.com/microSIM-ACC/ICE)
- **CATS Open Datasets**. Three datasets were gathered in Tampa, Florida, and Madison, Wisconsin by the CATS Lab. [[Link]](https://github.com/CATS-Lab) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0968090X21001534)
  - [Filed-Experiment-Data-AV_Platooning_Data](https://github.com/CATS-Lab/Filed-Experiment-Data-AV_Platooning_Data)
  - [Filed-Experiment-Data-ACC_Data](https://github.com/CATS-Lab/Filed-Experiment-Data-ACC_Data)
  - [CATS-UWMadison-AV-Data](https://github.com/MarkMaaaaa/CATS-UWMadison-AV-Data)
- **OpenACC Database**. Four datasets were collected across Italy, Sweden, and Hungary by the European Commission's Joint Research Centre. [[Link]](https://data.europa.eu/data/datasets/9702c950-c80f-4d2f-982f-44d06ea0009f?locale=en) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0968090X21000772)
  - [Casale](https://jeodpp.jrc.ec.europa.eu/ftp/jrc-opendata/TransportExpData/JRCDBT0001/LATEST/Casale/)
  - [Vicolungo](https://jeodpp.jrc.ec.europa.eu/ftp/jrc-opendata/TransportExpData/JRCDBT0001/LATEST/Vicolungo/)
  - [AstaZero](https://jeodpp.jrc.ec.europa.eu/ftp/jrc-opendata/TransportExpData/JRCDBT0001/LATEST/AstaZero/)
  - [ZalaZone](https://jeodpp.jrc.ec.europa.eu/ftp/jrc-opendata/TransportExpData/JRCDBT0001/LATEST/ZalaZone/)
- **Central Ohio ACC Datasets**. Two datasets were collated in Ohio by UCLA's Mobility Lab and Transportation Research Center. [[Link]](https://catalog.data.gov/dataset/advanced-driver-assistance-system-adas-equipped-single-vehicle-data-for-central-ohio) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0968090X23001092)
  - [Advanced Driver Assistance System (ADAS)-Equipped Two-Vehicle Data for Central Ohio](https://catalog.data.gov/dataset/advanced-driver-assistance-system-adas-equipped-two-vehicle-data-for-central-ohio)
- **Waymo Open Dataset**. Two datasets were collected in six cities including San Francisco, Mountain View, and Los Angeles in California, Phoenix in Arizona, Detroit in Michigan, and Seattle in Washington by Waymo. [[Paper1]](https://www.sciencedirect.com/science/article/pii/S0968090X21004769)[[Paper2]](https://openaccess.thecvf.com/content/ICCV2021/papers/Ettinger_Large_Scale_Interactive_Motion_Forecasting_for_Autonomous_Driving_The_Waymo_ICCV_2021_paper.pdf)
  - [Waymo Motion Dataset](https://waymo.com/open/data/motion/)
  - [Vehicle trajectory data processed from the Waymo Open Dataset](https://data.mendeley.com/datasets/wfn2c3437n/2)
- **Argoverse 2 Motion Forecasting Dataset** [8]. Collected from Austin in Texas, Detroit in Michigan, Miami in Florida, Pittsburgh in Pennsylvania, Palo Alto in California, and Washington, D.C. by Argo AI with researchers from Carnegie Mellon University and the Georgia Institute of Technology. [[Paper]](https://arxiv.org/abs/2301.00493Thirteen open-source datasets provide diverse insights into AV behavior across various driving conditions and scenarios.)
  - [Argoverse 2 Motion Forecasting Dataset](https://www.argoverse.org/av2.html)


## Major Components

Open-PAV consists of the following components:

- **Data Repository:** A unified storage of diverse datasets (LiDAR, images, videos, trajectories).
- **Model Calibration:** Utilities to calibrate vehicle kinematic models and export them for simulation.
- **Simulation Integration:** Pre-configured packages for SUMO, Vissim, and other platforms.
<!-- **Scenario Manager:** Tools to create and manage simulation scenarios based on real-world data. -->
![Major Components](./docs/images/Workflow.png)

Check the [Open-PAV Documentation](https://markmaaaaa.github.io/OpenPAV) for more details.

## Get Started

### User Guide

- [Overview](https://markmaaaaa.github.io/OpenPAV/)
- [Installation](https://markmaaaaa.github.io/OpenPAV/installation/)
- [Quick Start](https://markmaaaaa.github.io/OpenPAV/quick_start/)
- [Model Calibration](https://markmaaaaa.github.io/OpenPAV/model_calibration/)
- [Simulation Integration](https://markmaaaaa.github.io/OpenPAV/simulation_integration/)
- [Model Download](https://markmaaaaa.github.io/OpenPAV/model_download/)

### Developer Guide

- [API Reference](https://open-pav-documentation.readthedocs.io/en/latest/api.html)
- [Class Design](https://open-pav-documentation.readthedocs.io/en/latest/developer_tutorial.html)
- [Customizing Algorithms](https://open-pav-documentation.readthedocs.io/en/latest/customization.html)

## Contribution Rules

We welcome contributions to Open-PAV! Here’s how you can help:

- Report bugs and suggest improvements by submitting issues.
- Submit contributions via [pull requests](https://github.com/example/Open-PAV/pulls). Please use the provided [pull request template](.github/PR_TEMPLATE.md).

## Citation

If you use Open-PAV in your research or projects, please cite the following:

```bibtex
@article{zhou2024unified,
  title={A unified longitudinal trajectory dataset for automated vehicle},
  author={Zhou, Hang and Ma, Ke and Liang, Shixiao and Li, Xiaopeng and Qu, Xiaobo},
  journal={Scientific Data},
  volume={11},
  number={1},
  pages={1123},
  year={2024},
  publisher={Nature Publishing Group UK London}
}
@article{ma2025automated,
  title={Automated vehicle microscopic energy consumption study (AV-Micro): Data collection and model development},
  author={Ma, Ke and Zhou, Hang and Liang, Zhaohui and Li, Xiaopeng},
  journal={Energy},
  pages={135096},
  year={2025},
  publisher={Elsevier}
}
```

## License

Open-PAV is released under the [MIT License](LICENSE). See the LICENSE file for details.

## Contributors

Open-PAV is developed and maintained by: [CATS Lab](https://catslab.engr.wisc.edu/) Xiaopeng Li ([Homepage](https://catslab.engr.wisc.edu/staff/xiaopengli/))

### Project Lead: [Ke Ma](https://markmaaaaa.github.io/KeMa.github.io/portfolio/))

### Team Members: [Hang Zhou](https://catslab.engr.wisc.edu/staff/zhou-hang/), [Shixiao Liang](https://catslab.engr.wisc.edu/staff/liang-shixiao/), [Keke Long](https://catslab.engr.wisc.edu/staff/long-keke/), [Chengyuan Ma](https://catslab.engr.wisc.edu/staff/ma-chengyuan/)

### Sponsors:

![Sponsors](./docs/images/Sponsors.png)

### External Acknowledgements:

We sincerely appreciate all the dataset providers and contributors for making this work possible. We would like to thank our collaborator Jinbiao Huo for his valuable contributions to this project.
