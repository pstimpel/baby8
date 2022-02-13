# Baby 8 sequencer for a modular synth, Eurorack format

Video: 

Some time ago I started building a modular synth. This is not so much about music, it is more about analogue electronics. Therefore, 

## be warned!
If your expectation is to have true volts per octave, this might not be the right thing for you. Even, this is not as important for a sequencer since its task is to produce a voltage offset, controlled by a gate. This sequencer here does this job.

### Credits

This whole thing here was built upon the ideas of Kristian Blåsol. So if you want to give Credit, he is the right person. Please check out his Baby 8 with lots of explanations here: https://www.youtube.com/watch?v=cfRnbIx2xjg

## Some remarks

If you go for project, you will need some material, beside the obvious stuff like Soldering tools and some Lab toys like a multimeter, power supply and oscilloscope. You need - beside the stuff mentioned in the circuit diagram:

- 8 potentiometers, 100k
- 6 3.5mm headphone jacks, with a breaking contact for cascade out
- 1 switch dual pole ON-ON
- 8 switches single pole ON-OFF-ON
- 1 push button
- 5mm LEDs
- Dupont wires, pinheaders male, IC sockets ...
- shrink tube, hot glue, ...

The connecting cable from panel to pcb stuff was done using pinheaders and dupont-wires. There are more reliable ways to do it, but again: for me this was OK. I had a hard time fitting all connections, it is kind of crowded. Maybe, I address this in a later version. 

The pcb I was creating is a single layer pcb. With two layers, I would have avoided some strange routing issues, but again it is about doing it for better understanding of what happens in such circuits. I had no single reason to make it nice. Sorry!

I am using THT, so sorry for those SMD fanboys out there. Call me "stuck in the 80s", no problem.

## The panel

Some people create nice panels out of nice materials, I was going for 3d printed PLA - since the whole idea of my Synth is to be a concept, not an instrument for a stage. You can find my panel in 3mf format in the panel folder. 

## The manual

Connect a clock signal, 5V to Clock In. Connect CV out to a VCO or something like that. Enable the clock, adjust each steps poti - Done.

What else do we have?

1.) Reset In: connect the sync of your clock to sync the sequencer stepping. 

2.) If you have more than one sequencer you can create chains using Cascase In and Cascade Out

3.) The DP switch turns on/off the received Gate signal for the whole sequencer

4.) The Step hold button enables you to go through the sequence step by step, the switch from 3 needs to be in its Ignore Gate position

5.) Gate out: produces a 5V gate signal if enables for a certain step

6.) The switch per step allows you do either
- reset the steps, like turning the Baby 8 into a Baby 2 by enabling reset on step 3
- enable the step and produce a gate signal 
- enable the step but do not produce a gate signal

# Known issues

- The connectivity between panel and board is so crowded, dupont wires might be the least reliable option here
- There is no true reset to step 1 yet
- Linear potentiometers create quite fiddly handlin in higher tones
- the hole circuit is as reliable as AWS: it works OK most of the time, but if there is an issue, the whole world goes nuts


## Dislaimer

Whatever you do with this stuff, don't blame me! If magic smoke appears, or you destroy your electronic lab, it is on you, only. As well I am not reliable if your created sounds cause zombees to go wild, or Aliens to examine your butt. You were warned!