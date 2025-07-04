# FZU Hydraulic Gear Pump Fault Dataset (Open-source Dataset Collected by the Laboratory)

##### Update Log: July 3, 2025 – Steady-state multivariable (speed and pressure) operating condition dataset.

&#x20;

We have released a hydraulic gear pump fault dataset, named **FZU_HGPFD**. The data collected in this update corresponds to fault conditions under steady operating states. We hope this dataset will be beneficial to your research.

##### Baidu NetDisk Data:通过网盘分享的文件：FZU_HGPFD
链接: https://pan.baidu.com/s/1DyMRz3kWsMPFO_Prye6i7A?pwd=c84s 提取码: c84s

Please cite the following paper when using this dataset in your publications.

##### 论文链接

## Dataset Introduction

This dataset includes vibration signals from hydraulic gear pumps under six different health conditions across 28 different operating conditions. The dataset is publicly available and can be used by anyone to validate diagnostic algorithms for hydraulic gear pumps.

![](README_md_files/18838bb0-581f-11f0-8868-2bbcb86325e2.jpeg?v=1&type=image)

**Fig. 1** Hydraulic and Mechanical System

![](README_md_files/d43eaad0-589a-11f0-801a-4df8120b4db1.jpeg?v=1&type=image)

**Fig. 2** Data Collection Environment and Sensor Placement

###### *Note: During data collection, NI acquisition system and B&K sound pressure and vibration sensors were used.

#### Gear Pump Description

The gear pump used in this dataset has 10 teeth on both the driving and driven gears, and it is equipped with four roller bearings, each containing 16 rollers.

For this pump, six health conditions were defined: the normal state (HS), three primary fault types — bearing wear (BW), root cut (RC), and gear surface wear (GW) — as well as two compound fault types — gear surface wear combined with root cut (GW_RC) and gear surface wear combined with bearing wear (GW_BW).

![](README_md_files/db273430-5821-11f0-8868-2bbcb86325e2.jpeg?v=1&type=image)

**Fig. 3** Basic Fault Types

#### Sampling Settings

The sampling frequency is 48 kHz, and data is collected for 3 minutes under each operating condition.

The collected data is saved in TDMS format. The first three columns correspond to sound pressure signals 1, 2, and 3, while the last three columns correspond to vibration signals 1, 2, and 3. The sound pressure sensors are arranged on a hemispherical surface 1 meter away from the sound source, in accordance with ISO 4412-1.

#### Operating Condition Settings

A total of 28 typical operating conditions were collected, covering 7 speed levels from 600 rpm to 1200 rpm (in 100 rpm increments) and 4 pressure levels from 2 MPa to 8 MPa (in 2 MPa increments).

This dataset is suitable for evaluating model performance in cross-condition and compound fault diagnosis tasks. Notably, the dataset features multivariable operating conditions, aligning with practical industrial scenarios.

#### File Organization Format

The data is organized using a three-level folder structure. Each data file is named according to the corresponding pressure value of the operating condition, as illustrated below:

* FZU_HGPFD

  * Fault Types

    * Rpm

      * Bar.tdms

## Contact Information

If you have any questions or suggestions, please feel free to contact us at:

huihuang，huihuang@fzu.edu.cn
