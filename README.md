- 👋 Hi, I’m @dvmixalkin
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
dvmixalkin/dvmixalkin is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

- [x] 3DMM - https://github.com/sshuster/3DMM-Fitting-Pytorch?ref=https://githubhelp.com
- [x] FLAME - https://github.com/soubhiksanyal/FLAME_PyTorch?ref=https://githubhelp.com
- [x] JAANet(Action Unit Recognizer) - https://github.com/ZhiwenShao/PyTorch-JAANet
- [ ] DECA - https://github.com/YadiraF/DECA
- [ ] MTCNN - https://github.com/RuoyuChen10/MTCNN_Portable.git
- [ ] Py-FEAT: Python Facial Expression Analysis Toolbox - https://github.com/cosanlab/py-feat

## Micro Expression Recognition
Micro-Expression Recognition Enhanced by Macro-Expression from Spatial-Temporal Domain
- [x] DANN(main idea how to improve student performance) - https://github.com/NaJaeMin92/pytorch_DANN
- [ ] MA-Net - https://github.com/zengqunzhao/MA-Net
- [ ] MicroNet - https://github.com/ListIndexOutOfRange/MicroNet
- [ ] TSCNN - https://github.com/jeffreyyihuang/two-stream-action-recognition 
- [ ] ICE-GAN - https://github.com/crane-papercode/ICE-GAN 
- [ ] GRAPH-AU - https://github.com/Justin900429/Facial-Graph-Representation-Learning
- [ ] CapsuleNet - https://github.com/davidnvq/me_recognition
- [ ] STSTNet - https://github.com/christy1206/STSTNet

## TOLearn
- [ ] PyTorch-GAN - https://github.com/eriklindernoren/PyTorch-GAN

# MER on SMIC, CASME, CASME II, SAMM, and CMED datasets.

|Dataset|     Method      |Year|Pre-p. |Input   |Network architecture |Block |Pre-train    |Protocol |Cate. |  F1 |ACC (%)|
|-------|-----------------|----|-------|--------|---------------------|------|-------------|---------|------|------|-------|
|SMIC   |3D-CNN+LSTM [117]|2019|      -|Sequence|3DCNN+LSTM           |     -|            -|     LOSO|     3|     -|   56.6|
|       | OFF-ApexNet [96]|2019|      -|OF      |2S-CNN               |     -|            -|     LOSO|     3|0.6709|  67.68|
|       | TSCNN [100]     |2019|E, R   |OF+Apex |3S-CNN               |     -|FER2013 [193]|     LOSO|     3|0.7236|  72.74|
|       | LEARNet [76]    |2019|      -|DI      |CNN                  |Hybrid|            -|     LOSO|     3|     -|  81.60|
|       | STRCN-G [57]    |2019|E      |OF|CNN| RCN| - |LOSO| 3| 0.695| 72.3|
|       | STSTNet [107]   |2019| E| OF| 3S-3DCNN| -| - |LOSO| 3| 0.6801| 70.13|
|       | LGCcon [56]     |2020| E, R| Apex| CNN| Attention| VGG-FACE [180]| LOSO| 3| 0.62| 63.41|
|       | CBAMNet [90]    |2020| E, T| Sequence| 3DCNN| Attention| Oulu-CASIA [194]| 10-fold| 3| -| 54.84|
|       | DIKD [66]       |2020| -| Apex| CNN+KD+SVM| -| -| LOSO| 3| 0.71| 76.06|
|       | SMA-STN [71]    |2020| -| Snippet| CNN| -| WIDER FACE [195]| LOSO |3| 0.7683| 77.44|
|       | SETFNet [175]   |2020| R| Sequence| 3S-3DCNN| SE| -| 5-Fold| 5| -| 70.25|
|       | MTMNet [123]    |2020| -| Onset-Apex| 2S-CNN+DA+GAN| RES |CK+[196],MMI [10],| Oulu-CASIA [194]| LOSO |3| 0.744| 76.0 |
|       | GEME [74]       |2021| -| DI| 2S-CNN+ML| RES |-| LOSO |3| 0.6158 |64.63|
|       | MiMaNet [186]   |2021| T| Apex+sequence| 2S-CNN+DA| RES| CK+ [196],MMI [10]| LOSO| 3| 0.778 |78.6|
|       | DSTAN [176]     |2021| T| OF+sequence |2S-CNN+LSTM+SVM| Attention |-| LOSO |3| 0.78| 77|
|       | KFC [173]       |2021| -| OF| 2S-CNN| Attention |-| LOSO| 3| 0.6638| 65.85|
|CASME  |TSCNN [100]| 2019 |E,R| OF+Apex |3S-CNN| - |FER2013 [193]| LOSO |4| 0.7270 |73.88|
|CASME  |LEARNet [76] 2019 - DI CNN Hyfeat - LOSO 8 - 80.62
|CASME  |LGCcon [56] 2020 E, R Apex CNN Attention VGG-FACE [180] LOSO 4 0.60 60.82
|CASME  |DIKD [66] 2020 - Apex CNN+KD+SVM RES - LOSO 4 0.77 81.80
|CASME  |OrigiNet [77] 2020 - AI CNN Hyfeat - LOSO 4 - 66.09
|CASME  |AffectiveNet [163] 2020 E DI 4S-CNN MFL - LOSO 4 - 72.64
|CASME  |DSTAN [176] 2021 T OF+sequence 2S-CNN+LSTM+SVM Attention - LOSO 4 0.75 78

CASME II
ELRCN [113] 2018 T OF 4S-CNN+LSTM - VGG-Face [180] LOSO 5 0.5 52.44
OFF-ApexNet [96] 2019 - OF 2S-CNN - - LOSO 3 0.8697 88.28
TSCNN [100] 2019 E, R OF+Apex 3S-CNN - FER2013 [193] LOSO 5 0.807 80.97
LEARNet [76] 2019 - DI CNN Hyfeat - LOSO 7 - 76.57
STRCN-G [57] 2019 E OF CNN RCN - LOSO 3 0.747 80.3
STSTNet [107] 2019 E OF 3S-3DCNN - - LOSO 3 0.8382 86.86
3D-CNN+LSTM [117] 2019 - Sequence 3DCNN+LSTM - - LOSO 5 - 62.5
Graph-TCN [92] 2020 L, R Apex TCN+GCN Graph - LOSO 5 0.7246 73.98
AU-GACN [55] 2020 - Sequence 3DCNN+GCN Graph - LOSO 3 0.355 71.2
CBAMNet [90] 2020 E, T Sequence 3DCNN Attention Oulu-CASIA [194] 10-fold 3 - 69.92
LGCcon [56] 2020 E, R Apex CNN Attention VGG-FACE [180] LOSO 5 0.64 65.02
CNNCapsNet [82] 2020 - OF 5S-CNN Capsule - LOSO 5 0.6349 64.63
DIKD [66] 2020 - Apex CNN+KD+SVM - - LOSO 4 0.67 72.61
OrigiNet [77] 2020 - AI CNN Hyfeat - LOSO 4 - 62.09
SMA-STN [71] 2020 - Snippet CNN Attention WIDER FACE [195] LOSO 5 0.7946 82.59
SETFNet [175] 2020 R Sequence 3S-3DCNN SE - 5-Fold 5 - 66.28
AffectiveNet [163] 2020 E DI 4S-CNN MFL - LOSO 4 - 68.74
GEME [74] 2021 - DI 2S-CNN+ML RES - LOSO 5 0.7354 75.20
MiMaNet [186] 2021 T Apex+sequence 2S-CNN+DA RES CK+ [196],MMI [10] LOSO 5 0.759 79.9
LR-GACNN [72] 2021 E OF+Landmark 2S-GACNN Graph - LOSO 5 0.7090 81.30
GRAPH-AU [166] 2021 L Apex 2S-CNN+GCN Graph,
Transformer - LOSO 5 0.7047 74.27
DSTAN [176] 2021 T OF+sequence 2S-CNN+LSTM+SVM Attention - LOSO 5 0.73 75
KFC [173] 2021 - OF 2S-CNN Attention - LOSO 5 0.7375 72.76

SAMM
OFF-ApexNet [96] 2019 OF 2S-CNN - - LOSO 3 0.5423 68.18
STSTNet [107] 2019 E OF 3S-3DCNN - - LOSO 3 0.6588 68.10
Graph-TCN [92] 2020 L,R Apex TCN+GCN Graph - LOSO 5 0.6985 75.00
AU-GACN [55] 2020 - Sequence 3DCNN+GCN Graph - LOSO 3 0.433 70.2
LGCcon [56] 2020 E, R Apex CNN Attention VGG-FACE [180] LOSO 5 0.34 40.90
STRCN-G [57] 2019 E OF CNN RCN - LOSO 3 0.741 78.6
TSCNN [100] 2019 E, R OF+Apex 3S-CNN - FER2013 [193] LOSO 5 0.6942 71.76
DIKD [66] 2020 - Apex CNN+KD+SVM - - LOSO 4 0.83 86.74
OrigiNet [77] 2020 - AI CNN Hyfeat - LOSO 4 - 34.89
SMA-STN [71] 2020 - Snippet CNN - WIDER FACE [195] LOSO 5 0.7033 77.20
MTMNet [123] 2020 - Onset-Apex 2S-CNN+GAN+DA RES CK+ [196],MMI [10],
Oulu-CASIA [194]
LOSO 5 0.736 74.1
GEME [74] 2021 - DI 2S-CNN+ML RES - LOSO 5 0.4538 55.88
MiMaNet [186] 2021 T Apex+sequence 2S-CNN+DA RES CK+ [196],MMI [10] LOSO 5 0.764 76.7
LR-GACNN [72] 2021 E OF+Landmark 2S-GACNN - - LOSO 5 0.8279 88.24
GRAPH-AU [166] 2021 L Apex 2S-CNN+GCN Graph,
Transformer - LOSO 5 0.7045 74.26
KFC [173] 2021 - OF 2S-CNN Attention - LOSO 5 0.5709 63.24

CMED Shallow CNN [35] 2020 E OF CNN - - LOSO 7 0.6353 66.06
