# MASF

Since there are more and more speech-related applications and various noises exist in real life, speech enhancement plays an important role. However, speech enhancement (SE) systems, based on generative adversarial networks (GANs), are limited in improving speech quality and intelligibility. In this study, we propose a novel multiple self-attention field method for speech enhancement (MSAF). The models with different positions of the self-attention layers focus on different features. Considering the effect of the position of the self-attention layers on SE performance, SASEGANs with self-attention layers at different positions are fused. The output of each model is assigned a different feature weight, which is obtained by training. Then, we fuse the models according to the feature weights to obtain a clean speech signal. For speech quality, the proposed method improves by 8.22%, 8.52%, 9.28%, and 9.40% in CBAK, CSIG, COVL, and PESQ on average compared with the baseline SASEGANs. As to SSNR and STOI, compared with the baseline SASEGANs on average, the proposed method obtains absolute gains of 1.71 and 0.77, respectively. The results show that the MSAF comprehensively improves the performance of the baseline SASEGAN and performs better than the mainstream GAN-based SE methods. Importantly, the proposed method can be extended to other GAN-based SE methods.

---
**All utterances are partially or completely unseen during training, and the results are uncurated (NOT cherry-picked) unless otherwise specified**.

#### MMF-SASEGAN Audio Samples
##### The audio loading may be slower and you need to wait patiently. If you cannot load audio, please contact us to provide original audio files. Our mail address is 20214239031@stu.suda.edu.cn.

|              | Sample 1  | Sample 2  |
|:------------:|:-------:|:-------:|
|       **Noisy**    |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/N_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/N_2.wav"></source> </audio>  |
|      **Clean**     |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/C_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/C_2.wav"></source> </audio>  |
|    **SASEGAN-3**   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/2_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/2_2.wav"></source> </audio>  |
|    **SASEGAN-4**    |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/3_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/3_2.wav"></source> </audio>  |
|   **SASEGAN-5**   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/4_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/4_2.wav"></source> </audio>  |
|    **SASEGAN-6**   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/5_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/5_2.wav"></source> </audio>  |
|    **SASEGAN-7**    |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/6_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/6_2.wav"></source> </audio>  |
|    **SASEGAN-8**    |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/7_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/7_2.wav"></source> </audio>  |
|    **SASEGAN-9**    |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/8_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/8_2.wav"></source> </audio>  |
|    **SASEGAN-10**    |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/9_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/9_2.wav"></source> </audio>  |
|    **SASEGAN-11**    |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/10_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/10_2.wav"></source> </audio>  |
|       **MASF**       |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/M_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/M_2.wav"></source> </audio>  |

#### Ablation study
##### In this study, we also investigate the performance of the speech enhancement system when only two models are fused.The specific experimental results are as follows：

|              | **PESQ**| **CSIG**|**CBAK** |**COVL** | **SSNR**|**STOI(%)** |
|:------------:|:-------:|:-------:|:-------:|:-------:|:-------:|:-------:|
|    **SASEGAN-3**   |   2.32    | 3.51    |  3.07   |   2.90    |  8.53   |  93.35   |
|    **SASEGAN-4**   |   2.36    | 3.57    |  3.08   |   2.95  |  8.38   |  93.47   |
|    **SASEGAN-5**   |   2.31    | 3.46    |  2.94	 |  2.85   |  7.20   |  93.22   |
|    **SASEGAN-6**   |   2.38	   | 3.46	   | 3.12	| 2.90	| 8.86 |	93.39    |
|    **SASEGAN-7**   |   2.30	| 3.52	| 2.98	| 2.89	| 7.34	| 93.38    |
|    **SASEGAN-8**   |   2.34	| 3.55	| 3.03	| 2.92	| 8.03	| 93.24    |
|    **SASEGAN-9**   |   2.29	| 3.45	| 3.05	| 2.85	| 8.48	| 93.28    |
|    **SASEGAN-10**   |  2.41	| 3.62	| 3.06	| 2.99	| 7.87	| 93.36    |
|    **SASEGAN-11**   |  2.35	| 3.57	| 3.03	| 2.94	| 7.76	| 93.19    |
|    **Field 3 add 4**   |   2.54   |  3.79   |  3.24   |  3.16   |  9.12   |   93.60  |
|    **Field 3 add 5**   |   2.56   |  3.81   |  3.25   |  3.17   |  9.28   |   93.77  |
|    **Field 3 add 6**   |   2.53   |  3.83   |  3.17   |  3.17   |  8.25   |   93.78  |
|    **Field 3 add 7**   |   2.53   |  3.79   |  3.24   |  3.15   |  9.29   |   93.84  |
|    **Field 3 add 8**   |   2.50   |  3.76   |  3.24   |  3.12   |  9.48   |   93.77  |
|    **Field 3 add 9**   |   2.47   |  3.66   |  3.22   |  3.06   |  9.40   |   93.86  |
|    **Field 3 add 10**  |   2.51   |  3.74   |  3.24   |  3.11   |  9.43   |   93.79  |
|    **Field 3 add 11**  |   2.49   |  3.72   |  3.23   |  3.10   |  9.39   |   93.75  |
|    **Field 4 add 5**   |   2.54   |  3.78   |  3.26   |  3.15   |  9.43   |   93.64  |
|    **Field 4 add 6**   |   2.52   |  3.82   |  3.19   |  3.17   |  8.41   |   93.67  |
|    **Field 4 add 7**   |   2.52   |  3.79   |  3.24   |  3.14   |  9.36   |   93.76  |
|    **Field 4 add 8**   |   2.49   |  3.76   |  3.24   |  3.12   |  9.52   |   93.71  |
|    **Field 4 add 9**   |   2.46   |  3.68   |  3.21   |  3.06   |  9.45   |   93.80  |
|    **Field 4 add 10**  |   2.49   |  3.73   |  3.24   |  3.10   |  9.60   |   93.71  |
|    **Field 4 add 11**  |   2.47   |  3.69   |  3.23   |  3.07   |  9.48   |   93.68  |
|    **Field 5 add 6**   |   2.54   |  3.84   |  3.20   |  3.18   |  8.64   |   93.81  |
|    **Field 5 add 7**   |   2.54   |  3.79   |  3.25   |  3.15   |  9.54   |   93.86  |
|    **Field 5 add 8**   |   2.51   |  3.77   |  3.24   |  3.13   |  9.59   |   93.81  |
|    **Field 5 add 9**   |   2.47   |  3.66   |  3.22   |  3.06   |  9.52   |   93.89  |
|    **Field 5 add 10**  |   2.51   |  3.74   |  3.24   |  3.12   |  9.52   |   93.80  |
|    **Field 5 add 11**  |   2.49   |  3.70   |  3.24   |  3.08   |  9.64   |   93.80  |
|    **Field 6 add 7**   |   2.50   |  3.79   |  3.20   |  3.14   |  8.94   |   93.84  |
|    **Field 6 add 8**   |   2.48   |  3.78   |  3.21   |  3.12   |  9.22   |   93.81  |
|    **Field 6 add 9**   |   2.44   |  3.71   |  3.18   |  3.07   |  9.01   |   93.88  |
|    **Field 6 add 10**  |   2.48   |  3.78   |  3.21   |  3.12   |  9.16   |   93.81  |
|    **Field 6 add 11**  |   2.45   |  3.73   |  3.17   |  3.08   |  8.70   |   93.77  |
|    **Field 7 add 8**   |   2.47   |  3.79   |  3.19   |  3.12   |  8.91   |   93.85  |
|    **Field 7 add 9**   |   2.43   |  3.73   |  3.17   |  3.07   |  8.97   |   93.90  |
|    **Field 7 add 10**  |   2.47   |  3.77   |  3.20   |  3.11   |  9.13   |   93.85  |
|    **Field 7 add 11**  |   2.45   |  3.71   |  3.19   |  3.07   |  9.23   |   93.81  |
|    **Field 8 add 9**   |   2.42   |  3.70   |  3.15   |  3.05   |  8.80   |   93.86  |
|    **Field 8 add 10**  |   2.45   |  3.73   |  3.17   |  3.08   |  8.92   |   93.79  |
|    **Field 8 add 11**  |   2.43   |  3.70   |  3.19   |  3.05   |  9.26   |   93.76  |
|    **Field 9 add 10**  |   2.42   |  3.66   |  3.16   |  3.03   |  8.97   |   93.83  |
|    **Field 9 add 11**  |   2.40   |  3.65   |  3.17   |  3.01   |  9.23   |   93.81  |
|    **Field 10 add 11** |   2.43   |  3.67   |  3.19   |  3.04   |  9.34   |   93.76  |
|    **Field all added**   |   **2.56**   |  **3.82**   |  **3.29**   |  **3.18**   |  **9.76**   |   **94.09**  |

'SASEGAN-N' means the SASEGANs with the self-attention layer in the Nth convolutional layer. 'Model Fusion A+B' refers to the network after the fusion of SASEGAN-A and SASEGAN-B.
