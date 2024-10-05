# ASPIRE_ai_music_generator
🎶 Emotion-Based Music Generation with AI:
This project is an AI-powered music generation system that composes music based on user-selected emotions, using a dataset of MIDI files. The system is trained to generate music sequences and plays them using MIDI synthesis. It uses the EMOPIA dataset for emotion recognition and music generation.

Technologies used:
TensorFlow: Used for building and training the Recurrent Neural Network (RNN) with LSTM layers to generate music sequences based on emotional input.
Keras (TensorFlow API): A high-level deep learning API for designing, training, and evaluating the LSTM model.

PrettyMIDI: A powerful library for reading, writing, and manipulating MIDI files. It is used to extract note sequences (pitch, start time, end time, velocity) from MIDI files and also to synthesize audio from generated music sequences.
FluidSynth: A software synthesizer used to convert generated MIDI notes into audio using SoundFonts (.sf2 files).
Music21: A Python toolkit used for MIDI analysis and playback in a Jupyter notebook or Colab environment.

Description:
In the first file (one_instrument_generation.ipynb) we have made use of 50 songs midi dataset. It takes the input of a song in the midi form and analyzes it to generate the output midi file. Here, the output tune is generated using only a single instrument.
The second file (multiple_instrument_generation.ipynb) as the name suggests, generates the output midi file based on all the instruments used in the original input midi. It consists of the same 50 songs dataset.
Lastly, the third file (Emopia_final.ipynb) consists of the EMOPIA dataset that includes the song midi file as well as the label for the emotion. Based on the input emotion given, the created model generates the output midi file.
All the three files make use of RNN LSTM model. The first two files use the built-in RNN in tensorflow. Whereas in the last file we are creating a new model with different layers.

Output:Every time the program is run, it generates a new tune. The best output so far has been attached in the files list
