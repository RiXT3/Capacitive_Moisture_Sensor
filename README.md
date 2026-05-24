This project includes DXF drawings for the probes used in a capacitive soil moisture sensor. 

The provided designs can be integrated into your own project to enable soil moisture detection.

# How does it work:
A constant PWM signal is applied to the probe. 
Pads P1 and P2 form an RC low-pass filter, whose characteristics vary depending on the soil moisture level. 
Changes in ground moisture alter the filter response.

<img width="981" height="450" alt="obraz" src="https://github.com/user-attachments/assets/ca77900f-c696-4e1e-8b8a-1fa836abab13" />

- Channel_2 = probe P1 

- Channel_1 = A0 output 

<img width="1270" height="594" alt="ezgif-3d75c32dca41f8db" src="https://github.com/user-attachments/assets/f11556fd-3d0a-4431-9da5-57f38523edbb" />

**The sensor was dipped into and removed from a glass of water**


## Adding DXF file
**In your PCB editor, use the Import DXF option to load provided file.**
- Set the sensor electrodes areas as fill regions / copper pours
- Set the sensor outline layer as the **board outline**
  
(Connecting traces to the sensor pads may require manually assigning or editing the net names)

# Use example: 
Example used here shows solar powered moisture sensor with 433Mhz communication
<img width="989" height="587" alt="595664335-68c4386d-8e84-4c4e-9ee1-ce0fb8b08ed3" src="https://github.com/user-attachments/assets/f4c4430e-3423-4fd4-af38-f6b1cd05bb3d" />

## Do not add ground plane under sensor area
