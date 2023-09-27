# Wave_Generation

## Diffwave
![image](https://github.com/Yukino1010/Wave_Generation/blob/master/image_source/img_1.png)

Kong et al. (2020) introduced DiffWave as a probabilistic diffusion model that can generate conditional and unconditional waveforms.  <br>
It converts white noise signals into structured waveforms during synthesis using a constant number of steps using a Markov chain mechanism.

## The Key Advantages Offered by DiffWave
### Better audio quality
Have a better performance in the unconditional and conditional waveform generation tasks.😄😄

### Enhanced Generative Speed:
The diffusion model is non-autoregressive. It can synthesise high-dimensional waveforms in parallel.

### No Need for Extra Neural Networks:
Diffusion models utilise a parameter-free diffusion process, eliminating the need for additional neural networks during training. <br>
This avoids the 'posterior collapse' or 'mode collapse' challenges associated with joint training (VAE, GAN….).

## Training Process of Diffwave
![image](https://github.com/Yukino1010/Wave_Generation/blob/master/image_source/img_3.png)

The training process of DiffWave is similar to that of a typical diffusion model.  <br>
The only difference is that it replaces the original U-Net model with a WaveNet model, which is better suited for generating speech.

The diffusion model mainly comprises two processes, Forward Noising and Backward Denoising;  <br>
this could be regarded as continuously adding noise into the image and then reversing this process. 😃😃

## Architecture

![image](https://github.com/Yukino1010/Wave_Generation/blob/master/image_source/img_2.png)

***For the detail, welcome visit my medium*** [[link](https://medium.com/p/b6579be7838e/edit)]


## References
1. ***WaveNet: A Generative Model for Raw Audio*** [[link](https://arxiv.org/abs/1609.03499)]
2. ***DiffWave: A Versatile Diffusion Model for Audio Synthesis*** [[link](https://arxiv.org/abs/2009.09761)]
3. ***Denoising Diffusion Probabilistic Models*** [[link](https://arxiv.org/abs/2006.11239)]

