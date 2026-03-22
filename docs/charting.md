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
