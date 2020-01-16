This is a Step Stick style adapter with a level shifter/buffer
to allow boards with low current and/or 3.3v outputs to feed
off-board drivers.

It takes step+direction+enable inputs and outputs them 
non-inverted on the motor pins, along with ground.

The jumper block allows driving the buffer from Vio, Vmot or remove the 
jumper and feed with a 2 pin female from another +5v source.

If Vio is 5v then you can use that. If it's 3.3v then output will also
be 3.3v, but this can work if you just need more current.

If your board allows Vmot to be 5v(thus is only used for the stepper
drivers) then you can use Vmot. 

Else connect +5v and ground if needed to the header pins.

The Buffer Chip:
http://www.ti.com/product/SN74LV4T125/technicaldocuments
