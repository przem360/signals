# SIGNALS

Pure Data patch for creating soundscapes with samples and generative melodies. It contains:

  - Oscilators and ADSR
  - Random note generator
  - Noise generators
  - "Sampler" (it's more like looper for now)
  - Mixer with reverb
  - writesf object to record performance

## Example track

This is sample track made only with this patch and samples (included in repository).

[Listen on Bandcamp](https://distortiongain.bandcamp.com/track/signals-nocturne-for-pure-data).

## How it works

If you turn on module but not hearing any sound - check sliders in `subs/mixer`.

Clone or download this repository and open **signals.pd**. Click the first bang object, open `subs/theosc` and increse the volume of oscilator. Open `subs/osc2` and increase both sliders. Goto to `subs/mixer` and turn on firs two channels and master slider. In **signals.pd** toggle on the `subs/noiser`. If you need more noise open `subs/rndnoise` and click the main bang object.

In `subs/sampler` you can load your samples, playback them at full, half or quarter speed. Just click the first, topmost bang object to load wave file and turn on the volume. Playback should start. Don't change values of horizontal sliders in `subs/sampler` - htey are just indicators. You can click two bang objects under the "speed" slider to slow down the playback of sample.

The horizontal sliders inside of `subs/mixer` can be used to add reverb to each track.

To record your performance click "start" command at the bottom of signals.pd. Sound will be recorded to **test.wav** file inside of the signals.pd directory. Make sure to click "stop" when you wish to end recording.

## Creadits

 - Noise generators was originally created by **auur**, and are described in [this article](https://olidunham.wordpress.com/2010/05/04/ambient-pd-composition/).
 - **jon~** reverb is brilliant work of **antonhornquist**. [Here is the GitHub repository](https://github.com/antonhornquist/jon-pd).
 - **Rubbing Metal.wav** [sample by PsychoPancake](https://freesound.org/people/PsychoPancake/sounds/325235/).
 - Toy piano samples made with Yamaha Reface CP.
 

