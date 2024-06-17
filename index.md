# Ball Tracking Robot with OpenCV: Computer Vision

This project is about making a ball-tracking robot using OpenCV, a Python library for computer vision. The robot has a Raspberry Pi computer, a PiCamera for detecting the ball, DC motors for moving the wheels, and ultrasonic sensors to avoid collisions. Each part works together to create a robot that can follow a ball.

<!---
You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:

<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site 
-->

|**Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Dhruva J. | Cupertino HS | Computer Science | Incoming Junior |

<!---
**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
-->


# Final Milestone

## Summary
My final milestone is to make the robot turn after detecting the red ball, then move to the red ball. This would be possible by sending the angle needed to turn the robot from the the Raspberry Pi to the motors. After that, the robot would move forward until the ball is directly in front of it.

<!---
**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE
-->

# Second Milestone

## Summary
My goal for this milestone was for the robot's camera to detect the red ball. This would be possible by taking a image from the robots camera and finding the largest area of red pixels. This was done by using OpenCV which is a python library. My code would see if there was a area of red pixels which was greater than 400. If so, then that would be the ball. If not, then that would not be the ball. The robot cannot be able to detect the ball if it was too far away since the area of red pixels would be less than 400.


<!---
**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VAmNlER5Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone 
-->

# First Milestone

## Summary
My first milestone is to construct the overall build for the robot. I constructed the chassy and attached the battery pack, Raspberry pi, camera, breadboard, and infared sensors to it. I had to wire electrical components together for exampel, wiring the breadboard to the raspberry pi and connecting the h-bridge to the motors. I also had to solder some wires together because the slot would only allow one wire and I had to connect two wires.

## Components Used
- 1x Raspberry Pi Minicomputer
- 1x H-Bridge
- 1x Robot Chassy
- 3x Resistor (1k Ohm)
- 2x DC Motors 
- 1x Battery Pack
- 1x Breadboard
- 3x Ultrasonic Sensor
- 1x PiCamera
- 20x Wires
- 2x Wheels

## Challenges Faced
One of the main challenges that I faced when building the overall build was managing my wires. Since I was using so many wires, there would be a lot of unorganized messy wires everywhere. I decided to use zipties to group wires that led to the same place. I also realised that the Raspberry Pi's case had a little gap at the top, this was helpful because I could fit wires through there, making it easier to organize my wires. Another challenge that I faced was assembling the chassy. This was because the screws were very hard to install because there was not enough space which required me to take apart everything and re install them. I also had some challenges with installing the PiCamera because I forced it into the slot on the Pi's motherboard instead of lifiting the tabs and carefully placing them in resulting in the holder for the camera chipping away and causing a loose connection. I fixed this by placing the camera in correctly by lifiting the tabs, and it worked when I tested it again.   
<!---
**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/CaCazFBhYKs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your first milestone, describe what your project is and how you plan to build it. You can include:
- An explanation about the different components of your project and how they will all integrate together
- Technical progress you've made so far
- Challenges you're facing and solving in your future milestones
- What your plan is to complete your project
-->


# Schematics 
<!---
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

-->
![image](https://github.com/djoglekar893/Dhruva_BlueStampPortfolio/assets/155853576/3f27e7b8-454a-40a6-b50a-874711f114eb)


# Code


```python
 import cv2
        
      
```

# Bill of Materials

| **Part**            | **Use**                   | **Price** | **Link**                                                                                                                                    |
|:-------------------:|:--------------------------:|:---------:|:------------------------------------------------------------------------------------------------------------------------------------------:|
| Raspberry Pi        | Building the Raspberry Pi  | $99.95    | [Link](https://www.canakit.com/raspberry-pi-4-starter-kit.html)                                                                            |
| Emonzy Chassis      | The base for the vehicle   | $12.99    | [Link](https://www.amazon.com/Smart-Chassis-Motors-Encoder-Battery/dp/B01LXY7CM3/ref=asc_df_B01LXY7CM3/?tag=hyprod-20&linkCode=df0&hvadid=693448563566&hvpos=&hvnetw=g&hvrand=13188769298549160467&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9032183&hvtargid=pla-584495246069&psc=1&mcid=3f54405bf4d93ae384d78ef10f75b962&gad_source=1) |
| Power Bank BI-B41   | Powering the Raspberry Pi  | $19.99    | [Link](https://iniushop.com/products/iniu-b41-portable-charger-15w-fast-charging-slimmest-10000mah?variant=43637931147442&currency=USD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic&gad_source=1&gclid=CjwKCAjwjqWzBhAqEiwAQmtgT1XwMCJbZkhMTRSuZs4hHaQyGw7Jys7nqwnwtI10GClJyrz8Do8syxoCC0AQAvD_BwE) |
| Breadboard | Connecting the electrical circuits | $2.33 | [Link](https://www.amazon.com/ELEGOO-tie-points-breadboard-Arduino-Jumper/dp/B01EV640I6/ref=sr_1_3?crid=1B2OOFCZPLH09&dib=eyJ2IjoiMSJ9.c3AY57g3DJYx1mV7GL3Z2BI7VibPC8inlAG7IgmFmBylQ1IYt_Q8-A2F8NYW2VoP8zxEXvFyPX4v8cE_nDBNctifJt4txhQ_3ee7GJ_JPAfhix9ISztD_Flaob8teY24RDocApew_6ggjXw-6TapCa6RKIFjgk2YDJCVZC_oqui-dnrQ7bmOb-QMemrgLq9K-NNIbeOwuG3U1KKIKwpq0_8Ng45zZBz_hMuiasUIUgI.diGqVHf1K4w9nydJ8Bc3Dfvz_GEmWAN_Yd6s-8IDG2o&dib_tag=se&keywords=half+breadboard&qid=1718304133&sprefix=half+breadboard%2Caps%2C126&sr=8-3) |

<!---
# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
-->

# Starter Project - Calculator 

<iframe width="560" height="315" src="https://www.youtube.com/embed/JeRtqHQ6S8k?si=xQgf9Ill7YbIALUa" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Summary
For my starter project, I created a functional calculator. The calculator was able to perform simple action such as adding, subtracting, multiplying, and dividing two numbers. It could also deal with decimals and scientific notification if a number was too large or small to fit in its 6 digit screen. When you press the buttons on the calculator, it sends a packet to the main computer of the calculator which would perform the operation. Finally, the computer will print the final answer on its six digit screen.

## Components Used
- 1x 
- 1x Raspberry Pi minicomputer 
- 1x Usb Socket
- 1x Resistor
- 17x Push Down Buttons 
- 17x Button Caps

## Challenges Faced
Some challenges I faced, include adding the case to my calculator. The screws were pretty hard to tighten and my case was loose which forced me to restart making it. Another challenge I faced was that my resistor went too tall so I had to bend it in order to make it fit in the case. I also had some challenges with soldering because the pins were too close to eachother and one wrong move would make it not work.
