# Peregrine (work in progress)

A split steno keyboard that (will hopefully) work with Plover.

# 01.  Ergogen

Start designing both halves in Ergogen https://ergogen.cache.works/
I went with a left half and a right half because that made life a lot easier in kiCAD.

peregrine-lefty.yaml

peregrine-righty.yaml

# 02. Export that to a KiCAD board 


> ergogen peregrine-lefty.yaml -o peregrinelefty
> 
> ergogen peregrine-righty.yaml -o peregrinerighty

# 0.3 Edit the board in KiCAD 

I am using a different switch so replaced the one ergogen gave me with a footprint that matches the AliExpress one. It's in footprints\AliExpressResetButton6x45xH.kicad_mod 
And this is the switch https://nl.aliexpress.com/item/1005006195785196.html . I don't have it yet so I don't yet know if it actually works.

Also clicked until all the connections were there and KiCAD was showing 0 errors.

- TODO: there are some warnings about the silkprint overlapping...somthing? for the ProMicro microcontroller. Not sure if I can ignore those.

- TODO: Check if I did anything stupid that will mean it instantly shorts out as soon as I connect it.

# 04. Firmware

- TODO: figure out how to write the firmware to make it work, and to make it work with Plover  