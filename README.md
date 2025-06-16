# Log Analyzer GUI

This project is a Log Analyzer GUI built using Python's Tkinter library. It allows users to upload log files, analyze their contents, and generate AI-based suggestions for improvements or issues found in the logs.

## Features

- **File Upload**: Users can select log files in `.log` or `.txt` formats for analysis.
- **Textual Analysis**: The application provides a detailed textual analysis of the log file, including error and warning counts, top IP addresses, HTTP methods, requested URLs, and status codes.
- **Graphical Analysis**: Users can view graphical representations of the log data, including requests per hour and top requested URLs.
- **AI Suggestions**: The application integrates with an AI service to generate actionable suggestions based on the log analysis.

## Requirements

- Python 3.x
- Tkinter (usually included with Python)
- Matplotlib
- Pillow
- python-docx
- google-generativeai (for AI suggestions)

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd log_analyzer
   ```

2. Install the required packages:
   ```
   pip install matplotlib Pillow python-docx google-generativeai
   ```

3. Set up the environment variable for the AI API key:
   - For Windows:
     ```
     setx GEMINI_API_KEY "your_api_key_here"
     ```
   - For Linux/macOS:
     ```
     export GEMINI_API_KEY="your_api_key_here"
     ```

## Usage

1. Run the application:
   ```
   python gui.py
   ```

2. Use the "Choose Log File" button to select a log file for analysis.

3. Click on "Analyze Log" to start the analysis process.

4. View the results in the textual analysis section and the graphical analysis section.

5. Review AI suggestions generated based on the analysis.

## Notes

- Ensure that the log files are accessible and readable.
- The application currently uses multiprocessing for handling file uploads and log analysis to improve performance and responsiveness.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.