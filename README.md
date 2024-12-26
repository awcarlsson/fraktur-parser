## About
Script to translate scanned German Fraktur texts into English and export them to a document.

Uses Google Cloud Vision and GPT-4o.

## Setting Up the Environment
Create and activate a virtual environment and install dependencies:
```
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
```

You'll need to [setup Google Cloud Vision](https://cloud.google.com/vision/docs/setup) and get an [OpenAI API key](https://platform.openai.com/docs/quickstart).

## Usage
1. Accepts PDF of scanned text (images) as input.
2. Modify translation prompt in `prompt.txt`.
3. Run with:
```
python3 translator.py [PATH_TO_PDF]
```
4. Output will be saved in `output/` as `[INPUT_PDF_NAME]_translated.docx`