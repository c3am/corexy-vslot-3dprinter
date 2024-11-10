# corexy vslot 3d-printer
This 3d printer design is supposed to be a fully free and open source cheap and reliable printer
that is easy to build and easy to source parts for.
Also, it is supposed to have a decent print quality and speed and support higher temperature
filaments like ABS.

Why is this project important?
because the 3d printer is the optimal rapid prototyping tool and thereby necessary for further
open source development.
This is not just supposed to be a fun to build hobbyist project but a capable and reliable tool,
which is to be improved further by everyone who uses it and has improvement ideas.

## design requirements

The following are the requirements that the printer shall fulfill.

1. compatible with PLA, PETG and ABS
2. fast while good print quality
3. portable/compact
4. cheap
5. easy to build, maintain and modify
6. reliable/robust

## design decisions
- 2020 extrusions
This printer uses 20*20mm aluminium v-slot extrusions because they are cheap and versitile.
They allow you to mount anything to them easilly with T-nuts and can be solidly
connected to each other using blind joints.
One downside though is that for a straight connection they need to be cut very precisely at a 90deg angle.

- enclosure
an enclosure is necessary for printing ABS without warping (design requirement 1)

- corexy motion system
In a corexy motion system the motors do not move which reduces the moving mass.
This enables higher accelerations as moving mass creates ringing effects which would degrade
the print quality meaning a higher print speed can be achieved (see design requirement 2).

- v-wheels
V-wheels are cheaper than linear rails (see design requirement 4).

- bed is supported on 4 corners
This ensures that the bed is moving perpendicular to the xy-plane of the motion
system reliably (see design requirement 6).

- 1 stepper for z
This not only saves on stepper motor costs but also enables the use of mainboards
with only 4 stepper drivers which are cheaper.

- minimal toolhead
because the voron stealthburner toolhead is too big and the mini stealthburner doesn't have
good enough cooling and the dragonburner requires a seperat (expensive) extruder,
I designed my own toolhead.

- frame corners
aluminium extrusions can twist when tightening down blind joints which can be prevented
by 3d printed corner pieces which also protect the enclosure panels.
This makes the build easier and improves portability and robustness (see design requirements 3 and 6).

- stationary gantry
the xy-gantry is stationary as this is more compact than a flying gantry (see design requirement 3)

## build instructions
