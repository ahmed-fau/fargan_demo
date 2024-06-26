## <center>Jean-Marc Valin,&nbsp; Ahmed Mustafa,&nbsp; Jan Büthe</center>

<br>

<center><p><b>Xiph.Org Foundation &nbsp;&nbsp;&nbsp;&nbsp;   Amazon Web Services</b></p></center> 

<br>

### Abstract:
<p>Neural vocoders are now being used in a wide range of speech processing applications. In many of those applications, the vocoder can be the most complex component, so finding lower complexity algorithms can lead to significant practical benefits. In this work, we propose FARGAN, an autoregressive vocoder that takes advantage of long-term pitch prediction to synthesize high-quality speech in small subframes, without the need for teacher-forcing. Experimental results show that the proposed 600~MFLOPS FARGAN vocoder can achieve both higher quality and lower complexity than existing low-complexity vocoders. The quality even matches that of existing higher-complexity vocoders.</p>


<p><a href="https://2023.ieeeicassp.org/"> arxiv</a> & <a href="https://gitlab.xiph.org/xiph/opus/-/tree/spl_fargan/dnn/torch/fargan">code</a></p>

<br> 


### Comparison between different models (listening via headset is recommended):

<table align="center"  style="text-align: center;">
  <thead>
    <tr>
      <th style="text-align: center;">Original</th>
      <th style="text-align: center;">FARGAN 600MFLOPS (Proposed)</th>
      <th style="text-align: center;">HiFi-GAN (V1) 38.5GFLOPS</th>
      <th style="text-align: center;">CARGAN 64.47GFLOPS</th>
      <th style="text-align: center;">Framewise WaveGAN (FWGAN) 1.2GFLOPS</th>
      <th style="text-align: center;">LPCNet 2.8GFLOPS</th>
      <th style="text-align: center;">HiFi-GAN (V3) 2.8GFLOPS</th>
    </tr>
  </thead>
  <tbody>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_M02_si760.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_M02_si760.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v1/mic_M02_si760.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/cargan/mic_M02_si760.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fwgan_1p2gflops/mic_M02_si760.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/lpcnet_shoestring/mic_M02_si760.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v3/mic_M02_si760.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_F10_si2267.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_F10_si2267.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v1/mic_F10_si2267.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/cargan/mic_F10_si2267.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fwgan_1p2gflops/mic_F10_si2267.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/lpcnet_shoestring/mic_F10_si2267.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v3/mic_F10_si2267.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_M06_si1492.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_M06_si1492.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v1/mic_M06_si1492.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/cargan/mic_M06_si1492.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fwgan_1p2gflops/mic_M06_si1492.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/lpcnet_shoestring/mic_M06_si1492.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v3/mic_M06_si1492.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_F05_si1388.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_F05_si1388.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v1/mic_F05_si1388.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/cargan/mic_F05_si1388.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fwgan_1p2gflops/mic_F05_si1388.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/lpcnet_shoestring/mic_F05_si1388.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v3/mic_F05_si1388.wav"></audio></td>
    </tr>
    
    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_M03_si894.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_M03_si894.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v1/mic_M03_si894.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/cargan/mic_M03_si894.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fwgan_1p2gflops/mic_M03_si894.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/lpcnet_shoestring/mic_M03_si894.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v3/mic_M03_si894.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_F01_si494.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_F01_si494.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v1/mic_F01_si494.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/cargan/mic_F01_si494.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fwgan_1p2gflops/mic_F01_si494.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/lpcnet_shoestring/mic_F01_si494.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v3/mic_F01_si494.wav"></audio></td>
    </tr>


    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_M01_si572.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_M01_si572.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v1/mic_M01_si572.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/cargan/mic_M01_si572.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fwgan_1p2gflops/mic_M01_si572.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/lpcnet_shoestring/mic_M01_si572.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v3/mic_M01_si572.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_F04_si1076.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_F04_si1076.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v1/mic_F04_si1076.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/cargan/mic_F04_si1076.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fwgan_1p2gflops/mic_F04_si1076.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/lpcnet_shoestring/mic_F04_si1076.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v3/mic_F04_si1076.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_M10_si2200.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_M10_si2200.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v1/mic_M10_si2200.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/cargan/mic_M10_si2200.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fwgan_1p2gflops/mic_M10_si2200.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/lpcnet_shoestring/mic_M10_si2200.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v3/mic_M10_si2200.wav"></audio></td>
    </tr>


    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_F06_si1438.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_F06_si1438.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v1/mic_F06_si1438.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/cargan/mic_F06_si1438.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fwgan_1p2gflops/mic_F06_si1438.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/lpcnet_shoestring/mic_F06_si1438.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/hifigan_v3/mic_F06_si1438.wav"></audio></td>
    </tr>
  </tbody>
</table>

<br>

### Ablations (listening via headset is recommended):

<table align="center"  style="text-align: center;">
  <thead>
    <tr>
      <th style="text-align: center;">Original</th>
      <th style="text-align: center;">FARGAN Baseline</th>
      <th style="text-align: center;">FARGAN w/o Pitch Prediction</th>
      <th style="text-align: center;">FARGAN w/o Autoregression</th>
    </tr>
  </thead>
  <tbody>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_M02_si760.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_M02_si760.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_nopitch/mic_M02_si760.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_noar/mic_M02_si760.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_F10_si2267.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_F10_si2267.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_nopitch/mic_F10_si2267.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_noar/mic_F10_si2267.wav"></audio></td>
    </tr>
      
    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_M06_si1492.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_M06_si1492.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_nopitch/mic_M06_si1492.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_noar/mic_M06_si1492.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_F05_si1388.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_F05_si1388.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_nopitch/mic_F05_si1388.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_noar/mic_F05_si1388.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_M03_si894.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_M03_si894.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_nopitch/mic_M03_si894.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_noar/mic_M03_si894.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_F01_si494.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_F01_si494.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_nopitch/mic_F01_si494.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_noar/mic_F01_si494.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_M01_si572.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_M01_si572.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_nopitch/mic_M01_si572.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_noar/mic_M01_si572.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_F04_si1076.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_F04_si1076.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_nopitch/mic_F04_si1076.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_noar/mic_F04_si1076.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_M10_si2200.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_M10_si2200.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_nopitch/mic_M10_si2200.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_noar/mic_M10_si2200.wav"></audio></td>
    </tr>

    <tr>
      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/orig/mic_F06_si1438.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_large/mic_F06_si1438.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_nopitch/mic_F06_si1438.wav"></audio></td>

      <td><audio  controls="" style="width:150px;" preload="auto">
            <source src="wavs/fargan_noar/mic_F06_si1438.wav"></audio></td>
    </tr>
  </tbody>
</table>
