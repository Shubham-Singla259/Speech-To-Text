## Audio Analysis and Transcription Tool 

This Python script offers functionalities for audio analysis and transcription. 

### Features

* **Speech-to-Text Transcription:** Transcribes audio files (ideally WAV format) to text using Google Speech Recognition.
* **Word Statistics:** Calculates basic word statistics including total word count and frequencies of the top 10 most frequent words (customizable). 
* **Waveform Visualization:** Plots the waveform of the audio file for visual inspection.

### Requirements

* Python 3.x
* `speech_recognition` library (install using `pip install speech_recognition`)
* `pydub` library (install using `pip install pydub`)
* `librosa` library (install using `pip install librosa`)
* `matplotlib` library (install using `pip install matplotlib`)

### Usage

1. Clone this repository to your local machine.
2. Install the required libraries using `pip install -r requirements.txt` (assuming a `requirements.txt` file is present listing the dependencies).
3. Replace the placeholder path in `audio_file_path` within the script (`audio_analysis.py`) with the actual path to your audio file.
4. Run the script from your terminal using `python audio_analysis.py`.

### Output

* The transcribed text will be displayed in the terminal.
* If transcription is successful, word statistics including total word count and top 10 most frequent words will be shown.
* A waveform plot of the audio file will be displayed.

### Error Handling

* If the audio file format is not WAV, the script will attempt to convert it to WAV before processing.
* In case of errors during speech recognition, informative messages will be displayed.

### Customization

* You can modify the number of displayed word frequencies in the `calculate_word_stats` function by changing the value passed to the list slicing (`word_frequencies[:10]`).
* The `plot_waveform` function allows adjustments for visualization like figure size and y-axis customizations. Refer to the function documentation for details.
