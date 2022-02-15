This is the demo page for the paper **"Automatic DJ Transitions with Differentiable Audio Effects and Generative Adversarial Networks"**. Source code can be found [here](https://github.com/ChenPaulYu/DJtransGAN)


## Abstract
A central task of a Disc Jockey (DJ) is to create a mixset of music with seamless transitions between adjacent tracks. In this paper, we explore a data-driven approach that uses a generative adversarial network to create the song transition by learning from real-world DJ mixes. In particular, the generator of the model uses two differentiable digital signal processing components, an Equalizer (EQ) and fader, to mix two tracks selected by a data generation pipeline. The generator has to set the parameters of the EQs and fader in such a way that the resulting mix resembles real mixes created by human DJ, as judged by the discriminator counterpart. Result of a listening test shows that the model can achieve competitive results compared with baselines.

### Audio Samples

<hr>
We include 8 groups (A–H) of paired tracks (x1, x2) from the testing set, and for each transition type, we include 2 groups of paired tracks. Furthermore, we create 5 mixes (x3^) in each row by the following approaches with the same paired. In colclusion, we provide totally 7 audios in each row which include 2 paired tracks and 5 mixs, the detailed is shown below.
<hr>

![Mixing Pipeline](./assets/images/pipeline.png 'Mixing Pipeline')



1. `Prev`   : track which is considered to be the first track in a mix as shown in figure above (x1)
2. `Next`   : track which is considered to be the second track in a mix as shown in figure above (x2)
3. `Sum`    : transitions created by summation of two tracks without any effects
4. `Linear` : transitions created by applying linear cross-fading in the transition region
5. `Rule`   : transitions created by general purpose expert DJs' rule
6. `GAN`    : transitions created by GANs' generator (our proposed)
7. `Human`  : transitions created by an expert DJ




#### non-vocal to non-vocal (nv-nv)

<table style='text-align: center;'>
  <tbody>
    <tr>
      <td></td>
      <td>Prev</td>
      <td>Next</td>
      <td>Sum</td>
      <td>Linear</td>
      <td>Rule</td>
      <td>GAN</td>
      <td>Human</td>
    </tr>
    <tr>
      <td>A</td>
      <td><audio controls=""><source src="./assets/audios/1/prev.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/1/next.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/1/sum.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/1/linear.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/1/rule.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/1/gan.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/1/human.wav" type="audio/mpeg" /></audio></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>B</td>
      <td><audio controls=""><source src="./assets/audios/2/prev.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/2/next.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/2/sum.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/2/linear.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/2/rule.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/2/gan.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/2/human.wav" type="audio/mpeg" /></audio></td>
    </tr>
  </tfoot>
</table>

#### non-vocal to vocal (nv-v)

<table style='text-align: center;'>
  <tbody>
    <tr>
      <td></td>
      <td>Prev</td>
      <td>Next</td>
      <td>Sum</td>
      <td>Linear</td>
      <td>Rule</td>
      <td>GAN</td>
      <td>Human</td>
    </tr>
    <tr>
      <td>C</td>
      <td><audio controls=""><source src="./assets/audios/3/prev.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/3/next.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/3/sum.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/3/linear.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/3/rule.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/3/gan.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/3/human.wav" type="audio/mpeg" /></audio></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>D</td>
      <td><audio controls=""><source src="./assets/audios/4/prev.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/4/next.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/4/sum.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/4/linear.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/4/rule.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/4/gan.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/4/human.wav" type="audio/mpeg" /></audio></td>
    </tr>
  </tfoot>
</table>



#### vocal to non-vocal (v-nv)

<table style='text-align: center;'>
  <tbody>
    <tr>
      <td></td>
      <td>Prev</td>
      <td>Next</td>
      <td>Sum</td>
      <td>Linear</td>
      <td>Rule</td>
      <td>GAN</td>
      <td>Human</td>
    </tr>
    <tr>
      <td>E</td>
      <td><audio controls=""><source src="./assets/audios/5/prev.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/5/next.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/5/sum.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/5/linear.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/5/rule.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/5/gan.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/5/human.wav" type="audio/mpeg" /></audio></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>F</td>
      <td><audio controls=""><source src="./assets/audios/6/prev.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/6/next.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/6/sum.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/6/linear.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/6/rule.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/6/gan.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/6/human.wav" type="audio/mpeg" /></audio></td>
    </tr>
  </tfoot>
</table>


#### vocal to vocal (v-v)

<table style='font-size: 12px; text-align: center;'>
  <tbody>
    <tr>
      <td></td>
      <td>Prev</td>
      <td>Next</td>
      <td>Sum</td>
      <td>Linear</td>
      <td>Rule</td>
      <td>GAN</td>
      <td>Human</td>
    </tr>
    <tr>
      <td>G</td>
      <td><audio controls=""><source src="./assets/audios/7/prev.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/7/next.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/7/sum.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/7/linear.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/7/rule.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/7/gan.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/7/human.wav" type="audio/mpeg" /></audio></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>H</td>
      <td><audio controls=""><source src="./assets/audios/8/prev.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/8/next.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/8/sum.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/8/linear.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/8/rule.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/8/gan.wav" type="audio/mpeg" /></audio></td>
      <td><audio controls=""><source src="./assets/audios/8/human.wav" type="audio/mpeg" /></audio></td>
    </tr>
  </tfoot>
</table>



### Contact 

<hr>
Bo-Yu Chen: bernie40916@gmail.com

