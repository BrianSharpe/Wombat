Wombat
An efficient texture-free GLSL procedural noise library
Source: https://github.com/BrianSharpe/Wombat
Derived from: https://github.com/BrianSharpe/GPU-Noise-Lib

I'm not one for copyrights.  Use the code however you wish.
All I ask is that credit be given back to the blog or myself when appropriate.
And also to let me know if you come up with any changes, improvements, thoughts or interesting uses for this stuff. :)
Thanks!

Brian Sharpe
brisharpe CIRCLE_A yahoo DOT com
http://briansharpe.wordpress.com
https://github.com/BrianSharpe


Wombat
===

Wombat is a set of standalone GLSL procedural noise functions.
By standalone we mean it requires no texture sampling or use of any other GPU resources ( other than registers and clock cycles )
It is ideal for use in cases when texture resources are scarce or when only GLSL code by itself can be provided for shading.

Efficiency has been a primary goal which means aggressive optimization has been applied wherever possible.
Attempts have been made to provide for each noise a matching version which also computes analytical derivatives.
The noises have been written to have a consistent set of behaviors to facilitate interoperable use.
eg
- Frequency of 1.0
- C2 continuous ( where applicable )
- Analytically defined strict output range of either 0.0->1.0 or -1.0->1.0



