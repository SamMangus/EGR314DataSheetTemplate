---
title: Course Reflection
---

## Review of Module's Success

Overall my module was successful in the majority of what it set out to do, I was able to send and receive data, forward messages and communicate with our control board who would forward the information to our HMI so it could be displayed to the user. The part where I fell short was keeping everything surface mount on my PCB due to some oversights while designing.

## Module Startup Tips

-Breadboard your design ASAP
-Check the data sheets of every component to make sure you're utilizing them properly
-Have backup plans for power supply
-Test your PCB part by part don't solder everything at once then test
-Coordinate with teammates frequently

## Lessons Learned

1. Stay ahead of schedule the farther you fall behind the harder it is catch up.
2. Coordinate with your teammates frequently your success heavily relies on your team working together.
3. Build your design on a bread board first before you take it to the PCB to avoid later errors.
4. Make sure your voltage regulator meets the shared power needs and have backup options to supply your microcontroller with power in case something is wrong with the team's shared connection.
5. The teams project should be able to function without one person's subsystem so make sure the design is rugged and not reliant on one person for the rest to function.
6. Print your PCB out on a piece of paper and lay your components out ahead of time to make sure your footprints are correct before submitting it for manufacturing.
7. Choose your microcontroller carefully make sure all the peripherals you need are available for the communication type you're using and not interfering with other functions such as the MCLR and other pins needed for programming the pic.
8. Order extra parts for your PCB you will more than likely mess something up and need to resolder components and the more time you waste waiting for more parts to arrive the less time you will have to debug and test
9. Work with your teammates on the code to make sure you guys are you using the same standard and will be able to properly parse messages and forward them if you can't communicate the functionality of your systems there are limited ways to prove it's working as intended
10. Ask for help from the TA's or Dr.Nichols, we're learning as we go and you will likely make mistakes it's important to have someone double check your work especially someone who has more experience than you it will save you a lot of time down the road.

## Recommendations For Future Students

1. Learn/review coding whether it's C, C++, Python this course requires a substantial amount of coding so making sure your knowledge is as good is it can be prior to taking this course it will save you a lot of time.
2. Be prepared to be challenged you will need to learn a lot of new information and be expected to apply it while coordinating with your team but it's okay to feel like you're struggling and you shouldn't feel discouraged because of it.
3. Being able to work well with your team is just as important as any technical skills you may have, your project heavily relies on how well you and your team coordinate.
4. While designing your PCB make sure you have fail safes you need to have measures in place to make sure your design will still function should something go wrong for example emergency jumper holes or a way to bring in external power to your microcontroller should your regulator stop working
5. Be willing to learn and ask questions there will be points where you get stuck and won't know how to proceed with your project so be willing to ask for help from the teaching staff they are there to help you and it is a very valuable resource you should be taking advantage of.