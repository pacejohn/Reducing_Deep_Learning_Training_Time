# Reducing Deep Learning Training Time

In my blog (xxx), I showed how much deep learning training time could be reduced by using enterprise level servers rather than laptops or workstations.  Here, I show the specs of the 2 servers (S1 and S2) and workstation (WS) used in the comparisons.  I also list the actual training times each BERT model for 1 epoch.

Server Specs

| Machine      | CPU                                                    | RAM    | GPU                 |
| -------------|:------------------------------------------------------:| ------:| -------------------:|
| **S1**       | 2x Intel(R) Xeon(R) CPU E5-2698 v4 @ 2.20GHz, 20 cores | 512 GB | 8x Nvidia V100 32GB |
| **S2**       | 2x Intel(R) Xeon(R) Bronze 3106 CPU @ 1.70GHz, 8 cores |  64 GB | 1x Nvidia V100 16GB |
| **WS**       | 1x AMD Ryzen 7 2700X @ 3.70 GHz, 16 cores              |  32 GB | 1x Nvidia Titan RTX |


Model Training Times - Times shown for S1 and S2 are the average of 3 training iterations.  Times shown for WS are from [Thilina Rajapakse's Medium article](https://towardsdatascience.com/to-distil-or-not-to-distil-bert-roberta-and-xlnet-c777ad92f8) (https://towardsdatascience.com/to-distil-or-not-to-distil-bert-roberta-and-xlnet-c777ad92f8)

| Model                                  | Machine  | Training Time for 1 Epoch (min:sec) |
| ---------------------------------------|:--------:|------------------------------------:| 
| **bert-base-cased**                    | S1       | 19:32                               |
|                                        | S2       | 23:16                               |
|                                        | WS       | 22:17                               |
| **roberta-base**                       | S1       | 19:40                               |
|                                        | S2       | 23:23                               |
|                                        | WS       | 29:59                               |
| **distilbert-base-uncased**            | S1       | 10:37                               |
|                                        | S2       | 12:26                               |
|                                        | WS       | 15:34                               |
| **xlnet-base-cased**                   | S1       | 58:17                               |
|                                        | S2       | 64:57                               |
|                                        | WS       | 102:25                              |
| **distilroberta-base**                 | S1       | 11:02                               |
|                                        | S2       | 12:47                               |
|                                        | WS       | 15:59                               |
| **bert-base-multilingual-cased**       | S1       | 20:36                               |
|                                        | S2       | 23:56                               |
|                                        | WS       | 24:38                               |
| **distilbert-base-multilingual-cased** | S1       | 11:46                               |
|                                        | S2       | 13:08                               |
|                                        | WS       | 18:49                               |


