# **Audio Denoiser**
# **Work In Progress**
This project attempts to build an audio denoiser using Deep Learning to study the noise pattern from the spectrogram respresentation of the noisy audio and clean audio.
The dataset is created using three open sources for audio data, including:
- Clean audio:
  + Mozilla Common Voice: consists of 7,226 recorded hours in .mp3 forms (with diversity accents, genders, etc).
- Noise audio:
  + UrbanSound8K Dataset: 10 common environment noises
  + ESC-50 dataset: More diverse noises: tic clock, footsteps, etc.
By combining the noise audio and clean audio, the train and test data are created. 

Some input configs used in this project include:
- Audio length: Limited to 3-second length 
- Sampling rate: 8kHz 
- Hop-length: 188
- Number of FFT: 255

This project uses U-Net model as the base model.

# **References**

Speech enhancement: https://github.com/vbelz/Speech-enhancement

Daitan (2019), How To Build a Deep Audio De-Noiser Using TensorFlow 2.0. Available online: https://medium.com/better-programming/how-to-build-a-deep-audio-de-noiser-using-tensorflow-2-0-79c1c1aea299

Lamba, H. (2019), Understanding Semantic Segmentation with UNET. Available online: https://towardsdatascience.com/understanding-semantic-segmentation-with-unet-6be4f42d4b47
