# Reducing Deep Learning Training Time

In my blog (xxx), I showed how much deep learning training time could be reduced by using enterprise level servers rather than laptops or workstations.  Here, I show the specs of the 2 servers (S1 and S2) and workstation (WS) used in the comparisons.  I also list the actual training times each BERT model for 1 epoch.

Server Specs

| Machine  | CPU                                                    | RAM    | GPU                 |
| ---------|:------------------------------------------------------:| ------:| -------------------:|
| S1       | 2x Intel(R) Xeon(R) CPU E5-2698 v4 @ 2.20GHz, 20 cores | 512 GB | 8x Nvidia V100 32GB |
| S2       | 2x Intel(R) Xeon(R) Bronze 3106 CPU @ 1.70GHz, 8 cores |  64 GB | 1x Nvidia V100 16GB |
| WS       | 1x AMD Ryzen 7 2700X @ 3.70 GHz, 16 cores              |  32 GB | 1x Nvidia Titan RTX |


Model Training Times

| Model                              | Machine  | Training Time for 1 Epoch (min:sec)           |
| -----------------------------------|:--------:|----------------------------------------------:| 
| bert-base-cased                    | S1       | |
|                                    | S2       | |
|                                    | WS       | |
| roberta-base                       | S1       | |
|                                    | S2       | |
|                                    | WS       | |
| distilbert-base-uncased            | S1       | |
|                                    | S2       | |
|                                    | WS       | |
| xlnet-base-cased                   | S1       | |
|                                    | S2       | |
|                                    | WS       | |
| distilroberta-base                 | S1       | |
|                                    | S2       | |
|                                    | WS       | |
| bert-base-multilingual-cased       | S1       | |
|                                    | S2       | |
|                                    | WS       | |
| distilbert-base-multilingual-cased | S1       | |
|                                    | S2       | |
|                                    | WS       | |


