This is the demo page for the paper **"Automatic DJ Transitions with Differentiable Audio Effects and Generative Adversarial Networks"**



## Abstract
A central task of a Disc Jockey (DJ) playing music in a livesetting  is  to  control  the  flow  of  music  with  seamless  tran-sitions between adjacent tracks by employing various audioeffects. This  involves  a  series  of  decisions  that  depend  onthe audio characteristics of the music being manipulated, for which a simple rule-based system cannot exhaustively enumerate. In this paper, we explore a data-driven approach that uses a generative adversarial  network to learn to create  the song  transition by learning from real-world  DJ  mixes. In particular, the generator of the model uses two differentiabledigital signal processing components, an Equalizer (EQ) and fader, to mix two tracks selected by a data generation pipeline. The generator has to set the parameters of the EQs and fader in such a way that the resulting mix resembles real mixes created by human DJ, as judged by the discriminator counterpart. Result of a listening test shows that the model can achieve competitive results compared with baselines.

### Audio Samples

<hr>

1. `Sum` : 
2. `Linear` : 
3. `Rule` : 
4. `GAN` : 
5. `Human` : 
<div align="center">

| |Transition Type|Sum|Linear|Rule|GAN|Human|
|A|nv-nv|<audio src="assets/audios/1/sum.wav" controls="" preload=""></audio>|<audio src="assets/audios/1/linear.wav" controls="" preload=""></audio>|<audio src="assets/audios/1/rule.wav" controls="" preload=""></audio>|<audio src="assets/audios/1/gan.wav" controls="" preload=""></audio>|<audio src="assets/audios/1/human.wav" controls="" preload=""></audio>|
|B|nv-nv|<audio src="assets/audios/2/sum.wav" controls="" preload=""></audio>|<audio src="assets/audios/2/linear.wav" controls="" preload=""></audio>|<audio src="assets/audios/2/rule.wav" controls="" preload=""></audio>|<audio src="assets/audios/2/gan.wav" controls="" preload=""></audio>|<audio src="assets/audios/2/human.wav" controls="" preload=""></audio>|
|C|nv-v|<audio src="assets/audios/3/sum.wav" controls="" preload=""></audio>|<audio src="assets/audios/3/linear.wav" controls="" preload=""></audio>|<audio src="assets/audios/3/rule.wav" controls="" preload=""></audio>|<audio src="assets/audios/3/gan.wav" controls="" preload=""></audio>|<audio src="assets/audios/3/human.wav" controls="" preload=""></audio>|
|D|nv-v|<audio src="assets/audios/4/sum.wav" controls="" preload=""></audio>|<audio src="assets/audios/4/linear.wav" controls="" preload=""></audio>|<audio src="assets/audios/4/rule.wav" controls="" preload=""></audio>|<audio src="assets/audios/4/gan.wav" controls="" preload=""></audio>|<audio src="assets/audios/4/human.wav" controls="" preload=""></audio>|

<div/>
### Contact 

<hr>
Bo-Yu Chen: bernie40916@gmail.com

