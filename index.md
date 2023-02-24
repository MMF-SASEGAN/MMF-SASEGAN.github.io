# MMF-SASEGAN

Since there are more and more speech-related applications and various noises exist in real life, speech enhancement plays an important role. However, speech enhancement (SE) systems, based on generative adversarial networks (GANs), are limited in improving speech quality and intelligibility. In this study, we propose a novel multi-model fusion SE system based on self-attention generative adversarial networks (MMF-SASEGAN). The models with different positions of the self-attention layers focus on different features. Considering the effect of the position of the self-attention layers on SE performance, SASEGANs with self-attention layers at different positions are fused. For speech quality, the proposed method improves by 8.22%, 8.52%, 9.28%, and 9.40% in CBAK, CSIG, COVL, and PESQ on average compared with the baseline SASEGANs. As to SSNR and STOI, compared with the baseline SASEGANs on average, the proposed method obtains absolute gains of 1.71 and 0.77, respectively. The results show that the MMF-SASEGAN comprehensively improves the performance of the baseline SASEGAN and performs better than the mainstream GAN-based SE methods. Importantly, the proposed method may generalize to other GAN-based SE methods.

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
|    **MMF-SASEGAN**    |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/M_1.wav"></source> </audio>   |    <audio controls="controls">  <source type="audio/wav" src="https://raw.githubusercontent.com/MMF-SASEGAN/MMF-SASEGAN.github.io/main/wavs/M_2.wav"></source> </audio>  |

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
|    **Model Fusion 3+4**   |   2.54    |  3.79   |  3.24   |  3.16   |  9.12   |   93.60  |
|    **Model Fusion 3+5**   |   2.56    |  3.81   |  3.25   |  3.17   |  9.28   |   93.77  |
|    **Model Fusion 3+6**   |   2.53    |  3.83   |  3.17   |  3.17   |  8.25   |   93.78  |
|    **Model Fusion 3+7**   |   2.53    |  3.79   |  3.24   |  3.15   |  9.29   |   93.84  |
|    **Model Fusion 3+8**   |   2.50    |  3.76   |  3.24   |  3.12   |  9.48   |   93.77  |
|    **Model Fusion 3+9**   |   2.47    |  3.66   |  3.22   |  3.06   |  9.40   |   93.86  |
|    **Model Fusion 3+10**   |  2.51    | 3.74    |  3.24   |  3.11   |  9.43   |   93.79  |
|    **Model Fusion 3+11**   |  2.49    | 3.72    |  3.23   |  3.10   |  9.39   |   93.75  |
