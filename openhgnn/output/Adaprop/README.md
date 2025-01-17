# AdapropT[KDD2023]

-   paper: https://arxiv.org/pdf/2205.15319.pdf
-   Code from author: [AdapropT](https://github.com/LARS-research/AdaProp)

This model is divided into two scenarios: inductive and transactional, so we will integrate them into two models: AdaptropT and AdaptropI
## AdapropT
### How to run

- Clone the Openhgnn-DGL

  ```bash
  python main.py -m Adaprop -d Adaprop -t link_prediction -g 0
  ```

  If you do not have gpu, set -gpu -1.

  the dataset AdapropT is supported.

### Performance: Family

-   Device: GPU, **GeForce RTX 2080Ti**
-   Dataset: AdapropT

| transductive |               Family              
|:------------:| :-----------------------------: 
|     MRR      | paper: 0.988    OpenHGNN: 0.9883 
|     H@1      | paper: 98.6    OpenHGNN: 0.9864 
|     H@10     | paper: 99.0    OpenHGNN: 0.9907 







### TrainerFlow: AdapropT_trainer

#### model

- ​	AdapropT 
  - ​		AdapropT is a meta-path based recommendation model, which is based on the idea of meta-path based heterogeneous graph neural network.


  

## AdapropI
### How to run

- Clone the Openhgnn-DGL

  ```bash
  python main.py -m AdapropI -d AdapropI -t link_prediction -g 0
  ```

  If you do not have gpu, set -gpu -1.

  the dataset AdapropI is supported.

 ## Performance: fb15k237_v1

-   Device: GPU, **GeForce RTX 2080Ti**
-   Dataset: AdapropI
- 
| inductive |               fb15k237_v1              
|:---------:| :-----------------------------: 
|    MRR    | paper: 0.310    OpenHGNN: 0.3121 
|    H@1    | paper: 0.191    OpenHGNN: 0.1946 
|   H@10    | paper: 0.551    OpenHGNN: 0.5462






### TrainerFlow: AdapropI_trainer

#### model

- ​	AdapropI 
  - ​		AdapropI is a meta-path based recommendation model, which is based on the idea of meta-path based heterogeneous graph neural network.

#### Contributor

zikai Zhou[GAMMA LAB]

#### If you have any questions,

Submit an issue or email to  460813395@qq.com



