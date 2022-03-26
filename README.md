# gpu-screen-recorder-instantreplaybashscript
Bash script that runs gpu-screen-recorder from terminal, for personal use.

##Prerequisites
This bash script requires an installation of gpu-screen-recorder (https://git.dec05eba.com/gpu-screen-recorder)
and is based on commit 5ca83d45cf044754ba1ae60a057b5420ab407a35. The file "gpu-screen-recorder" needs to be in $PATH. Pulseaudio is used for setting the sound source (the monitor of the default sink is used). 

An nvidia graphics card with support for nvfbc is required, driver will probably need to be patched using https://github.com/keylase/nvidia-patch to allow use of nvfbc.


##Setup

1. Download the `recordbuffer` bash script
2. Place it in any directory you want (recommend one in $PATH, like /usr/local/bin)

Some parameters can be tweaked in the bash script itself if needed.

##Usage
`recordbuffer`:
	Starts the video buffer (default size of 5 minutes).
	Output is placed in $HOME/Videos/gpu-screen-recorder.
`recordbuffer "some dir name`:
	Same but output is placed in "$HOME/Videos/gpu-screen-recorder/some dir name"