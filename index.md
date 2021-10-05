This is the demo page for the paper **"Automatic DJ Transitions with Differentiable Audio Effects and Generative Adversarial Networks"**



## Abstract
A central task of a Disc Jockey (DJ) playing music in a live setting is to control the flow of music with seamless transitions between adjacent tracks by employing various audio effects. This involves a series of decisions that depend on the audio characteristics of the music being manipulated, for which a simple rule-based system cannot exhaustively enumerate. In this paper, we explore a data-driven approach that uses a generative adversarial network to learn to create the song transition by learning from real-world DJ mixes. In particular, the generator of the model uses two differentiable digital signal processing components, an Equalizer (EQ) and fader, to mix two tracks selected by a data generation pipeline. The generator has to set the parameters of the EQs and fader in such a way that the resulting mix resembles real mixes created by human DJ, as judged by the discriminator counterpart. Result of a listening test shows that the model can achieve competitive results compared with baselines.

### Audio Samples

<hr>
We include 8 groups (A–H) of paired tracks from the testing set, and for each transition type, we include 2 groups of paired tracks. Furthermore, we create 5 mixes in each row by the following approaches with the same paired tracks.    
<hr>

1. `Sum`    : transitions created by summation of two tracks without any effects
2. `Linear` : transitions created by applying linear cross-fading in the transition region
3. `Rule`   : transitions created by general purpose expert DJs' rule
4. `GAN`    : transitions created by GANs' generator (our proposed)
5. `Human`  : transitions created by an expert DJ




#### non-vocal to non-vocal (nv-nv)

<table style='text-align: center;'>
  <tbody>
    <tr>
      <td></td>
      <td>Sum</td>
      <td>Linear</td>
      <td>Rule</td>
      <td>GAN</td>
      <td>Human</td>
    </tr>
    <tr>
      <td>A</td>
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
      <td>Sum</td>
      <td>Linear</td>
      <td>Rule</td>
      <td>GAN</td>
      <td>Human</td>
    </tr>
    <tr>
      <td>C</td>
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
      <td>Sum</td>
      <td>Linear</td>
      <td>Rule</td>
      <td>GAN</td>
      <td>Human</td>
    </tr>
    <tr>
      <td>E</td>
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
      <td>Sum</td>
      <td>Linear</td>
      <td>Rule</td>
      <td>GAN</td>
      <td>Human</td>
    </tr>
    <tr>
      <td>G</td>
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

