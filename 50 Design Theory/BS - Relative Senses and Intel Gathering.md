---
title: "BS - Relative Senses and Intel Gathering"
source: "Game Stuff/Game Ideas/BS - Relative Senses and Intel Gathering"
modified: 2013-06-12
type: design-doc
area: design-theory
status: "idea"
projects: []
concepts: ["Design: Sensors and Intel Gathering"]
words: 573
summary: "Design brainstorm of sensor and signature mechanics for a space game: relative signatures, merging, eclipse detection, LOS, triangulation, lock-on."
tags: ["area/design-theory", "type/design-doc"]
---

Brainstorming - Intel Sources/Senses

Infrared and Low light vision in real life is at risk of being "blinded" but fast changes in incoming information.

**Some high tech examples would display the results relative to one another.**

*5 targets emitting the same infrared signature move into sensor range. One ignites its afterburners. Its signature increases by just 10% while the others recrease by the same amount.*

Friendlies could be "cloaked" by increasing your own signature to overcome the sensors of your enemies.

*One of the 5 targets activates an EWAR system that increases its signature by 1000%. The other 4 activate ECM which decrease its signature by 90%. These now seem to be 1000x smaller, well below the defenders sensor resolution.*

**Signatures might add together or be "swallowed up" by the larger**

*One signature has a radius of 100m. Another is 80m away and has a signature of 10m. Since the smaller signature is totally inside the larger, it doesnt even register. Distance+Sig1 \< Sig2*

When inside one another, signatures could add together, breaking apart when they actually separate enough.

*In the example above only one signature of 110m is seen. Once the smaller moves more than 90m away from the larger, two separate signatures are seen.*

**Some sensors might only detect objects that are eclipsing another object (visual or infrared)**

*A group of targets with plasma drives burning flying in front of a star might actually seems to dissapear, while a ship emitting no heat in stealth mode will show up like a black spot against a white background!*

Sometimes objects can stay hidden if they only move against the background of deep space.

Taking a non direct path would allow the stealth mode ship above to sneak up on most ships

**Some sensors are blocked by the objects they are detecting (line of sight) while others have an area effect**

*A gravametric sensor would detect the mass of objects with accuracy falling off the farther away the detected object is. Another object behind an objstacle will still be detected.*

*Infrared and Visual spectrums could be blocked by flying behind an asteroid*

Even this can be blocked or evaded. Every system has its downside.

*The ship flying behind a really large asteroid would have its gravametric signature swallowed up by the asteroid. Close inspection would show if the ship had moved away, but where it will emerge is impossible to tell.*

*At long range, gravametric sensors become inaccurate so all but the largest signatures fail to appear.*

**Some systems rely on triangulation**

Visual sensors can find an object easily but cannot show if it is a small object close up or a large object farther away. Radar/Ladar can only detect distance to the object but not exactly where it is.

When certain sensors are used in paralel the speed of an object can be detected using doppler.

**Some sensors have limited directional arcs or can only track single objects at a time**

LADAR/RADAR only work efficency when use directionally.

Hyperspace tracking requires expensive equipment and can only track very few targets at a time.

**Using several systems can allow a "lock on" effect**

If enough sensors are focused on one target then a computer can be used to calculate its position from now on with minimal sensor focus. This can be broken if a threshold is reached, at which point the sensors must be trained to allow lock on to be acheived again.
