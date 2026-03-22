[Back](index.md)

# Charting Tab

The **Charting** tab allows interactive mapping of objects detected in the Detection tab.  
This tab is disabled if no objects have been detected.

---

## Table of Contents

- [Modes](#modes)
  - [Move Mode](#move-mode)
  - [Select Mode](#select-mode)
- [Outline Panel](#outline-panel)
- [Label Panel](#label-panel)
- [Line Panel](#line-panel)

---

![Charting Tab](images/charting/preview.png)

## Features

1. **Preview Window:** Displays the working image with mapped objects.
2. **Control Panel**
3. **Mode Switch:** Toggle between moving the image or selecting objects.
4. **Bake Button:** Rasterizes all map elements into the working image.
     - Locks Detection and Charting tabs for the current image.
5. **Save Button:** Applies baked image. 
6. **Reset Button:** Removes all elements from the map.

---

## Modes

### Move Mode
- Allows the user to **move or scale the image** freely.  
- Supports **zooming** and **panning**.

<table>
  <tr>
    <th>Action</th>
    <th>Result</th>
    <th>Action</th>
    <th>Result</th>
  </tr>
  <tr>
    <td>None</td>
    <td><img src="images/charting/mov_1_1.png"></td>
    <td>Zoom in</td>
    <td><img src="images/charting/mov_2_1.png"></td>
  </tr>
  <tr>
    <td>Pan</td>
    <td><img src="images/charting/mov_1_2.png"></td>
    <td>Zoom out</td>
    <td><img src="images/charting/mov_2_2.png"></td>
  </tr>
</table>

### Select Mode
- Allows the user to **select objects** for further mapping.  
- Clicking inside a green circle selects an object (red circle appears).

<table>
  <tr>
    <td><img src="images/charting/sel_1.png"></td>
    <td><img src="images/charting/sel_2.png"></td>
    <td><img src="images/charting/sel_3.png"></td>
  </tr>
</table>

- Clicking outside any object cancels the previous selection.

---

## Outline Panel

<table>
  <tr><th>Preview</th></tr>
  <tr><td><img src="images/charting/out_preview.png"></td></tr>
</table>

- Each object can have **one outline**.  
- Steps:
  1. Select an object.
  2. Click **Apply** to create or update the outline.
  3. Modify parameters at any time and click **Apply**.
  4. Click **Remove** to delete the outline.

**Parameters**

| Parameter | Description | Range |
|-----------|------------|-------|
| Thickness | Outline line thickness | 1–200 px |
| Radius    | Outline radius | 1–1000 px |
| Color RGB | Outline color | 0–1 per channel |
| Shape     | Outline shape | Circle / Square |

**Usage:**

<table>
  <tr>
    <td>Thickness</td>
    <td><img src="images/charting/out_1_1.png" width="150"></td>
    <td><img src="images/charting/out_2_1.png" width="150"></td>
    <td><img src="images/charting/out_3_1.png" width="150"></td>
  </tr>
  <tr>
    <td>Radius</td>
    <td><img src="images/charting/out_1_2.png" width="150"></td>
    <td><img src="images/charting/out_2_2.png" width="150"></td>
    <td><img src="images/charting/out_3_2.png" width="150"></td>
  </tr>
  <tr>
    <td>Color</td>
    <td><img src="images/charting/out_1_3.png" width="150"></td>
    <td><img src="images/charting/out_2_3.png" width="150"></td>
    <td><img src="images/charting/out_3_3.png" width="150"></td>
  </tr>
  <tr>
    <td>Thickness</td>
    <td><img src="images/charting/out_1_4.png" width="150"></td>
    <td><img src="images/charting/out_2_4.png" width="150"></td>
    <td></td>
  </tr>
</table>

---

## Label Panel

<table>
  <tr><th>Preview</th></tr>
  <tr><td><img src="images/charting/lab_preview.png"></td></tr>
</table>


- Each object can have **one label**.  
- Steps:
  1. Select an object.
  2. Click **Apply** to create or update the label.
  3. Modify parameters at any time and click **Apply**.
  4. Click **Remove** to delete the label.

**Parameters**

| Parameter    | Description | Range |
|--------------|------------|-------|
| Label        | Text | 0–16 characters |
| Text Size    | Font size | 8–128 px |
| Distance     | Distance from object center | 0–1000 px |
| Rotation     | Rotation angle (0° = right, 90° = bottom) | 0–360° |
| Color RGB    | Font color | 0–1 per channel |

**Usage:**

<table>
  <tr>
    <td>Label</td>
    <td><img src="images/charting/lab_1_1.png" width="150"></td>
    <td><img src="images/charting/lab_2_1.png" width="150"></td>
    <td><img src="images/charting/lab_3_1.png" width="150"></td>
  </tr>
  <tr>
    <td>Text Size</td>
    <td><img src="images/charting/lab_1_2.png" width="150"></td>
    <td><img src="images/charting/lab_2_2.png" width="150"></td>
    <td><img src="images/charting/lab_3_2.png" width="150"></td>
  </tr>
  <tr>
    <td>Distance</td>
    <td><img src="images/charting/lab_1_3.png" width="150"></td>
    <td><img src="images/charting/lab_2_3.png" width="150"></td>
    <td><img src="images/charting/lab_3_3.png" width="150"></td>
  </tr>
  <tr>
    <td>Rotation</td>
    <td><img src="images/charting/lab_1_4.png" width="150"></td>
    <td><img src="images/charting/lab_2_4.png" width="150"></td>
    <td><img src="images/charting/lab_3_4.png" width="150"></td>
  </tr>
  <tr>
    <td>Color</td>
    <td><img src="images/charting/lab_1_5.png" width="150"></td>
    <td><img src="images/charting/lab_2_5.png" width="150"></td>
    <td><img src="images/charting/lab_3_5.png" width="150"></td>
  </tr>
</table>

---

## Line Panel

<table>
  <tr><th>Preview</th></tr>
  <tr><td><img src="images/charting/lin_preview.png"></td></tr>
</table>


- Each object can have **many lines**.  
- Steps:
  1. Select the first object.
  2. Click **Select Second Point**, then click another object.
  3. Click **Apply** to create or update the line.
  4. Click **Remove** to delete the line.

Line selection endpoint is marked with **yellow circle**. Same rules apply as for [Select Mode](#select-mode). ***Second object can't be same as the first one***.
<img src="images/charting/lin_sel_1.png"> 

**Status Indicators**
Different indicators mark what state the line is in:

<table>
  <tr>
    <th>Indicator</th>
    <th>Meaning</th>
  </tr>
  <tr>
    <td><img src="images/charting/lin_sel_2.png" alt="red"></td>
    <td>Second object is not selected. Line can neither be created nor modified</td>
  </tr>
  <tr>
    <td><img src="images/charting/lin_sel_3.png" alt="yellow"></td>
    <td>User is selecting the second object</td>
  </tr>
  <tr>
    <td><img src="images/charting/lin_sel_4.png" alt="green"></td>
    <td>Second object is selected. Line can be created or modified.</td>
  </tr>
</table>


**Parameters**

| Parameter | Description | Range |
|-----------|------------|-------|
| Line Width | Thickness | 1–100 px |
| Color RGB  | Line color | 0–1 per channel |

**Usage:**

<table>
  <tr>
    <td>Line Width</td>
    <td><img src="images/charting/lin_1_1.png" width="150"></td>
    <td><img src="images/charting/lin_2_1.png" width="150"></td>
    <td><img src="images/charting/lin_3_1.png" width="150"></td>
  </tr>
  <tr>
    <td>Color</td>
    <td><img src="images/charting/lin_1_2.png" width="150"></td>
    <td><img src="images/charting/lin_2_2.png" width="150"></td>
    <td><img src="images/charting/lin_3_2.png" width="150"></td>
  </tr>
</table>

---

