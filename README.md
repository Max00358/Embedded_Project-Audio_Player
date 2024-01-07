# Embedded_Project-Audio_Player
An embedded system project of an audio player made using Altera Max 10 FPGA, Quartus Prime & NIOS II

## System Demo
https://github.com/Max00358/Embedded_Project-Audio_Player/assets/125518862/1652dea4-407a-4c59-89e3-23f0ce0c5e80

## Software & Hardware Used
  * Software
      * NIOS II
      * Quartus Prime
  * Hardware
      * Intel® Max® 10 FPGA
    
## Design Specifications
<img width="626" alt="Screen Shot 2024-01-07 at 12 39 09 PM" src="https://github.com/Max00358/Embedded_Project-Audio_Player/assets/125518862/661a0f54-8fec-49d0-ae11-80bddd5d038f">

**Must Include:**
 * The audio player must support .wav format audio files (stereo audio with 16 bit audio samples). - The audio must be read from a MicroSD card
 * The audio output uses a standard headphone jack
 * The hardware must include an LCD display that indicates the track number (as enumerated on
the SD card) and the track title (filename) on the first line of the LCD display. The second line of the LCD display must show the Player functions for STOPPED, PAUSED, PBACK-NORM SPD,
PBACK–HALF SPD, PBACK–DBL SPD, PBACK–MONO.
 * The player must only display track titles (the filename) that are actual wav files indicated by the
.wav extension.
 * The audio played must be free of distortion for all speeds - User interface must function as described

**Push Button Functionality:**

* When the Player is initialized, it displays the FIRST track Title on the LCD Display and is then in the STOPPED mode. Pressing the Play/Pause button plays the currently selected track, as currently displayed on the LCD and then must automatically STOP. Pressing the Play/Pause button while a track is playing pauses the track. When paused, the Waveplayer must remain on the current track at its current position and the audio must be silent. Pressing the Play/Pause Button again will allow the WavePlayer to continue the playback from its current track position and then continue to the end of the track. At this point the Waveplayer must STOP and then set the current track position back to the beginning of the current track. This button must be de-bounced with NO s/w delays employed.

* The <ins>**Stop**</ins> button stops a currently playing track and resets the track position to the beginning of the track. If a track is paused, the Stop button resets the track position to the beginning of the track. This button must be de-bounced with NO s/w delays employed.

* The <ins>**Previous**</ins> button searches backwards through the tracks on the SD card, one track each time the button is pressed, and displays the current track name on the LCD if the button is pressed. Searching farther backward past the first track in the list should cause the last track to be displayed. If the button is pressed while a track is not playing (stopped or paused) then the player just moves to the start of the previous track and STOPs. If the button is pressed while a track is playing, then the playing continues but it begins at the start of the previous track. This button must be de-bounced with NO s/w delays employed.

* The <ins>**Next**</ins> button searches forwards through the tracks on the SD card (one track each time the button is pressed) and displays the newly searched track name on the LCD. Searching farther forward past the last track in the list should cause the first track to be displayed If the button is pressed while a track is not playing (stopped or paused) then the player just moves to the start of the next track and STOPs. If the button is pressed while a track is playing, then the playing continues but it begins at the start of the next track. This button must be de-bounced with NO s/w delays employed.
