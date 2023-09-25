# SimChart9K

<div align=center>
<img src="https://github.com/Uni-Modal/SimChart9K/blob/main/images/SC.png" width="400" height="150">
</div>

<div align="center">
<h1>SimChart9K: An LLMs-based Simulatied Visual Chart Understanding Benchmark<br></h1>
</div>

The proposed simulated dataset consisting of 9,098 charts and associated data annotations in CSV format. 

 We perform data augmentation for chart perception and reasoning by leveraging an LLMs-based self-inspection data production scheme, producing the SimChart9K dataset. Besides, we observe that StructChart continuously improves the chart perception performance as more simulated charts are used for pre-training.

## SimChart9K Dataset Download

a. Register an account from OpenXLab website as follows.
```shell
https://openxlab.org.cn/home
```

b. Install the dependent libraries as follows:

* Install the openxlab dependent libraries.
  ```shell
    pip install openxlab
  ```
* Obtain the Access Key and Secret Key on the OpenXLab website by clicking the button of Account Security
* Login the OpenXLab using the Access Key and Secret Key
  ```shell
    openxlab login
  ```

c. Download the ReSimAD dataset by performing the following command:
```shell
openxlab dataset get --dataset-repo  Lonepic/SimChart9K
```

## t-SNE comparisons with Real Chart Datasets

<p align="center">
  <img src="images/t-SNE_a.PNG" width="62%">
  <div>Feature Distribution using t-SNE of Real Datasets.</div>
</p>


<p align="center">
  <img src="images/t-SNE_b.PNG" width="62%">
  <div>Feature Distribution using t-SNE of both Real Datasets and SimChart9K.</div>
</p>

## Visualization Exapmles

<p align="center">
  <img src="images/multi_task_1.PNG" width="92%">
  <div>Visualization results using the proposed StructChart on different chart-related reasoning tasks including Question Answering (QA), Summarization, and Redrawing.</div>
</p>

<p align="center">
  <img src="images/multi_task_2.PNG" width="92%">
  <div>Visualization results using the proposed StructChart on different chart-related reasoning tasks including Question Answering (QA), Summarization, and Redrawing.</div>
</p>