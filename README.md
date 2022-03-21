# List of hobby projects
Very incomplete, but these are the most fun to play with. I will likely continuously update this list with fancier gifs and more thrilling descriptions.

### What I'm currently working on
* Crypto research
* Figuring out how to leverage fractals to make games without it being gimmicky
* Procedural sound fiddlings

## Game prototypes (all in Pico-8)
### ❤️ Material Girl ❤️
![material_girl p8](https://user-images.githubusercontent.com/39782/159227267-e9732b5c-78aa-401a-a8a8-12e3e397bf11.png)

My first end-to-end prototype that goes from intro to ending sequence. This is based on an idea I had about representing getting close to people via dating as JRPG-style combat where you have to figure out and manage metrics that are only indirectly measurable through your "opponent"s words and actions. Conquer all the boys and stock up on accessories to land your dream beach hunk 💅🏖️💞 Lots of fun with promise-driven tween chains in this one.

[play](https://jcwilk.github.io/material_girl) [discuss](https://www.lexaloffle.com/bbs/?pid=39675&tid=29166) [source](https://github.com/jcwilk/material_girl/blob/master/material_girl.p8)

### 🙈 Anx 🙈
![anx p8](https://user-images.githubusercontent.com/39782/159228458-f87d88d7-8596-496c-8362-94cfed732df8.png)

A prototype about the terror of other people as we go about the tedium of our day. This was basically an excuse to implement a (sloppy) 3d engine on top of a 2d engine (pico-8). Because it's so horribly inefficient I had to implement some kind of interesting lossy optimizations, it basically skips rendering certain columns of pixels and renders the other ones nearby as wider to fill in the gaps which leads to a somewhat pleasing shimmering effect when things get too busy in a certain part of the screen. Social stress leads to panic attacks, pixel deconstruction, and fisheye effects. Side effects of demons may occur.

[play/discuss](https://www.lexaloffle.com/bbs/?pid=42366&tid=29630) [source](https://github.com/jcwilk/anx/blob/master/anx.p8)

### 🚙 Traffic World 🚗
![traffic_world p8](https://user-images.githubusercontent.com/39782/159228213-c1349d9f-7fd1-41b7-a345-d0222b870105.png)

A quick protoype towards an idea I had about a world that was entirely covered by roads without destinations, just traffic all the time. As we all know though, traffic can be influenced by causing accidents which can be a very effective way of deterring police from interfering with your progress. They tend to respond quickly and firmly to transgression though...

[play/discuss](https://www.lexaloffle.com/bbs/?pid=59847#p) [source](https://github.com/jcwilk/traffic_world/blob/master/traffic_world.p8)

## Fractal experiments
### Mandel1 (pico-8)
![mandel1 p8](https://user-images.githubusercontent.com/39782/159228732-b464f1c0-03f2-4c96-ae57-aea1c830a72b.png)

My first foray into mandelbrot generators. This one is pretty straightforward but it has a fun tile-based continuous rendering method you can see below.

![mandel1_0](https://user-images.githubusercontent.com/39782/159221534-62b12cfe-13b0-4eb1-ba33-48d998fc1d84.gif)

[play](https://jcwilk.github.io/mandel1/) [writeup](https://jcwilk.com/mandelbrot-explorer-in-pico-8/) [source](https://github.com/jcwilk/mandel1/blob/master/mandel1.p8)

### Mandel2 (webgl)
My first webgl project. Turns out graphics cards are really good at calculating mandelbrot sets! This one renders a fixed iteration limit and allows you to wander around and zoom.

[play](https://jcwilk.github.io/mandel2) [source](https://github.com/jcwilk/mandel2/blob/master/mandel2.js)

### Mandel3 (pico-8)
![mandel3 p8](https://user-images.githubusercontent.com/39782/159229838-3ddb43ae-1d98-4042-959e-b41fe11b435d.png)

Time to get weird. This takes a bastardized version of the 3d-ish renderer from Anx to see the mandelbrot set growing out of the ground in 3d. It's pretty rough around the edges and you have to really work for it to get any particularly thrilling vistas, but still a reasonably pleasant hellscape to exist in for some time.

[play](https://jcwilk.github.io/mandel3) [source](https://github.com/jcwilk/mandel3/blob/master/mandel3.p8)

### Mandel4 (webgl)
An expansion of Mandel2, this time with continuous iteration. While moving it stays fixed but while stationary it continues iterating nearly endlessly. Very pleasing to find a deep spiral to let it churn through for a few minutes, and fun source material for making gif loops too. It keeps updating the URL to be your current position so it's easy to share your favorite spots just by copying from the URL bar.

[![mandel4_zoom_loop](https://user-images.githubusercontent.com/39782/159221416-f011a2eb-9b13-4a5c-884b-21d152af6320.gif)](https://jcwilk.github.io/mandel4/?x=-1.3998553800531095&y=0&z=1254.8361126647887)

[play](https://jcwilk.github.io/mandel4) [source](https://github.com/jcwilk/mandel4/blob/master/src/index.ts)
