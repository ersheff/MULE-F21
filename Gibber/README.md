# MULE Gibber Cheat Sheet

## General
- Set tempo at the top with — e.g. Clock.bpm = 140
- We should prepare a stop line for every variable ahead of time — e.g. kick.stop()
- Set key with — e.g. Theory.root = 'c4'
- Set scale with — e.g. Theory.mode = 'lydian'
    - Options: aeolian, dorian, phrygian, ionian, mixolydian, lydian, etc.

## Running Code
- Put your cursor on a line and press Control-Enter to run just that line
- Highlight multiple lines and press Control-Enter to run a selection
- Execute "blocks" of code by placing your cursor inside a block and pressing Alt-Enter (Option-Enter in macOS)
- A block is a chunk of code with a blank line on either side of it

## Instruments
- Create an instrument by calling is and assigning to a variable — e.g. kick = Kick()
- Using variables is super important — it makes it much easier to stop parts later!
- Basic instruments to use:
    - Rhythmic (don’t need note.seq)
        - Kick, Snare, Hat, Cowbell, Clap
    - Melodic/Harmonic (need note.seq)
        - FM, Monosynth, Synth, Pluck

## Sequencing
- To create a sequence of notes/triggers, use .trigger.seq(amplitude,duration) — the actual sequence is defined inside the parentheses with square brackets for sequences longer than 1 — e.g. .trigger.seq(\[1,0,0.5,1],1/4)
- To create a sequence of pitches, use .note.seq(pitch,duration) — pitches start at 0 for the chosen scale

## Advanced
- FX!
- Instrument parameters (e.g. presets, decay, detune, etc)
- Other ways to define drum sequences (tidal cycles or step sequencer)
