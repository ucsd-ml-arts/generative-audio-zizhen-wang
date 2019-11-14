# Project 3 Generative Audio

Zizhen Wang, ziw142@ucsd.edu



## Abstract

Different types music always have the specific rhythm, melody and instruments. People could recognize these sytles depends on the them but if we use machine learning to generate the new music which it may change the number of instrument, the melody and the rhythm, could we still can recognize them. I will sue GANsynth, MusicVAE and Transformer to change the number of instruments, the melody and the rhythm in different orders to get results

## Model/Data


La companella
This is a piano song which represents classical style and only one instrument.



## Code
Jupyter notebooks: 
- generative_code.ipynb [gansynth_external.ipynb](https://github.com/ucsd-ml-arts/generative-audio-zizhen-wang/blob/master/gansynth_external.ipynb)
- Generating Piano Music with Transformer.ipynb [Generating_Piano_Music_with_Transformer.ipynb](https://github.com/ucsd-ml-arts/generative-audio-zizhen-wang/blob/master/Generating_Piano_Music_with_Transformer.ipynb)
- MusicVAE.ipynb [MusicVAE.ipynb](https://github.com/ucsd-ml-arts/generative-audio-zizhen-wang/blob/master/MusicVAE.ipynb)

## Results
- Firstly, I used GANSynth generator to generate new music by 16 random samples of instruments. GANSynth is a new approach to audio synthesis using neural networks to release a playable set of neural synthsizer instruments. The Synth dataset has a lot of intruments samples and qualities like bright or dark.  They use encoder and decoder to generate new instuments into new waveform. The generate custom inerpolation for instruments: [0, 3, 6, 0] and for time :[0, 0.3, 0.6, 1.0]
![](https://github.com/ucsd-ml-arts/generative-audio-zizhen-wang/blob/master/01.jpg) ![](https://github.com/ucsd-ml-arts/generative-audio-zizhen-wang/blob/master/02.jpg)
- [03 - La Campanella.mp3](https://www.driveplayer.com/#fileIds=1uJ7OjY9J_JI7a-0ljdvY03kuDINwl8_7&userId={userId})
- [generated_clip.wav](https://www.driveplayer.com/#fileIds=1wes7C-NwRwIrbI1a45EJgnVIOejcnAdv&userId={userId}) You could also download from github if you do not have permission.
- The first one is original music and second one is generated music. We will see the form for x-axis is almost same which means the rhythm and melody is almost same. We could also listen from these 2 musics. The interesting thing is the generated music still keep the classic music style and it listens like symphony or drama which have a lot of instruments.

-Secondly, I used Generating Piano Music with Transformer for melody-conditioned piano performance model. Music Transformer is an attention-based neural network that can generate music with improved long-term coherence. For the training data, I both use the original music and generated music by GANSynth to input 16-bar melody models and temperature is 0.5.
![](https://github.com/ucsd-ml-arts/generative-audio-zizhen-wang/blob/master/03.jpg) ![](https://github.com/ucsd-ml-arts/generative-audio-zizhen-wang/blob/master/04.jpg)
- [hierdec_mel_16bar_mean.mp3](https://www.driveplayer.com/#fileIds=1RWU81FDX85-TUaEZ3KXS5KQJ0IAsuJro&userId={userId})
- [hierdec_mel_16bar_mean2.mp3](https://www.driveplayer.com/#fileIds=1RqNkG644XDAfcey46_jTpsk7ekVPqLod&userId=104858041665593101824)  You could also download from github if you do not have permission.



## Technical Notes



## Reference
- Music Transformer: Generating Music with Long-Term Structure
https://magenta.tensorflow.org/music-transformer
- MusicVAE: Creating a palette for musical scores with machine learning.
https://magenta.tensorflow.org/music-vae
- GANSynth: Making music with GANs
https://magenta.tensorflow.org/gansynth
