
# Multimedia-Content-Summarizer

## Overview
A cascaded architecture for extractive summarization of multimedia content via audio-to-text alignment. This project combines state-of-the-art speech recognition, natural language processing, and summarization techniques to generate concise summaries from video content.

## Features
- Audio extraction from multimedia content
- Speech-to-text conversion using Microsoft Azure Speech
- Advanced NLP processing with BERT and BART models
- Extractive and abstractive summarization
- Performance evaluation using ROUGE and BLEU metrics

## Technologies Used
- Python
- PyTube (for video downloading)
- Pydub (audio processing)
- Microsoft Azure Speech Recognition
- NLTK
- Transformers (BERT, BART)
- SpeechRecognition
- GTTS (Google Text-to-Speech)

## Installation

```bash
pip install -r requirements.txt
```

## Usage

```python
# Example code for basic usage
from summarizer import VideoSummarizer

# Initialize summarizer
summarizer = VideoSummarizer()

# Process video URL
summary = summarizer.process_video("youtube_url")

# Get summary
print(summary)
```

## Architecture
1. **Data Collection**: Video retrieval using PyTube
2. **Audio Processing**: Extract audio using Pydub
3. **Speech Recognition**: Convert audio to text using Azure Speech
4. **Text Preprocessing**: NLP pipeline using NLTK
5. **Summarization**: Cascaded architecture combining extractive and abstractive techniques

## Performance Metrics
- ROUGE-L F1 Score: 0.219
- BLEU Score: 0.36

## Dataset
The project uses the XSum dataset containing:
- 226,711 article-summary pairs
- Average article length: 431 tokens
- Average summary length: 23 tokens

## Contributing
1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## Authors
- Tanzir Hossain
- Ar-Rafi Islam
- Avishek Roy Sparsho
- Marjuk Ahamed
- Md. Sabbir Hossain
- Mehnaz Ara Fazal
- Annajiat Alim Rasel

## Acknowledgments
- BRAC University, Department of CSE
- Microsoft Azure for Speech Recognition API
- Facebook AI Research for BART model

## Citation
If you use this work in your research, please cite:
```bibtex
@article{hossain2024summarization,
  title={Summarization of Multimedia Content via Audio-to-Text Alignment},
  author={Hossain, Tanzir and Islam, Ar-Rafi and Sparsho, Avishek Roy and Ahamed, Marjuk and Hossain, Md. Sabbir and Fazal, Mehnaz Ara and Rasel, Annajiat Alim},
  journal={BRAC University},
  year={2024}
}
```
```

