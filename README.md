```markdown
# [TaqreeRx]

## Overview

This project provides a proof-of-concept (PoC) for a medical AI assistant that integrates Speech-to-Text (ASR) with a Large Language Model (LLM) to automate the generation of clinical SOAP notes from spoken medical consultations. It leverages Arabic language transcription and generation capabilities.

## Features

*   **Automatic Speech Recognition (ASR):** Transcribes spoken Arabic medical consultations using the Whisper Large-v3 model.
*   **Large Language Model (LLM) Integration:** Processes the transcribed text to generate structured SOAP (Subjective, Objective, Assessment, Plan) notes using the Qwen-1.5-7B-Chat model.
*   **GPU Accelerated:** Optimized for performance using GPU acceleration.
*   **Arabic Language Support:** Specifically designed and configured for Arabic medical dialogue.

## Getting Started

### Prerequisites

To run this notebook, you will need:

*   Google Colab (recommended for GPU access) or a local Python environment with GPU support.
*   The following Python libraries:
    *   `transformers`
    *   `torch`
    *   `torchaudio`
    *   `soundfile`
    *   `openai-whisper`
    *   `accelerate`
    *   `bitsandbytes`
    *   `sentencepiece`

### Installation

1.  **Clone this repository:**
    ```bash
    git clone [Your Repository URL]
    cd [Your Repository Name]
    ```

2.  **Open the Colab notebook:** Upload `TaqreeRx.ipynb` to Google Colab.

3.  **Run the installation cells:** Execute the first code cell in the notebook to install all necessary libraries.
    ```python
    # Install required libraries
    !pip install -q transformers torch torchaudio soundfile
    !pip install -q git+https://github.com/openai/whisper.git
    !pip install -q accelerate bitsandbytes sentencepiece
    ```

### Usage

1.  **Upload your audio file:** Ensure your medical consultation audio file (e.g., `arabic_clinical_audio.mp3`) is uploaded to your Colab environment or linked from Google Drive. Update the `AUDIO_FILE_PATH` variable in the notebook if your file name or path is different.

2.  **Execute the notebook cells sequentially:**
    *   The notebook will first load the Whisper ASR model and transcribe the audio.
    *   Then, it will load the Qwen LLM and generate the SOAP note based on the transcription.

3.  **Review the output:** The generated transcript and the final SOAP note will be printed in the output cells.

## Models Used

*   **ASR Model:** Whisper Large-v3 ([Link to Hugging Face or OpenAI page if desired])
*   **LLM for SOAP Note Generation:** Qwen-1.5-7B-Chat ([Link to Hugging Face page if desired])

## Example Output

(You might want to include a snippet of a sample transcription and generated SOAP note here, or a screenshot.)

## License

This project is licensed under the MIT License - 

## Contact

Dr. Ahmed Gomaa / ahmed.gomaa@scranotn.edu

```
