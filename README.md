# sierpinski-tree

A modular PCB Christmas Tree, using WS2812 LEDs. Designed in [EasyEDA](https://easyeda.com/) and manufactured by [JLCPCB](https://jlcpcb.com/).

![gif](https://github.com/lycarter/sierpinski-tree/blob/main/sierpinski_tree.gif)

Due to COVID, I'll be spending the holidays in my NYC apartment for the first time instead of traveling home. While unfortunate, that means I get to come up with some creative ideas for Christmas decorations. Resources for making things in a 400 sf studio apartment are essentially limited to 3D printing and soldering so I decided to make an apartment-sized tech-y Christmas tree. One of the critical requirements is that whatever I made needed to be compact enough to reasonably store and travel with later, so making something modular seemed like a good approach. The idea struck me to design a PCB that would represent a single unit of a Sierpinski Triangle so that I could tesselate together many identical boards to make a tree of any size.

I started by drawing a snow-covered Christmas Tree in [Inkscape](https://inkscape.org/), then imported that SVG into [EasyEDA](https://easyeda.com/). I've used other EDA software in the past, but EasyEDA's approach to user-driven libraries, and integration with [LCSC](https://lcsc.com/) has made it my go-to for simple projects like this. I elected to use 3 [WS2812b-mini](https://lcsc.com/product-detail/Light-Emitting-Diodes-LED_Worldsemi-WS2812B-Mini_C527089.html) addressable RGB LEDs per board, and connect each board at the corners with 3-position pin headers. I planned to drive the whole assembly from an external Arduino, which I knew could drive WS2812 chains of a pretty reasonable length without any issue. For the first pass, I ordered 10 boards with the goal of making a 9-member Sierpinski triangle. The next logical step up is 27 members, which was a bit more than I planned to commit to, and might be a bit too large for my apartment. As a final touch, I added a small hole to the top so that the board could be hung like an ornament, in the event that I send these boards to friends and family.

Check out my blog post for more: https://www.lycarter.com/2020-11-29/xmas-decorations

Also on [Hackaday](https://hackaday.com/2020/12/04/sierpinski-pcb-christmas-tree/)
