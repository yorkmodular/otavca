## Dual LM13700 voltage-controlled amplifier (VCA)

Another module brought to you by the Department Of Keeping It Simple.

The LM13700 is one of those chips that has been knocking around for years, minding its own business, despite the fact that it is a mind-bogglingly useful and versatile piece of silicon. Granted, it can be a bit of a pain to work with, but it's still useful nonetheless.

This is a dual VCA, each channel of which uses one of the transconductance amplifiers on the 13700. Other than the addition of a couple of linear current sources for CV control this isn't massively different from the circuit you'll find in the datasheet. It works best with signals in the +/-5V range, although it's relatively unbothered by particularly hot CVs from envelope generators.

Is it perfect? No - far from it; depending on your envelope generator there may be a bit of CV bleedthrough, but then if you want ultra-high fidelity then you're probably better off with the THAT2180, which has a unit cost about 10x that of the LM13700 ... that being said, they work well enough that I actually keep a couple in my own system.

Personally, I find that the LM13700 gives a bit of warmth to a sound, but that could just be me ...

Depending on the strength of the CVs you use, you may find it beneficial to have a couple of attenuators nearby - passive ones will do.

### Build notes

The build is relatively straightforward - apart from a couple of unusual resistors (R7/R14 - 8.2k) there are no real gotchas. The two MMBT3906 transistors should already be soldered in place.

The gain trimmers are 1M simply because there seems to be quite a bit of variation in the behaviour of LM13700s, even from chips that are from the same run - it also gives you a bit of headroom if you want unity gain at a voltage higher than 5V.

Take note of the polarity of the electrolytic capacitors and the diodes. The cathode of the diodes (the end with the black band) should match up with the ring on the silkscreen. For the CV LEDs, the square pad is ground - the short lead of the LED goes in here.

### Calibration

This is where it gets tricky - although you can probably calibrate things by ear, it's best to use an oscilloscope. For each channel, do the following - your 'scope should be attached to the output.

* Connect a source signal with known amplitude to the input - the peak voltage should correspond to unity gain. I generally use an sine or triangle LFO which is 10vp-p, with unity gain at 5V.

* Adjust the appropriate BAL trimmer until the signal is centred around 0V. If you're not using a through-zero input, use your own judgement. You may strike lucky and find that the signal is centred from the get-go - in this case, well done. If the output is clipped, back off the GAIN put until the clipping disappears and then adjust the balance accordingly.

*  Once the output is centred, adjust the gain until the input and output signals are identical.

### Purchase Links

* Pre-built module (4HP) - [https://www.yorkmodular.co.uk/products/otavca-dual-lm13700-linear-vca-4hp](https://www.yorkmodular.co.uk/products/otavca-dual-lm13700-linear-vca-4hp)
* Kit - [https://www.yorkmodular.co.uk/products/full-kit-dual-lm13700-linear-vca-4hp](https://www.yorkmodular.co.uk/products/full-kit-dual-lm13700-linear-vca-4hp)