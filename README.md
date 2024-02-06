
# CLIP4STR: Reproduced and Experimented with Slide Image STR task

This repository is the results reproduction of the re-implementation of [ CLIP4STR: A Simple Baseline for Scene Text Recognition with Pre-trained Vision-Language Model](https://arxiv.org/abs/2305.14014) by [VamosC/CLIP4STR](https://github.com/VamosC/CLIP4STR)


### NOTE: Follow the reproduction guide given by [VamosC](https://github.com/VamosC/CLIP4STR) (Not including them here)
![CLIP4STR architecture](https://github.com/NerdyVisky/CLIP4STR_Reproduced/blob/main/code/clip4str/misc/overall.png?raw=true)



## Reproduction Results
- Log of the CLIP4STR model run on inference mode on a Nvidia GeForce GTX 1080 Ti GPU with 18GB of RAM (2GB for 9CPUs)
- Distribution : Ubuntu 16.2
- Package Manager and Environment : Conda
- Reproduction Results by: <b>Vishvesh Trivedi, Junior Research Fellow, CVIT-IIITH</b>

(dataset) mean (0.48145466, 0.4578275, 0.40821073), std (0.26862954, 0.26130258, 0.27577711)

ArT: 100%|█████████████████████████████████████████████████████████████████████████████████████| 69/69 [05:42<00:00,  4.96s/it]
 
 COCOv1.4: 100%|█████████████████████████████████████████████████████████████████████████████████████| 20/20 [01:31<00:00,  4.56s/it]
   
   CUTE80: 100%|███████████████████████████████████████████████████████████████████████████████████████| 1/1 [00:03<00:00,  3.68s/it]

IC13_1015: 100%|███████████████████████████████████████████████████████████████████████████████████████| 2/2 [00:12<00:00,  6.01s/it]

IC15_1811: 100%|███████████████████████████████████████████████████████████████████████████████████████| 4/4 [00:17<00:00,  4.27s/it]

IC15_2077: 100%|███████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:19<00:00,  3.92s/it]
   
IIIT5k: 100%|███████████████████████████████████████████████████████████████████████████████████████| 6/6 [00:29<00:00,  4.93s/it]
      
SVT: 100%|███████████████████████████████████████████████████████████████████████████████████████| 2/2 [00:06<00:00,  3.41s/it]
     
SVTP: 100%|███████████████████████████████████████████████████████████████████████████████████████| 2/2 [00:06<00:00,  3.39s/it]
     
Uber: 100%|███████████████████████████████████████████████████████████████████████████████████| 158/158 [12:26<00:00,  4.73s/it]
Benchmark (Subset) set:
| Dataset   | # samples | Accuracy | 1 - NED | Confidence | Label Length |
|:---------:|----------:|---------:|--------:|-----------:|-------------:|
| IIIT5k    |      3000 |    99.20 |   99.76 |      97.74 |         5.09 |
| SVT       |       647 |    98.30 |   99.55 |      97.37 |         5.87 |
| IC13_1015 |      1015 |    98.23 |   99.39 |      97.86 |         5.31 |
| IC15_1811 |      1811 |    91.44 |   97.36 |      94.68 |         5.37 |
| IC15_2077 |      2077 |    90.61 |   97.07 |      94.01 |         5.33 |
| SVTP      |       645 |    96.90 |   99.30 |      96.47 |         5.86 |
| CUTE80    |       288 |    99.65 |   99.95 |      97.51 |         5.53 |
|-----------|-----------|----------|---------|------------|--------------|
| Combined  |      9483 |    95.53 |   98.63 |      96.23 |         5.34 |


Benchmark set:
| Dataset   | # samples | Accuracy | 1 - NED | Confidence | Label Length |
|:---------:|----------:|---------:|--------:|-----------:|-------------:|
| IIIT5k    |      3000 |    99.20 |   99.76 |      97.74 |         5.09 |
| SVT       |       647 |    98.30 |   99.55 |      97.37 |         5.87 |
| IC13_1015 |      1015 |    98.23 |   99.39 |      97.86 |         5.31 |
| IC15_1811 |      1811 |    91.44 |   97.36 |      94.68 |         5.37 |
| IC15_2077 |      2077 |    90.61 |   97.07 |      94.01 |         5.33 |
| SVTP      |       645 |    96.90 |   99.30 |      96.47 |         5.86 |
| CUTE80    |       288 |    99.65 |   99.95 |      97.51 |         5.53 |
|-----------|-----------|----------|---------|------------|--------------|
| Combined  |      9483 |    95.53 |   98.63 |      96.23 |         5.34 |


New set:
| Dataset  | # samples | Accuracy | 1 - NED | Confidence | Label Length |
|:--------:|----------:|---------:|--------:|-----------:|-------------:|
| ArT      |     35149 |    85.74 |   95.31 |      93.21 |         5.41 |
| COCOv1.4 |      9825 |    80.80 |   93.56 |      87.93 |         5.91 |
| Uber     |     80551 |    86.70 |   94.21 |      89.59 |         5.34 |
|----------|-----------|----------|---------|------------|--------------|
| Combined |    125525 |    85.97 |   94.47 |      90.48 |         5.40 |


Time: Total 1278.078631401062s, Average 9.466688132562973ms. Total samples 135008.

## Results with Slide Image STR task
(Experimentation underway)

## Acknowledgements
This repository experiments with exisiting works on [CLIP4STR](https://github.com/VamosC/CLIP4STR), [CLIP](https://github.com/openai/CLIP), [OpenCLIP](https://github.com/mlfoundations/open_clip), [PARSeq](https://github.com/baudm/parseq), among others.
