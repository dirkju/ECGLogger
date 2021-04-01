# ECGLogger

Arduino sketch to log ECG data onto an SDCard. 

Used hardware:
* Arduino Pro Atmega328P 3.3V, 8MHz 
* LC Technology SDCard reader shield 5V
* AD8232-based ECG front-end https://www.analog.com/media/en/technical-documentation/data-sheets/ad8232.pdf

Used libraries:
* SDFat https://github.com/greiman/SdFat
* This logger is heavily inspired by https://github.com/greiman/SdFat/tree/master/examples/AvrAdcLogger

Data format:
* A number of signal processing software understands WAV format. Maybe this should be used as a capture format? https://gasstationwithoutpumps.wordpress.com/2011/10/08/making-wav-files-from-c-programs/
* WAV resources: http://www.ringthis.com/dev/wave_format.htm
* https://code.google.com/archive/p/waverp/downloads
* TMR Arduino PCM library (with experimental record function): https://github.com/TMRh20/TMRpcm/wiki

ECG data post-processing:
* PhysioNet https://physionet.org/ and software package https://archive.physionet.org/physiotools/wfdb.shtml
* Database of ECGs https://physionet.org/about/database/