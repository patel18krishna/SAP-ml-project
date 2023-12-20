# Speech-to-Story Generator with GPT-2

This Python script utilizes speech recognition and the GPT-2 language model to generate a story based on user input. The script listens for a wake-up word, transcribes the user's input, generates a story prompt using GPT-2, and converts the generated text into speech.

## Dependencies

Make sure to install the required Python libraries before running the script:

```bash
pip install SpeechRecognition
pip install gtts
pip install transformers
```

## Usage

1. Run the script:
   ```bash
   python your_script_name.py
   ```

2. The script will listen for the wake-up word ("bob" by default). Once detected, it transcribes the user's input.

3. The transcribed input is used to generate a story prompt with GPT-2.

4. The generated story prompt is converted into speech, and the resulting audio is saved in the specified directory.

## Configuration

- **Model Selection:** The script uses the GPT-2 language model. You can explore different models supported by the `transformers` library.

- **Wake-up Word:** The wake-up word can be customized in the `listen_for_wake_word` function.

- **Audio Output Directory:** Change the `output_directory` variable to specify the directory where the generated audio will be saved.

## File Structure

- `SAP_college_project.ipynb`: The main Python script.

## Generated Audio

The generated audio file will be saved in the specified output directory with the filename `generated_story_output.mp3`.
