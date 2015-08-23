PerlinNim [![Build Status](https://travis-ci.org/Nycto/PerlinNim.svg?branch=master)](https://travis-ci.org/Nycto/PerlinNim)
===========

A small perlin noise generation library for Nim.

![](http://nycto.github.io/PerlinNim/example.png)

API Docs
--------

http://nycto.github.io/PerlinNim/perlin.html

A Small Example
---------------

```nimrod
import perlin, math

# Call randomize from the 'math' module to ensure the seed is unique
randomize()

let noise = newNoise()

# Output a 20x10 grid of noise
for y in 0..10:
    for x in 0..20:
        let value = noise.perlin(x, y, 0)
        stdout.write( int(9 * value) )
    stdout.write("\n")
```

License
-------

This library is released under the MIT License, which is pretty spiffy. You
should have received a copy of the MIT License along with this program. If
not, see http://www.opensource.org/licenses/mit-license.php


