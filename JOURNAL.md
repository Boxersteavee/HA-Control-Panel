# Planning
<small>Date formats are in DD-MM-YYYY because yes.</small>

## 27.07.2026
I've done some starting research for some eInk/ePaper capacitive displays and found some from "good-display.com". They have a 4.2", 4.26" (in a phone-like aspect ratio) and a 7.5". I'll probably end up using the 7.5" as it's a decent enough size, however to get the ESP32 kit (Display, Cables, Display Driver which includes an ESP32 module), it costs $65.10 (as I'm only buying one) + $14.78 for shipping. On AliExpress, this is £53.54 + £5.51 shipping (delivery mid-august... I'm running out of time for this!!!)

This seems like it'll be the best option, I just need to plan a bit more first:
- Figure out how this could interface with ESPHome (only having to work with YAML would be nice)
- Design and print an enclosure for this thing

### Parts (so far)
#### Display Options
- Good Display 7.5" Capacitive 800x480 E-Ink display including ESP32 HAT - [Store Link](https://buy-lcd.com/products/gdey075t7-t01?VariantsId=10549) - [Buy Link (Ali-Express)](https://www.aliexpress.com/item/1005002870223620.html)


Well that's it for today... It's getting late and I have things to do... I've got a good start on research though! I'll think of some model designs... some other time this week.

## 03.08.2026
Time to learn onshape... And figure out how to design this thing...

There's dimensions listed for the display itself on its store page (listed above), however I can't find any diagrams for the ESP32 control board... so this is gonna be a bunch of guess work and then eventually dealing with it when I get the thing...... Or just have a flat space underneath and put double-sided tape under there to stick it down... That'll do

So I need a place for the USB C port, and the power switch, and then the cables to the control board go from there... If they're too short, I'll need cable extensions, and the power switch will just always be on... That might work better actually.

The design I think is going to be 2 parts, the bottom half where the board sits, and the top half where the display lives - at an angle probably too (maybe? Is that harder to design? I'll see...)
Or maybe a bottom cover that comes off to reveal everything. With either clips or screw-holes to fit it together.

I better be able to control this thing... ESPHome supports touch displays right?

Well [that](https://esphome.io/components/touchscreen/) looks complicated, but yes it does.... FUTURE ME PROBLEM!!!

Okay so the design needs a bottom cover, and then a way for that to attach and detach... screws? Clips might not be flexible enough with my filament... idk

Hmm, screws means I need to tap it, and I don't think I have any tapping tools... I suppose I should try clips...

Restarting the design bit- Gonna do a wedge-shape from the right side, the front will have a hole.... noooooo clue how the display is gonna mount yet.... or where the control board is going.

Done a lot more work on the design, got the shape about right, just need to sort the display mounting area and also the heat-insert holes for the screw mounts...
If only I didn't accidentally leave the timelapse paused for OVER AN HOUR meaning i'm getting credited for 1hr 37 when I have been working on this for about 2hr 40 or more. Well, future me problem I suppose..... AAHHHHHH >:(

## 04.08.2026
Okay I've started working on the mounting mechanism for the top of the display and had a wild idea: Scrap having a bottom cover, just flip the display upside-down (since my top bezel is too big anyway), attach the control board to the back half of the top panel, and feed the USB cable out the back of the board... no need for a bottom cover, no need for screws or heat-seat inserts!! (I was worried about assembly, I haven't used a soldering iron in a while... and I don't want my Dad to be backseat soldering again 🙄)

Yup, done the design, for now... The display will be mounted upside down, there's little L-shape notches for it to sit in place. I've made a little cut out for the USB cable to fit through, so I just need to wait for parts, print this, and see how it goes... I hope it's not too light to the point it can't sit stable on its own... Some heavy weights could help fix that though. Files are all on github, funding submitted. It GO TIME!