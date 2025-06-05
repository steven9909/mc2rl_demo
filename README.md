<table>
  <tr>
    <th>Input</th>
    <th>CUT</th>
    <th>CUT + Dataset Augmentation</th>
    <th>CUT + Cycle</th>
    <th>CUT + Cycle (Low λ)</th>
    <th>CUT + Cycle + MultScale Discrim</th>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/c63eb8f0-4ac9-497e-b06c-6bafcc5fe24c" width="240"/></td>
    <td><img src="https://github.com/user-attachments/assets/b0494b45-f878-4c5a-bd66-17fbd77a8f65" width="240"/></td>
    <td><img src="https://github.com/user-attachments/assets/68895c08-d424-4c27-9a09-977169b4554e" width="240"/></td>
    <td><img src="https://github.com/user-attachments/assets/845160fd-12e1-42e9-917b-d4e72daab3a5" width="240"/></td>
    <td><img src="https://github.com/user-attachments/assets/751e75ea-dafe-4d1b-815f-93e1555b72bc" width="240"/></td>
    <td><img src="https://github.com/user-attachments/assets/02aceaa6-e8c8-4210-b094-7140c106f948" width="240"/></td>
  </tr>
</table>

### 📊 FID Score Comparison (↓ Lower is Better)


> *Fréchet Inception Distance (FID) computed against real images from the **LHQ** dataset. Lower scores indicate higher perceptual similarity and realism.*

<table>
  <tr>
    <th>Input</th>
    <th>CUT + Dataset Augmentation</th>
    <th>CUT + Cycle</th>
    <th>CUT + Cycle (Low λ)</th>
  </tr>
  <tr>
    <td>198.68</td>
    <td>114.45</td>
    <td>106.45</td>
    <td>108.64</td>
  </tr>
</table>

### 📊 Mean SSIM Score (↑ Higher is Better)

> *Structual Similiarity Index (SSIM) computed against subsequent frames. Higher scores indicate higher perceptual similarity inbetween frames.*

<table>
  <tr>
    <th>Input</th>
    <th>CUT + Dataset Augmentation</th>
    <th>CUT + Cycle</th>
    <th>CUT + Cycle (Low λ)</th>
  </tr>
  <tr>
    <td>0.329</td>
    <td>0.228</td>
    <td>0.236</td>
    <td>0.245</td>
  </tr>
</table>

### TODO

Fix temporal consistency issues:
 - Color consistency loss
 - Gaussian filtering in temporal domain
 - Conditioned training on previous frames
 - Optical flow
 - Self consistency loss
