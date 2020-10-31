# XOR Texture
```
float xor(vec2 p){
    float r = 0.;
	for (float i = 1.; i <= 32.; ++i) {
        p = floor(p/2.),
	r += mod(p.x+p.y, 2.) * exp2(i);
	}
    return r;
}
```
From [a comment in this Shadertoy](https://www.shadertoy.com/view/ltsGzN)

<img src="credit.png"></img>
