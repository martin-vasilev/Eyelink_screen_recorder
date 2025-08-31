**Eyelink screen recorder**:

This programme can record Eyelink data in the background while you are doing other things on your screen (e.g., using a particular application or website). The Eyelink window is minimised while you do other things, but the eye-movement data is still being recorded. The programme automatically sends UNIX timestamps to the Eyelink machine every time you call drift check ("D") to help synchronise the Eyelink data with your PC application.

The easiest way to set it up is to install Anaconda (https://www.anaconda.com/download). The code is tested on python version 3.11.

You will also need to download and install the Eyelink developer API kit: https://www.sr-research.com/support/forum-9.html . NOTE: if you use a different python version, you will need to manually copy the pylink files (under the folder "pylink") associated with your version from the SR Research folder).

The code uses a few python packages. To install them, open the Anaconda prompt and type "conda install requirement.txt"

Execute pygame_experiment.py to start. Note that this may open a minimised screen (depending on your OS), so you may need to click it to open it full-screen.

How to control the programme:

- Enter: do Eyelink camera set-up etc.
- press "C" to enter calibration setup-up at any time
- press "D" to enter drift check any time. NB: once you exit drift check/ calibration, the screen will minimise. The programme keeps recording your computer screen until you call the C/D keys again.
- press "Ctr+E" to exit the programme and stop recording. You can find your data file in the "Results" folder.

