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
Firstly, I changed the number of instruments, we will see the assumption is good which we still could recognize the style but the piano song changed to symphony concert which is very interesting.
![](https://github.com/ucsd-ml-arts/generative-audio-zizhen-wang/blob/master/01.jpg) ![](https://github.com/ucsd-ml-arts/generative-audio-zizhen-wang/blob/master/02.jpg) [generated_clip.wav](https://drive.google.com/drive/u/0/folders/1YpMPXa_yhK15U-gevQIJHAhNd4H8c_RO)
Secondly, I only inputed the  piano music to musicVAE which changed the melody. We will see all the song changed to the piano song, but when the melody changed.
I put the generated song into Transformer, we would see the rhythm changed a lot but the melody almost keeped same.

## Technical Notes



## Reference
- Music Transformer: Generating Music with Long-Term Structure
https://magenta.tensorflow.org/music-transformer
- MusicVAE: Creating a palette for musical scores with machine learning.
https://magenta.tensorflow.org/music-vae
- GANSynth: Making music with GANs
https://magenta.tensorflow.org/gansynth
