Software engineer with 15 years experience in backend systems, API design, and AI tooling.

Currently: Learning functional languages, exploring and contributing to [Goose](https://github.com/block/goose), and generally building and exploring AI agent tools in this new crazy era.

Previously: Tech lead at Doximity, CTO at Gimmie, Principal Engineer at ReferralCandy, games engineer.

## Recent Work
- [Tree Driven Interaction](https://github.com/jcwilk/tdi) - AI chat client with tree-oriented conversational navigation
- [simplekiq](https://github.com/doximity/simplekiq) - Open source sidekiq workflow orchestration library
- Pico-8 game dev, fractal visualizations, AI automation tools

# List of hobby projects
Very incomplete, but these are the most fun to play with. I will likely continuously update this list with fancier gifs and more thrilling descriptions.

## Game prototypes (all in pico-8)
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

### Mandel5 (pico-8)
![mandel5 p8](https://user-images.githubusercontent.com/39782/159668858-00d73aad-cd84-4162-acb9-d5cbc421e73b.png)

I was curious about how to make multiple mandelbrot sets "collide" with each other, or how one might be able to link together many mandelbrot sets into a fractal field of sorts. This went through a lot of iterations. I started out trying to do a universal-law-of-gravity-inspired approach where each mandelbrot origin would all tug on orbits as they happened and with a lot of fudging I could get interesting results, but it didn't feel right because it was bastardizing how fractals work and the emergent shapes were too directly resultant from the arbitrary limits my code was imposing. Instead, eventually I settled on an interesting approach where it keeps track of a number of orbit possibilities and keeps testing them all as they fork and lead to new possibilities. The longest lasting hypothetical path ends up being the one counted. This leads to satisfyingly nuanced interactions between mandelbrot sets that are a good distance from each other. Below is a gif of moving one of three mandels back and forth, and then zooming in on the nuance of an overlap to see how it changes as the mandel continues to shift.

![mandel5_1](https://user-images.githubusercontent.com/39782/159233775-bef88e64-6d37-4208-9163-c4ac8170c1fe.gif)

Update: the difference between tracking only the orbit closest to its nearest origin vs tracking a pool of orbits for each iteration was pretty negligible, but there's a pretty huge difference in performance so I just set it to only track one orbit for now. Turns out another important thing was raising the max orbit range to be larger, still figuring out what the right size of it should be... Seems like somewhere around large enough to encompass the whole area of objects is ideal but scaling individual mandels up and down throws a bit of a wrench in that. Tried adjusting the max orbit range for each mandel but having too tight a range is just ugly and very unfractal-like. As-is it's coming together nicely, nearby fractals can be seen in the details of their neighbors sort of like a hall of mirrors. There's definitely some potential here for a really mind-bending game universe.

![mandel5_6](https://user-images.githubusercontent.com/39782/159674754-f6a8cbe2-efc5-4f8b-b0e4-388fb19af324.gif)

[play](https://jcwilk.github.io/mandel5) [source](https://github.com/jcwilk/mandel5/blob/master/mandel5.p8)

### Mandel6 (webgl)
Basically a realtime/hires upgrade of Mandel5 into webgl, plus extra interactivity bonuses. You can click or tap and hold to create new mandels wherever you want and drag them around as they grow to see how it makes things shift. Once you release the pointer it'll freeze in that spot until you reload the page. Currently zooming in and making very small mandels is a bit buggy, but buggy fractals can be interesting too ;)

![Screenshot from 2022-04-02 16-16-14](https://user-images.githubusercontent.com/39782/161404548-bf70c5ad-1edf-4069-8da7-6889ae6a411a.png)

[play](https://jcwilk.github.io/mandel6) [source](https://github.com/jcwilk/mandel4/blob/master/src/index.ts)
