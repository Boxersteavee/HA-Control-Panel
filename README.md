# Home Assistant Control Panel
This project is for a control panel for Home Assistant, using an ePaper touch display, and an ESP32 control board.

## Model Design
I'm designing this project in onshape, and as it's my first onshape project, I'm also learning how to use it as I go. The design is sort of inspired by the Seeed Studio XIAO 7.5" ePaper display, but is more like a wedge shape, with a fixed display angle of about 50°. 

The design is in one 3D printed part (was two but is now one for simpler assembly). The display will be mounted upside-down with L-shape notches to help line it up. It can be stuck down with some kind of adhesive, double sided tape or hotglue probably would both work. The flex cables can then be connected to the control board/HAT, which can then be stuck to the back of the case with hot glue or double sided tape. There is a notch at the back of the case for a USB cable to feed through, from the USB C port on the control board.

## Parts
This project has 3 main parts:
- Display: 7.5" ePaper touch display from [GoodDisplay](https://buy-lcd.com/products/gdey075t7-t01?VariantsId=10549)
- Control board: ESP32 board and Display driver HAT, included in the display "Demo Kit"
- 3D Printed case, which I am designing through onshape. The model can be viewed [here](https://cad.onshape.com/documents/a9146dbc20244f4e95451b05/w/7d499ee4389c66a144f918b2/e/b62aeb3ed69b79fa7c5cc0ee?renderMode=0&uiState=6a70aafd231415c45910523a), as well as .step files in the [models](models/) folder.

## Assembly
To assemble the project, 3D print the parts from [models](models/). Slot, slot the display into the top half of the housing, attach it with some form of adhesive, connect the display connector and the touch panel connector to the driver board, attach the driver board HAT to the ESP32 board, then stick the control board to the back of the box with double sided tape or hot glue. Plug in a USB C cable into the control board, feed it through the notch in the back of the case then plug in the other end of the cable to a 5V power source.

## Programming
This section of the project is somewhat unknown at this stage. The ESP32 board needs to be flashed with ESPHome - which can be done [here](https://web.esphome.io/), then it can be adopted into Home Assistant. I haven't figured out what needs to be done to program the display yet, however ESPHome does have [documentation](https://esphome.io/components/touchscreen/) for touch displays, and there are tools available to design touch control dashboards such as [this one](https://github.com/koosoli/ESPHomeDesigner).
