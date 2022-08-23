# Generating Thermal Gas Images with Blender on Colab

Through installing **Blender 3.2** on a **Python Notebook**, we can use **Colab's GPU** to render large amounts of 128x128 pixel thermal gas images (with a *transparent background*). 

The Python notebook **render_gas.ipynb** will control the whole process, and after being uploaded to Google Colab it can store all of its data on Google's servers.

![enter image description here](https://github.com/max-wild/gas_rendering/raw/main/example.png)

## Steps
To generate 128x128 pixel thermal images of gas:

 1. Download render_gas.ipynb and open it in Google Colab
 2. Update the Python parameters at the top (output directory and amount of gas renders) if necessary
 3. Ensure that Colab's GPU is enabled by going to "Edit" -> "Notebook settings" at the top and setting "Hardware accelerator" to GPU
 4. At the top, go to "Runtime" and select "Run all"

## Background

Thermal images of **gas** can't be simulated in the same way that standard images of **smoke** can, because gas is typically more wispy and less defined. 

The blender file used in this project fixes this issue by using parameters to make the smoke-material **more "gas-like"**. In every render, it also randomizes the gas' position, direction, and behavior, to generate new images every four renders. The color also changes ranging from darker grey to a lighter white.

This rendering includes effects such as wind, turbulence, vorticity, and heat interaction to generate more realistic gas behavior.

## Customize the Output

By default, the renders will be saved to your google drive account. In the Python journal, you have the option to change the **output directory** and **number of renders**--change this in the first cell.

<br>

Thanks!   

Max
