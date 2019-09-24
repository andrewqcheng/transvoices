# transvoices
Analysis of speech patterns of monologues taken from YouTube video blogs.

Running the ipython notebook in this repository will require [audiolabel](https://github.com/rsprouse/audiolabel), a library for reading phonetic label files (e.g., Praat TextGrids) into dataframes.

Also included in the repository are a folder that contains .ifc files, created by ifcformant (Ueda et al, 2007), and .multi_align files, created by an [automatic alignment script](https://raw.githubusercontent.com/rsprouse/ucblingmisc/master/python/multi_align), created by Ronald Sprouse. These files were created from raw .wav files and manually-transcribed TextGrids using tools from the Berkeley Phonetics Machine. If you do not use the BPM, you can use files of your own that replicate the format of the files in this repository. The .ifc files are a dataframe containing formant information about a sound file containing speech, with columns for time in seconds, root mean square, f0, and F1-4. The .multi_align files are TextGrids containing tiers for words and phones, which correspond in filename to the .ifc files.

The ipython notebook has been run on a subset of the full dataset to demonstrate how the .ifc and .multi_align files are merged, organized, and written to .csv files for statistical analysis and visualization.
