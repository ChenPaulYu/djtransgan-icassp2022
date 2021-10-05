This is the demo page for the paper **"Automatic DJ Transitions with Differentiable Audio Effects and Generative Adversarial Networks"**



## Abstract
A central task of a Disc Jockey (DJ) playing music in a livesetting  is  to  control  the  flow  of  music  with  seamless  tran-sitions between adjacent tracks by employing various audioeffects. This  involves  a  series  of  decisions  that  depend  onthe audio characteristics of the music being manipulated, for which a simple rule-based system cannot exhaustively enumerate. In this paper, we explore a data-driven approach that uses a generative adversarial  network to learn to create  the song  transition by learning from real-world  DJ  mixes. In particular, the generator of the model uses two differentiabledigital signal processing components, an Equalizer (EQ) and fader, to mix two tracks selected by a data generation pipeline. The generator has to set the parameters of the EQs and fader in such a way that the resulting mix resembles real mixes created by human DJ, as judged by the discriminator counterpart. Result of a listening test shows that the model can achieve competitive results compared with baselines.

### Audio Samples

<hr>

1. `Sum` : 
2. Loop combination made by human based on Query loop (`Original`)
3. Generated loop combination based on Query loop by `AutoMashupper`
4. Generated loop combination based on Query loop by `CNN+reverse`

|   |Transition Type|Sum|Linear|Rule|GAN|Human|
|1.|nv-nv|<audio src="assets/audios/1/sum.wav" controls="" preload=""></audio>|<audio src="assets/audios/1/linear.wav" controls="" preload=""></audio>|<audio src="assets/audios/1/rule" controls="" preload=""></audio>|<audio src="assets/audios/1/gan.wav" controls="" preload=""></audio>|<audio src="assets/audios/1/human.wav" controls="" preload=""></audio>|
|2.|nv-nv|<audio src="assets/audios/2/sum.wav" controls="" preload=""></audio>|<audio src="assets/audios/2/linear.wav" controls="" preload=""></audio>|<audio src="assets/audios/2/rule" controls="" preload=""></audio>|<audio src="assets/audios/2/gan.wav" controls="" preload=""></audio>|<audio src="assets/audios/2/human.wav" controls="" preload=""></audio>|
|3.|nv-v|<audio src="assets/audios/3/sum.wav" controls="" preload=""></audio>|<audio src="assets/audios/3/linear.wav" controls="" preload=""></audio>|<audio src="assets/audios/3/rule" controls="" preload=""></audio>|<audio src="assets/audios/3/gan.wav" controls="" preload=""></audio>|<audio src="assets/audios/3/human.wav" controls="" preload=""></audio>|
|4.|nv-v|<audio src="assets/audios/4/sum.wav" controls="" preload=""></audio>|<audio src="assets/audios/4/linear.wav" controls="" preload=""></audio>|<audio src="assets/audios/4/rule" controls="" preload=""></audio>|<audio src="assets/audios/4/gan.wav" controls="" preload=""></audio>|<audio src="assets/audios/4/human.wav" controls="" preload=""></audio>|

### Contact 

<hr>

Bo-Yu Chen bernie40916@gmail.com

