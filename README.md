# RoboDrive Toolkit
[![Twitter](https://badgen.net/badge/icon/twitter?icon=twitter&label)](https://twitter.com/RoboDrive2024)
[![website](https://img.shields.io/badge/website-%F0%9F%94%97-lightblue)](https://robodrive-24.github.io/)
[![slack](https://img.shields.io/badge/slack-%F0%9F%94%97-blue)](https://join.slack.com/t/robodrive/shared_invite/zt-29fnp2iye-QZtwxSdCchil6noIiTxoXg)
[![wechat](https://img.shields.io/badge/wechat-%F0%9F%94%97-lightblue)](https://robodrive-24.github.io/wechat_qr.jpg)
<img src="https://visitor-badge.laobi.icu/badge?page_id=robodrive-24.toolkit&left_color=gray&right_color=blue">
[![ICRA2024](https://img.shields.io/badge/icra2024-&#129302;-lightblue)](https://2024.ieee-icra.org/)

<p align="center">
  <img src="docs/figs/cover.png" align="center" width="100%">
</p>

Welcome to [The RoboDrive Challenge](https://robodrive-24.github.io/)! :wave:


## :oncoming_automobile: About
> `RoboDrive` is one of the first competitions that targeted probing the Out-of-Distribution (OoD) robustness of state-of-the-art autonomous driving perception models, centered around two mainstream topics: **common corruptions** and **sensor failures**.

> There are eighteen real-world corruption types in total, ranging from three perspectives:
>  - Weather and lighting conditions, such as bright, low-light, foggy, and snowy conditions.
>  - Movement and acquisition failures, such as potential blurs caused by vehicle motions.
>  - Data processing issues, such as noises and quantizations happen due to hardware malfunctions.

> Additionally, we aim to probe the 3D scene perception robustness under camera and LiDAR sensor failures:
>  - Loss of certain camera frames during the driving system sensing process.
>  - Loss of one or more camera views during the driving system sensing process.
>  - Loss of the roof-top LiDAR view during the driving system sensing process.

> Kindly visit our [webpage](https://robodrive-24.github.io/) to explore more details and instructions of this challenge. :blue_car:

## :rainbow: Venue

> This competition is affiliated with the 41st IEEE Conference on Robotics and Automation ([ICRA 2024](https://2024.ieee-icra.org/)).

><img src="https://robodrive-24.github.io/icra2024.png" width="19%"/><br/>
> ICRA is the IEEE Robotics and Automation Society's flagship conference. ICRA 2024 will be held from May 13th to 17th, 2024, in Yokohama, Japan.



# Outline
- [Useful Info](#information_source-useful-info)
- [Timeline](#clock1-timeline)
- [Challenge Tracks](#blue_car-challenge-tracks)
- [Data Preparation](#hotsprings-data-preparation)
- [Getting Started](#rocket-getting-started)
- [Changelog](#memo-changelog)
- [Awards](#1st_place_medal-awards)
- [License](#license)
- [Sponsor](#heart-sponsor)
- [Citation](#citation)
- [Terms & Conditions](#balance_scale-terms--conditions)
- [Frequently Asked Questions](#thinking-frequently-asked-questions)
- [Organizers](#organizers)
- [Affiliation](#affiliation)
- [Acknowledgements](#ok_man-acknowledgements)


## :information_source: Useful Info
| \# | Item | Link |
|:-:|:-|:-|
| :globe_with_meridians: | Competition Webpage | https://robodrive-24.github.io |
| :wrench: | Competition Toolkit | https://github.com/robodrive-24/toolkit |
| :octocat: | Official GitHub Account | https://github.com/robodrive-24 |
| :mailbox: | Contact | robodrive.2024@gmail.com |


## :clock1: Timeline
> **Note:** All timestamps are in the `AoE` (Anywhere on Earth) format.
- `Dec 25 '23` - Team Up; Register for your team by filling in [this](https://forms.gle/hnaezVhEycPAjUD78) Google Form. 
- `Jan 05 '24` - Release of training and evaluation data.
- `Jan 15 '24` - Competition servers online @ [CodaLab](https://codalab.lisn.upsaclay.fr/).
- `Mar 31 '24` - Phase `One` deadline.
- `Apr 30 '24` - Phase `Two` deadline.
- `May 17 '24` - Award decision announcement @ [ICRA 2024](https://2024.ieee-icra.org/).


## :blue_car: Challenge Tracks
There are **five** tracks in this `RoboDrive` challenge, with emphasis on the following 3D scene perception tasks:

| \# | Task | Description | Doc | Server |
|:-:|:-|:-|:-:|:-:|
| Track `1` | Robust BEV Detection | Evaluating the resilience of detection algorithms against diverse environmental and sensor-based corruptions | [`[Link]`](https://github.com/robodrive-24/toolkit/blob/main/track-1/README.md) | [`[Link]`](https://codalab.lisn.upsaclay.fr/competitions/17135) |
| Track `2` | Robust Map Segmentation | Focusing on the segmentation of complex driving scene elements in BEV maps under varied driving conditions | [`[Link]`](https://github.com/robodrive-24/toolkit/blob/main/track-2/README.md) | [`[Link]`](https://codalab.lisn.upsaclay.fr/competitions/17062) |
| Track `3` | Robust Occupancy Prediction | Testing the accuracy of occupancy grid predictions in dynamic and unpredictable real-world driving environments | [`[Link]`](https://github.com/robodrive-24/toolkit/blob/main/track-3/README.md) | [`[Link]`](https://codalab.lisn.upsaclay.fr/competitions/17063) |
| Track `4` | Robust Depth Estimation | Assessing the depth estimation robustness from multiple perspectives for comprehensive 3D scene perception | [`[Link]`](https://github.com/robodrive-24/toolkit/blob/main/track-4/README.md) | [`[Link]`](https://codalab.lisn.upsaclay.fr/competitions/17226) |
| Track `5` | Robust Multi-Modal BEV Detection | Tailored for evaluating the reliability of advanced driving perception systems equipped with multiple types of sensors | [`[Link]`](https://github.com/robodrive-24/toolkit/blob/main/track-5/README.md) | [`[Link]`](https://codalab.lisn.upsaclay.fr/competitions/17137) |

Our evaluation servers were developed based on the [CodaLab](https://codalab.lisn.upsaclay.fr/) platform. :ok_man:

><img src="docs/figs/codalab-logo.png" width="30%"/><br/>
> CodaLab is an open-source web-based platform that enables researchers, developers, and data scientists to collaborate, with the goal of advancing research fields where machine learning and advanced computation are used.


## :hotsprings: Data Preparation
Kindly refer to [DATA_PREPARE.md](docs/DATA_PREPARE.md) for the details to prepare the training and evaluation data.


## :rocket: Getting Started
Kindly refer to [GET_STARTED.md](docs/GET_STARTED.md) to learn more usage of this toolkit.


## :memo: Changelog

- `Jan 22 '24` - The evaluation server of Track `4` is online. [`[Server4]`](https://codalab.lisn.upsaclay.fr/competitions/17226)
- `Jan 15 '24` - The evaluation server of Track `5` is online. [`[Server5]`](https://codalab.lisn.upsaclay.fr/competitions/17137)
- `Jan 15 '24` - The evaluation server of Track `3` is online. [`[Server3]`](https://codalab.lisn.upsaclay.fr/competitions/17063)
- `Jan 15 '24` - The evaluation server of Track `2` is online. [`[Server2]`](https://codalab.lisn.upsaclay.fr/competitions/17062)
- `Jan 15 '24` - The evaluation server of Track `1` is online. [`[Server1]`](https://codalab.lisn.upsaclay.fr/competitions/17135)
- `Jan 12 '24` - Instructions, baseline models, and results of Track `5` have been released.
- `Jan 12 '24` - Training and evaluation data of Track `5` have been released.
- `Jan 08 '24` - A list of Frequently Asked Questions ([FAQs](https://github.com/robodrive-24/toolkit/blob/main/docs/GET_STARTED.md#frequently-asked-questions)) has been summarized for better clarity.
- `Jan 06 '24` - Instructions, baseline models, and results of Tracks `1` to `3` have been released.
- `Jan 05 '24` - Training and evaluation data of Tracks `1` to `4` have been released.
- `Dec 25 '23` - Register for your team by filling in [this](https://forms.gle/hnaezVhEycPAjUD78) Google Form.
- `Dec 01 '23` - Launch of [The RoboDrive Challenge](https://robodrive-24.github.io/) at [ICRA 2024](https://2024.ieee-icra.org/). More info coming soon!


## :1st_place_medal: Awards
The top-performing participants of this competition are honored with **cash awards** and **certificates**.

| Award | Amount | Honor | 
| :- | :- | :- | 
| :1st_place_medal: 1st Place | Cash Award $ 5000 | Official Certificate |
| :2nd_place_medal: 2nd Place | Cash Award $ 3000 | Official Certificate |
| :3rd_place_medal: 3rd Place | Cash Award $ 2000 | Official Certificate |

> **Note:** The cash awards are donated by our sponsors and are **shared** among five tracks. We reserve the right to examine the validity of each submission. For more information, kindly refer to the [Terms & Conditions](#balance_scale-terms--conditions) section.

Additionally, we provide the following awards for participants that meet certain conditions.

| Award | Honor | Condition |
| :- | :- | :- | 
| Innovative Award | Official Certificate | Solutions with excellent novelty |
| Certificate of Participation | Official Certificate | Teams with submission records in both phases |


## License
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/80x15.png" /></a>
<br />
This competition is under the <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.


## :heart: Sponsor
This competition is supported by [HUAWEI Noah's Ark Lab](https://www.noahlab.com.hk/#/home).
><img src="docs/figs/logo_sponsor.png" width="35%"/><br/>
> The Noah’s Ark Lab is the AI research center for Huawei Technologies, aiming to make significant contributions to both the company and society by innovating in artificial intelligence, data mining, and related fields.




## Citation
If you find this competition helpful for your research, kindly consider citing our papers:

```bibtex
@article{xie2023robobev,
    title = {RoboBEV: Towards Robust Bird's Eye View Perception under Corruptions},
    author = {Shaoyuan Xie and Lingdong Kong and Wenwei Zhang and Jiawei Ren and Liang Pan and Kai Chen and Ziwei Liu},
    journal = {arXiv preprint arXiv:2304.06719}, 
    year = {2023}
}
```

```bibtex
@inproceedings{kong2023robodepth,
    title = {RoboDepth: Robust Out-of-Distribution Depth Estimation under Corruptions},
    author = {Lingdong Kong and Shaoyuan Xie and Hanjiang Hu and Lai Xing Ng and Benoit R. Cottereau and Wei Tsang Ooi},
    booktitle = {Advances in Neural Information Processing Systems (NeurIPS)},
    year = {2023},
}
```

```bibtex
@inproceedings{kong2023robo3d,
    title = {Robo3D: Towards Robust and Reliable 3D Perception against Corruptions},
    author = {Lingdong Kong and Youquan Liu and Xin Li and Runnan Chen and Wenwei Zhang and Jiawei Ren and Liang Pan and Kai Chen and Ziwei Liu},
    booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
    pages = {19994-20006},
    year = {2023},
}
```
```bibtex
@misc{mmdet3d,
    title = {MMDetection3D: OpenMMLab Next-Generation Platform for General 3D Object Detection},
    author = {MMDetection3D Contributors},
    howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}},
    year = {2020}
}
```

In the meantime, kindly cite the technical reports of the [nuScenes](https://www.nuscenes.org/nuscenes) dataset and the [CodaLab](https://codalab.lisn.upsaclay.fr/) platform:
```bibtex
@inproceedings{caesar2020nuscenes,
    title={nuScenes: A Multimodal Dataset for Autonomous Driving},
    author={Holger Caesar and Varun Bankiti and Alex H. Lang and Sourabh Vora and Venice Erin Liong and Qiang Xu and Anush Krishnan and Yu Pan and Giancarlo Baldan and Oscar Beijbom},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    pages = {11621-11631},
    year={2020}
}
```

```bibtex
@article{pavao2023codalab,
    title = {CodaLab Competitions: An Open Source Platform to Organize Scientific Challenges},
    author = {Adrien Pavão and Isabelle Guyon and Anne-Catherine Letournel and Dinh-Tuan Tran and Xavier Baró and Hugo Jair Escalante and Sergio Escalera and Tyler Thomas and Zhen Xu},
    journal = {Journal of Machine Learning Research (JMLR)},
    pages = {1-6},
    year = {2023}
}
```




## :balance_scale: Terms & Conditions
This competition is made freely available to academic and non-academic entities for non-commercial purposes such as academic research, teaching, scientific publications, or personal experimentation. Permission is granted to use the data given that you agree:
1. That the data in this competition comes “AS IS”, without express or implied warranty. Although every effort has been made to ensure accuracy, we do not accept any responsibility for errors or omissions.
2. That you may not use the data in this competition or any derivative work for commercial purposes such as, for example, licensing or selling the data, or using the data with a purpose of procuring a commercial gain.
3. That you include a reference to RoboDrive (including the benchmark data and the specially generated data for academic challenges) in any work that makes use of the benchmark. For research papers, please cite our preferred publications as listed on our webpage.

To ensure a fair comparison among all participants, we require:
1. All participants must follow the exact same data configuration when training and evaluating their algorithms. Please do not use any public or private datasets other than those specified for model training.
2. The theme of this competition is to probe the out-of-distribution robustness of autonomous driving perception models. Therefore, any use of the corruption and sensor failure types designed in this benchmark is strictly prohibited, including any atomic operation that comprises any one of the mentioned corruptions.
3. To ensure the above two rules are followed, each participant is requested to submit the code with reproducible results before the final result is announced; the code is for examination purposes only and we will manually verify the training and evaluation of each participant's model.


## :thinking: Frequently Asked Questions

| | |
|:-:|:-|
| :thinking: | **Q1:** ***"How can I register a valid team for this competition?"*** |
| :blue_car: | **A1:**  To register a team, kindly fill in [this](https://forms.gle/hnaezVhEycPAjUD78) Google Form. The registration period is from `now` till the deadline of phase one, i.e., `Mar 31 '24`. |
|  |
|  |
| :thinking: | **Q2:** ***"Are there any restrictions for the registration? For example, the number of team members."*** |
| :blue_car: | **A2:**  Each team leader should make a **valid** registration for his/her team. Each participant can only be registered by **one** team. There is no restriction on the number of team members in a team.
|  |
|  |
| :thinking: | **Q3:** ***"Whether team members can be changed during the competition?"*** |
| :blue_car: | **A3:**  No. You **CANNOT** change the list of team members after the registration. You must register again as a **new** team if you need to add or remove any members of your team. |
|  |
|  |
| :thinking: | **Q4:** ***"How many tracks can I participate in?"*** |
| :blue_car: | **A4:**  Each team can participate in **at most two tracks** in this competition. |
|  |
|  |
| :thinking: | **Q5:** ***"What can I expect from this competition?"*** |
| :blue_car: | **A5:**  We provide the winning teams from each track with **cash awards** :moneybag: and **certificates** :1st_place_medal:. The winning solutions will be summarized as a **technical report** :book:. An example of last year's technical report can be found [here](https://arxiv.org/abs/2307.15061).
|  |
|  |
| :thinking: | **Q6:** ***“Can I use additional data resources for model training?"*** |
| :blue_car: | **A6:**  No. All participants must follow the **SAME** data preparation procedures as listed in [DATA_PREPARE.md](https://github.com/robodrive-24/toolkit/blob/main/docs/DATA_PREPARE.md). Additional data sources are **NOT** allowed in this competition.
|  |
|  |
| :thinking: | **Q7:** ***"Can I use corruption augmentations during model training?"*** |
| :blue_car: | **A7:**  **For Track 1-4**: No. The theme of this competition is to probe the **out-of-distribution robustness** of autonomous driving perception models. Therefore, all participants must **REFRAIN** from using any corruption simulations as data augmentations during the model training, including any atomic operation that comprises any one of the corruptions in this competition. **For Track 5**, there is no limitation on the augmentations.
|  |
|  |
| :thinking: | **Q8:** ***"How should I configurate the model training? Are there any restrictions on model size, image size, loss function, optimizer, number of epochs, and so on?"***
| :blue_car: | **A8:**  We provide one **baseline model** for each track in [GET_STARTED.md](https://github.com/robodrive-24/toolkit/blob/main/docs/GET_STARTED.md). The participants are recommended to refer to these baselines as the starting point in configuring the model training. There is no restriction on normal model training configurations, including model size, image size, loss function, optimizer, and number of epochs. 
|  |
|  |
| :thinking: | **Q9:** ***"Can I use LiDAR data for Tracks `1` to `4`?"*** |
| :blue_car: | **A9:**  Only **RAW LiDAR points** data is allowed for Tracks `1` to `4` in **training** (e.g., generate sparse depth map). During **inference**, Tracks `1` to `4` are **single-modality** tracks that only involve the use of camera data. The goal of these tracks is to probe the robustness of perception models under camera-related corruptions. Participants who are interested in **multi-modal robustness** (camera + LiDAR) can refer to Track `5` in this competition.
|  |
|  |
| :thinking: | **Q10:** ***"Is it permissible to use self-supervised model pre-training (such as MoCo and MAE)?"*** |
| :blue_car: | **A10:**  Yes. The use of **self-supervised** pre-trained models is possible. Such models may include [MoCo](https://arxiv.org/abs/1911.05722), [MoCo v2](https://arxiv.org/abs/2003.04297), [MAE](https://arxiv.org/abs/2111.06377), [DINO](https://github.com/facebookresearch/dino), and many others. Please make sure to acknowledge (in your code and report) if you use any pre-trained models.
|  |
|  |
| :thinking: | **Q11:** ***"Can I use large models (such as SAM) to generate pre-training or auxiliary annotations?"*** |
| :blue_car: | **A11:**  No. The use of large foundation models, such as [CLIP](https://github.com/openai/CLIP), [SAM](https://segment-anything.com/), [SEEM](https://github.com/UX-Decoder/Segment-Everything-Everywhere-All-At-Once), and any other similar models, is **NOT** allowed in this competition. This is to ensure a relatively fair comparing environment among different teams. Any violations of this rule will be regarded as **cheating** and the results will be canceled.
|  |
|  |
| :thinking: | **Q12:** ***"Are there any restrictions on the use of pre-trained weights (such as DD3D, ImageNet, COCO, ADE20K, Object365, and so on)?"*** |
| :blue_car: | **A12:**  Following the most recent BEV perception works, it is possible to use pre-trained weights on **DD3D**, **ImageNet**, and **COCO**. The use of weights pre-trained on other datasets is **NOT** allowed in this competition.
|  |
|  |
| :thinking: | **Q13:** ***"Can I combine the training and validation sets for model training?"*** |
| :blue_car: | **A13:**  It is strictly **NOT** allowed to use the validation data for model training. All participants **MUST** follow the nuScenes official `train` split during model training and **REFRAIN** from involving any samples from the validation set. Any violations of this rule will be regarded as **cheating** and the results will be canceled.
|  |
|  |
| :thinking: | **Q14:** ***"Can I use model ensembling and test-time augmentation (TTA)?"*** |
| :blue_car: | **A14:**  Like many other academic competitions, it is possible to use **model ensembling** and **test-time augmentation (TTA)** to enhance the model when preparing the submissions. The participants **SHOULD** include necessary details for the use of model ensembling and TTA in their code and reports.
|  |
|  |
| :thinking: | **Q15:** ***"How many times can I make submissions to the server?"*** |
| :blue_car: | **A15:**  For phase one (Jan. - Mar.), a team can submit up to **3** times per day and **99** times total. For phase two (Apr.), a team can submit up to **2** times per day and **49** times total. One team is affiliated with one CodaLab account only. Please **REFRAIN** from having multiple accounts for the same team.
|  |
|  |
| :thinking: | **Q16:** ***" Can I use pretrained denoising or deblurring models during inference?"*** |
| :blue_car: | **A16:**  No. The goal of the competition is to develop a more robust perception model and using pre-trained denoising models is out of the scope of this competition.
|  |
|  |
| :thinking: | **Q17:** ***" Can I use augmentation other than the corruption methods used in the competition?"*** |
| :blue_car: | **A17:**  Similar to Q7, you can use data augmentation methods that do **NOT** include the corruption simulation algorithms used in the competition. More details of the used corruptions can be found from [this](https://ldkong.com/PDF/2023_robobev.pdf) technical report.
|  |
|  |
| :thinking: | **Q18:** ***" What is the sensor corruptions in Track-5?"*** |
| :blue_car: | **A18:**  For the camera sensor, we use camera corruptions by setting all the pixels to 0. For the LiDAR sensor, we use random points drop, drop points within certain view field angles, and beam drop.
|  |
|  |
| :thinking: | **Q19:** ***" What is the depth estimation metric for Track 4?"*** |
| :blue_car: | **A19:**  We use **RELATIVE** depth estimation, not absolute depth estimation for evaluation.
|  |
|  |
| :thinking: | ... |
| :blue_car: | ... |

### Contact
:mailbox: Didn't find a related FAQ to your questions? Let us know (robodrive.2024@gmail.com)!


## Organizers

<p align="center">
  <img src="docs/figs/organizer.png" align="center" width="100%">
</p>

## Affiliation

<p align="center">
  <img src="docs/figs/affiliation.png" align="center" width="100%">
</p>


## :ok_man: Acknowledgements
This competition is developed based on the [RoboBEV](https://github.com/Daniel-xsy/RoboBEV), [RoboDepth](https://github.com/ldkong1205/RoboDepth), and [Robo3D](https://github.com/ldkong1205/Robo3D) projects.

This competition toolkit is developed based on the [MMDetection3D](https://github.com/open-mmlab/mmdetection3d) codebase.

><img src="https://github.com/open-mmlab/mmdetection3d/blob/main/resources/mmdet3d-logo.png" width="30%"/><br/>
> MMDetection3D is an open-source toolbox based on PyTorch, towards the next-generation platform for general 3D perception. It is a part of the OpenMMLab project developed by MMLab.

The evaluation sets of this competition are constructed based on the [nuScenes](https://www.nuscenes.org/nuscenes) dataset from [Motional AD LLC](https://motional.com/).

Part of the content of this toolkit is adopted from [The RoboDepth Challenge](https://robodepth.github.io/) @ [ICRA 2023](https://www.icra2023.org/).
