# OPL3.java

Software implementation of the Yamaha YMF262 sound generator.

Copyright (C) 2008 Robson Cozendey <robson@cozendey.com>

This library is free software; you can redistribute it and/or modify it under the terms of the GNU Lesser General Public License as published by the Free Software Foundation; either version 2.1 of the License, or (at your option) any later verion.

This library is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more details.

You should have received a copy of the GNU Lesser General Public License along with this library; if not, write to the Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA

One of the objectives of this emulator is to stimulate further research in the OPL3 chip emulation. There was an explicit effort in making no optimizations, and making the code as legible as possible, so that a new programmer interested in modify and improve upon it could do so more easily. 

This emulator's main body of information was taken from reverse engineering of the OPL3 chip, from the YMF262 Datasheet and from the OPL3 section in the YMF278b Application's Manual, together with the vibrato table information, eighth waveform parameter information and feedback averaging information provided in MAME's YMF262 and YM3812 emulators, by Jarek Burczynski and Tatsuyuki Satoh.

This emulator has a high degree of accuracy, and most of music files sound almost identical, exception made in some games which uses specific parts of the rhythm section. In this respect, some parts of the rhythm mode are still only an approximation of the real chip. The other thing to note is that this emulator was done through recordings of the SB16 DAC, so it has not bitwise precision.

Additional equipment should be used to verify the samples directly from the chip, and allow this exact per-sample correspondence. As a good side-effect, since this emulator uses floating point and has a more fine-grained envelope generator, it can produce sometimes a crystal-clear, denser kind of OPL3 sound that, because of that, may be useful for creating new music.

Version 1.0.6 [found here](http://opl3.cozendey.com/)