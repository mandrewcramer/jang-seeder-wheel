# Parametric Seed Roller

This is an edit from the work of Fordi and Fernplant. Fixted text box placement, changed solid body wheel to sunken text, and added text of each preset to the JSON. The following is from Fordi:

This is a parametric seed roller with default parameters and presets for Jang JP or JPH series rollers.

<img src="https://github.com/Fordi/jang-seeder-wheel/raw/main/Jang_F-12_PLA_Orange.jpg" width="320" alt="Jang F-12 sample print" />

You can adjust things like the diameter and borehole to adjust for your printer's tolerances. You can also adjust the number of seed cells and their size.

I started from an existing Jang wheel, took measurements, and implemented a fully parameterized version out of shape primitives.  Then [fernplant](https://github.com/fernplant) was nice enough to add other shapes.

The renders of every roller preset are available [on Thingiverse](https://www.thingiverse.com/thing:4462838).

# Usage

Running this command will open up OpenSCAD.  If you open up the Customizer, you'll see a bunch of presets for known Jang seed rollers.

```
openscad seed_roller.scad
```

The following command will render the preset "Jang M-12" as "Jang M-12.stl":

```bash
./render.sh "Jang M-12"
```

To list all the presets:

```bash
./render.sh list
```

The current set of supported rollers are:

```
Jang A-6
Jang AA-6
Jang B-12
Jang BL-12
Jang C-12
Jang C-6
Jang F-12
Jang F-24
Jang F-6
Jang G-12
Jang G-6
Jang J-2
Jang J-4
Jang J-8
Jang L J-12
Jang L J-24
Jang L J-6
Jang L V-12
Jang L V-24
Jang L-12
Jang L-24
Jang MJ-12
Jang MJ-24
Jang MJ-4
Jang MJ-6
Jang MM-12
Jang MM-24
Jang N-6
Jang Q-12
Jang Q-6
Jang R-12
Jang R-24
Jang X-12
Jang X-24
Jang X-4
Jang X-6
Jang XY-12
Jang XY-24
Jang XY-36
Jang XY-4
Jang XYY-12
Jang XYY-24
Jang XYY-36
Jang YX-12
Jang YX-24
Jang YX-4
Jang YX-6
Jang YYJ-12
Jang YYJ-24
Jang YYJ-6
Jang YYX-12
Jang YYX-24
Jang YYX-36
Jang Z-Blank
```

To render all the presets into `./stl/`.

```bash
./render.sh all
```

> Note: there are 52 Jang wheels, and they each take 2-3 minutes to render.  You're looking at about 2 hours of rendering.

