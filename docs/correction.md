# Correction Tab

The **Correction** tab provides tools for editing and enhancing nighttime sky images before detection and charting.

---

## Table of Contents

- [Colors](#colors)
- [Brightness](#brightness)
- [Contrast](#contrast)
- [Saturation](#saturation)
- [Sharpness](#sharpness)
- [Blur](#blur)
- [Noise Reduction](#noise-reduction)
- [Warmth (Temperature)](#warmth-temperature)

---

![Correction Tab](images/correction/preview.png)

---

## Features

1. **Preview Window:** Displays the working image while edits are applied.
2. **Tool Selection Panel:** Choose which correction tool to use.
3. **Control Panel:**
4. **Apply Changes:** Saves changes for the selected tool only.
5. **Undo Last Change:** Reverts only the last applied modification.

---


## Colors
Adjust the intensity of the RGB components of the working image.

- **Slider range:** `-255` to `+255`  
  - `-255` = remove component completely  
  - `0` = unchanged  
  - `+255` = maximum intensity  

**Usage**
<!-- Colors Table -->
<h3>Colors</h3>
<table>
  <tr>
    <th>Value</th>
    <th>Result</th>
  </tr>
  <tr>
    <td>Original</td>
    <td><img src="images/correction/original.png" width="150"/></td>
  </tr>
  <tr>
    <td><img src="images/correction/col_arg_1.png" width="150"/></td>
    <td><img src="images/correction/col_res_1.png" width="150"/></td>
  </tr>
  <tr>
    <td><img src="images/correction/col_arg_2.png" width="150"/></td>
    <td><img src="images/correction/col_res_2.png" width="150"/></td>
  </tr>
</table>
---

## Brightness
Adjust the brightness of the working image.

- **Slider range:** `-100` to `100`  
  - `-100` = very dark  
  - `0` = unchanged  
  - `100` = very bright  

**Screenshot:**  
![Brightness](images/correction/brightness.png)

---

## Contrast
Adjust the contrast of the working image.

- **Slider range:** `0` to `2`  
  - `0` = no contrast (uniform gray)  
  - `1` = unchanged  
  - `2` = maximum contrast  

**Screenshot:**  
![Contrast](images/correction/contrast.png)

---

## Saturation
Adjust color saturation of the working image.

- **Slider range:** `0` to `2`  
  - `0` = monochrome  
  - `1` = unchanged  
  - `2` = maximum saturation  

**Screenshot:**  
![Saturation](images/correction/saturation.png)

---

## Sharpness
Enhances image sharpness by emphasizing edges (opposite of blur).

- **Slider range:** `1` to `2`  
  - `1` = unchanged  
  - `2` = maximum sharpness  

**Note:** Edges are extracted by subtracting a Gaussian-smoothed version of the image, then blended with the original image to enhance sharpness.

**Screenshot:**  
![Sharpness](images/correction/sharpness.png)

---

## Blur
Applies Gaussian blur to the working image.

- **Slider range:** `0` to `10`  
  - `0` = unchanged  
  - `10` = maximum blur  

**Note:** The standard deviation of the Gaussian filter is set equal to the slider value.

**Screenshot:**  
![Blur](images/correction/blur.png)

---

## Noise Reduction
Removes noise while preserving edges.

- **Slider range:** `0` to `1`  
  - `0` = unchanged  
  - `1` = strong smoothing of fine details, edges preserved  

**Note:** Uses a bilateral filter for edge-preserving smoothing.

**Screenshot:**  
![Noise Reduction](images/correction/noise.png)

---

## Warmth (Temperature)
Adjusts the overall color temperature of the image.

- **Slider range:** `-100` to `100`  
  - Negative = cooler tones (blue)  
  - `0` = unchanged  
  - Positive = warmer tones (red)  

**Note:** The slider increases the red channel and decreases the blue channel accordingly.

**Screenshot:**  
![Warmth](images/correction/warmth.png)
