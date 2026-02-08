# AI-Powered Human Attribute Detection with Python, Streamlit & Google Gemini GenAI

An intelligent computer vision application that leverages Google's Gemini GenAI to analyze images and detect human attributes with remarkable accuracy. This interactive web application combines the power of generative AI with an intuitive Streamlit interface to provide detailed insights about people in photographs.

## Overview

This project harnesses Google's advanced Gemini AI model to perform comprehensive human attribute detection from uploaded images. The system analyzes visual data to identify various characteristics including demographics, appearance, clothing, emotions, and contextual information, delivering results through an elegant and user-friendly web interface.

## Features

**Advanced AI-Powered Analysis**  
Utilizes Google Gemini's state-of-the-art generative AI capabilities to perform sophisticated image analysis and attribute extraction.

**Comprehensive Attribute Detection**  
The system can identify and analyze multiple human attributes including:
- Age estimation and gender identification
- Facial expressions and emotional states
- Clothing and fashion attributes
- Physical characteristics and appearance
- Posture and body language
- Accessories and belongings
- Contextual scene information

**Interactive Web Interface**  
Built with Streamlit for a seamless, responsive user experience that requires no technical knowledge to operate.

**Real-Time Processing**  
Upload images and receive instant AI-generated insights about detected human attributes.

**Multi-Format Support**  
Accepts various image formats including JPG, JPEG, PNG, and other common file types.

**Detailed Insights**  
Provides comprehensive descriptions and analysis rather than just simple labels or tags.

**Privacy-Focused**  
Images are processed securely without permanent storage, ensuring user privacy and data protection.

## Technology Stack

**Backend & AI**
- Python 3.8+
- Google Gemini GenAI API
- PIL (Python Imaging Library)
- google-generativeai SDK

**Frontend**
- Streamlit (Interactive Web Framework)
- Custom CSS styling

**Image Processing**
- Pillow (PIL Fork)
- NumPy (for image array operations)

## Installation

### Prerequisites
- Python 3.8 or higher
- Google Gemini API key (obtain from Google AI Studio)
- pip package manager
- Virtual environment (recommended)

### Setup Instructions

1. **Clone the Repository**
```bash
git clone https://github.com/yourusername/ai-human-attribute-detection.git
cd ai-human-attribute-detection
```

2. **Create Virtual Environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install Dependencies**
```bash
pip install streamlit google-generativeai pillow python-dotenv
```

4. **Set Up API Credentials**

Create a `.env` file in the project root:
```env
GOOGLE_API_KEY=your_gemini_api_key_here
```

Alternatively, configure through Streamlit secrets:
```bash
mkdir .streamlit
```

Create `.streamlit/secrets.toml`:
```toml
GOOGLE_API_KEY = "your_gemini_api_key_here"
```

5. **Get Your Google Gemini API Key**
- Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
- Sign in with your Google account
- Create a new API key
- Copy the key to your `.env` or `secrets.toml` file

## Usage

### Running the Application

1. **Start the Streamlit Server**
```bash
streamlit run app.py
```

2. **Access the Application**
- The application will automatically open in your default browser
- If not, navigate to `http://localhost:8501`

3. **Analyze Images**
- Upload an image using the file uploader
- Click "Analyze Image" or let auto-analysis process the image
- View detailed AI-generated insights about detected human attributes
- Upload additional images for further analysis

### Example Use Cases

**Photography & Media**
- Analyze portrait photographs for subject descriptions
- Generate metadata for image cataloging
- Assist in photo editing workflows

**Fashion & Retail**
- Detect clothing styles and accessories
- Analyze fashion trends from images
- Generate product descriptions

**Security & Monitoring**
- Describe individuals in surveillance footage
- Generate incident reports from images
- Assist in missing person descriptions

**Social Media & Marketing**
- Analyze audience demographics from event photos
- Generate engaging image descriptions
- Understand visual content better

**Research & Education**
- Study human behavior and expressions
- Analyze group dynamics in photographs
- Educational demonstrations of AI capabilities

## Project Structure

```
ai-human-attribute-detection/
│
├── app.py                      # Main Streamlit application
├── requirements.txt            # Python dependencies
├── .env                        # Environment variables (not in repo)
├── .streamlit/
│   └── secrets.toml           # Streamlit secrets (not in repo)
├── .gitignore                 # Git ignore file
├── utils/
│   ├── __init__.py
│   ├── image_processor.py     # Image processing utilities
│   └── gemini_handler.py      # Gemini API interaction
├── assets/
│   └── images/                # Sample images or UI assets
├── README.md                  # Project documentation
└── LICENSE                    # License file
```

## How It Works

1. **Image Upload**: User uploads an image through the Streamlit interface
2. **Preprocessing**: Image is validated and prepared for AI analysis
3. **AI Processing**: Image is sent to Google Gemini AI with specialized prompts
4. **Attribute Extraction**: Gemini analyzes the image and identifies human attributes
5. **Results Display**: Comprehensive analysis is presented in an easy-to-read format
6. **Iterative Analysis**: Users can upload multiple images for batch processing

## Configuration

### Customizing AI Prompts

Edit the prompts in your application to focus on specific attributes:

```python
prompt = """
Analyze this image and provide detailed information about:
- Demographics (age, gender)
- Emotional state and expressions
- Clothing and style
- Physical appearance
- Context and environment
"""
```

### Adjusting Model Parameters

Configure Gemini model settings:
- **Temperature**: Control creativity (0.0 - 1.0)
- **Top-p**: Nucleus sampling parameter
- **Top-k**: Token selection range
- **Max tokens**: Response length limit

## API Reference

### Google Gemini Models

This application supports:
- **gemini-pro-vision**: For image and text analysis
- **gemini-1.5-pro**: Latest model with enhanced capabilities
- **gemini-1.5-flash**: Faster processing with good accuracy

### Key Functions

**Image Processing**
```python
process_image(image_file) -> PIL.Image
```

**AI Analysis**
```python
analyze_attributes(image, prompt) -> str
```

**Result Formatting**
```python
format_results(ai_response) -> dict
```

## Privacy & Ethics

**Data Handling**
- Images are processed in real-time and not stored permanently
- API calls are made securely over HTTPS
- User data is handled according to Google's privacy policies

**Ethical Considerations**
- This tool should be used responsibly and ethically
- Avoid using for discriminatory purposes
- Respect individual privacy rights
- Consider bias in AI predictions
- Use for intended legitimate purposes only

**Limitations**
- AI predictions may not always be 100% accurate
- Cultural and demographic biases may exist in the model
- Results should be interpreted with appropriate context

## Security Best Practices

- Never commit API keys to version control
- Use environment variables or secrets management
- Implement rate limiting for production use
- Validate and sanitize all user inputs
- Keep dependencies updated

## Troubleshooting

### Common Issues

**API Key Errors**
- Verify your API key is correctly set in `.env` or `secrets.toml`
- Check that your API key has necessary permissions
- Ensure your Google Cloud project has billing enabled

**Image Upload Issues**
- Verify image format is supported (JPG, PNG, JPEG)
- Check image file size (should be under 20MB)
- Ensure image is not corrupted

**Slow Processing**
- Large images may take longer to process
- Consider using gemini-1.5-flash for faster results
- Check your internet connection

## Performance Optimization

- Resize large images before processing
- Implement caching for repeated analyses
- Use appropriate Gemini model based on speed/accuracy needs
- Batch process multiple images when possible

## Future Enhancements

- **Multi-person detection**: Analyze multiple people in a single image
- **Batch processing**: Upload and analyze multiple images simultaneously
- **Export functionality**: Download results in JSON, CSV, or PDF format
- **Historical tracking**: Save and compare analyses over time
- **Video support**: Extend to video frame analysis
- **Custom training**: Fine-tune models for specific use cases
- **API endpoints**: Create REST API for programmatic access
- **Mobile optimization**: Enhance mobile browser experience
- **Language support**: Multi-language result generation

## Contributing

We welcome contributions! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Dependencies

```
streamlit>=1.28.0
google-generativeai>=0.3.0
pillow>=10.0.0
python-dotenv>=1.0.0
numpy>=1.24.0
```

## System Requirements

**Minimum**
- Python 3.8+
- 4GB RAM
- Internet connection for API calls

**Recommended**
- Python 3.10+
- 8GB RAM
- Stable broadband connection

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Google Gemini AI team for providing powerful GenAI capabilities
- Streamlit community for the excellent web framework
- Open-source contributors and the Python community
- Beta testers and early adopters for valuable feedback

## Disclaimer

This application uses AI to analyze images and detect human attributes. While the technology is advanced, it may not always be 100% accurate. Results should be used as supplementary information and not as definitive conclusions. Always respect privacy rights and use this tool ethically and responsibly.

## Support & Contact

- **Issues**: Report bugs via GitHub Issues
- **Questions**: Start a discussion in GitHub Discussions
- **Email**: your.email@example.com
- **Documentation**: Visit our wiki for detailed guides

## Changelog
### Version 1.0.0 (Current)
- Initial release with core attribute detection
- Streamlit web interface
- Google Gemini integration
- Multi-format image support

**Made with ❤️ using Google Gemini GenAI and Streamlit**
