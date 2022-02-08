---
layout: default
---
# Portfolio

## Dereverberación del habla utilizando Redes Neuronales Convolucionales (CNN)

In this research, speech dereverberation based on deep learning algorithms is studied. A convolutional neural network model called autocoder with skip connections is implemented, following the current state of the art. The neural network is developed to estimate amplitude masks that perform speech dereverberation in the short-time Fourier transform domain. One of the issues of this particular task is the lack of a large training dataset, so generation and augmentation techniques were analyzed, evaluating the impact on model’s performance. In addition, ways to handle phase information and data during training were studied.  

![Estructura Implementada](/images/modelo_red.png)

The results show that the generation and augmentation techniques allow to improve the model’s performance. Moreover, sorting the training data from smallest to largest reverberation time results in better evaluation metrics. Finally, improvements for the implemented model and future lines of research were proposed.

This research was the final thesis work developed to achieve the Sound Engineer degree in Universidad Nacional de Tres de Febrero, and has been finished in November 2021. Full document is available in this <a href="pdf/Meza_Dereverberación del habla a partir de algoritmos de aprendizaje profundo.pdf">link</a>.

<p align="center">
<a href="https://martinbmeza.github.io/deep-dereverb/">Keep Reading</a> |
<a href="https://github.com/martinBmeza/deep-dereverb">See GitHub Repo</a>
</p>


## Analisis and Augmentation of Room Impulse Responses
Room Impulse Response databases are usually expensive and time-consuming to collect. Moreover, if we analyze some acoustics parameters like reverberation time (RT) and direct-to-reverberant ratio (DRR) in the database, in general it is difficult to achieve a good variation of these parameters. In other words, small size datasets bring issues in some applications like training deep learning models. However, some studies have proposed several techniques to perform RIR augmentation, having control over certain acoustic parameters like the ones mentioned above, RT and DRR. Here, these techniques to parametrically control the RT and DRR where implemented generating a useful tool that allows expand a small dataset of RIR into a balanced dataset order of magnitude larger.

![Aumentacion](/images/tr_aug.png)

Also, this work provide some python scripts to perform basic acoustic analysis of audio signals, and more precisely, of RIRs, such as band-filtering, reverberation time calculation, direct-to-reverberant ratio calculation, and implementations of noise floor estimation methods.

![Filtros](/images/banco_filtros.png)

<p align="center">
<a href="pdf/rir_aug.pdf">Keep Reading</a> |
<a href="https://github.com/martinBmeza/rir_analysis">See GitHub Repo</a>
</p>


<!---# Audio Denoising Framework 
La idea de este projecto es servir como un punto de partida para explicar el uso de ciertas herramientas referidas a la inteligencia artificial y el uso de redes neuronales. Se plantea una aplicacion de ejemplo que consiste en elimiar ruido blanco presente en un tono puro. Se crean datos de partida, se arma un modelo de red neuronal convolucional tipo auto-encoder, se compila y entrena este modelo y se lo utiliza para hacer predicciones. De esta manera se recorren todas las instancias que entran en juego a la hora de desarrollar un projecto de esta indole. Las librerias que se utilizan son:
+ Tensorflow
+ Librosa
+ Numpy -->