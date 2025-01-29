# Problem Solver with Google Gemini

This Streamlit application allows you to analyze and solve problems, including math and logic, using Google's Gemini AI model. You can input problems through:

-   **Images:** Upload images (JPG, JPEG, PNG) containing math or logic problems.
-   **Text:** Directly type the problem into a text area. You can use either:
    -   **Testo Normale:** For general text interpretation and problem-solving.
    -   **LaTeX:** For entering mathematical expressions and equations using LaTeX syntax.
-   **Files:** Upload PDF, DOCX, or TXT files containing the problem.

The app uses the **Gemini 2.0 Flash Thinking** experimental model to generate a solution or provide an interpretation of the input.

## Features

-   **Multiple Input Methods:** Supports images, text input (normal and LaTeX), PDF, DOCX, and TXT files.
-   **Gemini AI Model:** Leverages the power of Google's experimental **Gemini 2.0 Flash Thinking** model.
-   **Detailed Explanations:** Provides explanations of the solution steps or interpretations of the text.
-   **Error Handling:** Gracefully handles invalid input and potential errors during processing.
-   **User-Friendly Interface:** Built with Streamlit for a simple and intuitive user experience.
-   **Copy to Clipboard:** Easily copy the generated solution to your clipboard.

## Getting Started

### Prerequisites

-   Python 3.8 or higher
-   A Google Cloud account with access to the Gemini API (you'll need an API key)

### Installation

1. **Clone the repository:**

    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```

2. **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

    (Make sure to create a `requirements.txt` file with the following content:

    ```text
    streamlit
    Pillow
    google-generativeai
    python-dotenv
    PyPDF2
    python-docx
    ```)

3. **Set up your environment variables:**
    -   Create a file named `.env` in the root directory of the project.
    -   Add your Gemini API key to the `.env` file:

    ```
    GEMINI_API_KEY=your_api_key_here
    ```

### Running the App

1. **Execute the following command in your terminal:**

    ```bash
    streamlit run main.py
    ```

2. **Open your web browser and go to the URL provided by Streamlit** (usually `http://localhost:8501`).

## Usage

1. **Choose your input method:** Select whether you want to upload an image, enter text, or upload a file.
2. **Provide the problem:** Upload your file or enter the problem text (selecting "Testo Normale" or "LaTeX" if entering text).
3. **Click "Analyze" (or a similarly named button):** The app will send the problem to Gemini and display the solution or interpretation.
4. **Copy the solution (optional):** The solution will be displayed in a code block and copied to your clipboard automatically when it's generated.

## Important Notes

-   The Gemini **2.0 Flash Thinking** model used in this app is experimental. The accuracy of the solutions or interpretations may vary.
-   For complex or ambiguous problems, the model might not always provide correct or complete answers.
-   Make sure your input (image, text, or file) clearly represents the problem you want to solve for the best results.
-   Be mindful of the limitations of the Gemini API, such as rate limits and usage quotas. Refer to the Google Cloud documentation for more information.