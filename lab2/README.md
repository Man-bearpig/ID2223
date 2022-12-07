# The largest heading
Task 1:
Hugging Face app:https://huggingface.co/spaces/Manbearpig01/whisper_swe


Task 2:

1. Ways of improvements

(a) model-centric approach - e.g., tune hyperparameters, change the
fine-tuning model architecture, etc

(a1) Adjust the learning rate. Smaller learning rate here might result in ending up at a less optimized result, but also has less possibility to miss the target.

(a2) Choose larger models such as whisper-medium or whisper-large, but the GPU resources on colab was limited so it is expensive to use them.

(a3) Different loss functions can be chosen.

(a4) As in Swedish there might be relation between words in seperate locations, we can set the evaluation intervals bigger.

(b) data-centric approach : 

(b1)Add new sources such as audio from youtube channels. They provide high-quality audio and some already have available subtitles.

(b2)Some public library can be used, such as NST Swedish Dictation:https://www.nb.no/sprakbanken/en/resource-catalogue/oai-nb-no-sbr-17/#resource-common-info.

2.checkpoints:It seems that hopsworks can't hold GBs of data, so we chose google drive.
```
from google.colab import drive
drive.mount('/content/drive')
import os
os.chdir('/content/drive/MyDrive/Colab Notebooks')
```
Google Drive:https://drive.google.com/drive/folders/1IRDk28HygcOiqZUq1IA56p1FPSzZaoXj?usp=share_link
