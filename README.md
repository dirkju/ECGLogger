# ECGLogger

Arduino sketch to log ECG data onto an SDCard. 

Used hardware:
* Arduino Pro 3.3V, 8MHz 
* LC Technology SDCard reader shield 5V
* AD8232-based ECG front-end https://www.analog.com/media/en/technical-documentation/data-sheets/ad8232.pdf

Used libraries:
* SDFat https://github.com/greiman/SdFat
* This logger is heavily inspired by https://github.com/greiman/SdFat/tree/master/examples/AvrAdcLogger

ECG data post-processing:
* A number of signal processing software understands WAV format. Maybe this should be used as a capture format? https://gasstationwithoutpumps.wordpress.com/2011/10/08/making-wav-files-from-c-programs/
* PhysioNet https://physionet.org/ and software package https://archive.physionet.org/physiotools/wfdb.shtml
* Database of ECGs https://physionet.org/about/database/