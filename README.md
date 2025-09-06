# ATS CV Optimizer powered by Gemini AI

Instantly tailor your resume to specific job requirements to beat Applicant Tracking Systems (ATS) and land more interviews. Powered by the Google Gemini API.

**GitHub Repository:** [https://github.com/your-username/gemini-cv-optimizer](https://github.com/your-username/gemini-cv-optimizer)

---

## ✨ Key Features

-   **AI-Powered Optimization**: Leverages the `gemini-2.5-flash` model to analyze your CV and a target job description, then rewrites your CV to highlight relevant skills and experience.
-   **ATS-Friendly Formatting**: Generates a clean, professionally structured CV layout that is easily parsable by modern Applicant Tracking Systems.
-   **Multi-Format File Support**: Accepts your current CV in both `.docx` and `.pdf` formats.
-   **Advanced OCR for Scanned PDFs**: Automatically detects image-based or scanned PDFs and uses Gemini's multimodal capabilities to perform Optical Character Recognition (OCR) to extract the text.
-   **Download as PDF**: Easily save your newly optimized CV as a high-quality PDF with a single click.
-   **Intuitive UI**: A simple, clean, and responsive user interface with drag-and-drop support for easy file uploads.

## 🚀 Technologies Used

-   **Frontend**: React, TypeScript, Tailwind CSS
-   **AI Engine**: Google Gemini API (`@google/genai`)
-   **File Parsing**: `pdfjs-dist` (for PDFs), `mammoth` (for DOCX)
-   **PDF Generation**: `html2pdf.js`

## ⚙️ Getting Started

### Prerequisites

-   A modern web browser.
-   A Google Gemini API Key.

### Running Locally

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/gemini-cv-optimizer.git
    cd gemini-cv-optimizer
    ```

2.  **Set up your API Key:**
    This project is configured to use an environment variable for the Google Gemini API key. You must set the `API_KEY` variable in the environment where you run the application.

3.  **Serve the application:**
    Since this is a client-side application using static HTML, CSS, and JS, you can serve it with any simple local server. For example, using Python:
    ```bash
    python -m http.server
    ```
    Or using Node.js with a package like `serve`:
    ```bash
    npx serve .
    ```

4.  Open your browser and navigate to the local server's address (e.g., `http://localhost:8000`).

## 📋 How to Use

1.  **Upload Your CV**: Drag and drop your current CV (`.docx` or `.pdf`) into the upload area, or click to select a file. The application will parse the content. If it's a scanned PDF, it will automatically use AI-powered OCR.
2.  **Paste the Job Description**: Copy the full text of the job description for the role you're targeting and paste it into the corresponding text area.
3.  **Optimize!**: Click the "Optimize My CV" button. The Gemini API will process your information and generate a new, tailored CV.
4.  **Download**: Review the optimized CV and click "Save as PDF" to download your new document.
