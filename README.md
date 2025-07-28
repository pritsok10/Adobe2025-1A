# PDF Processing Application

This project is designed to process PDF files, extracting content, validating titles and headings, and identifying candidates for headings. It utilizes various Python libraries to achieve these tasks efficiently.

## Project Structure

```
pdf-processing-app
├── app.py               # Main logic for processing PDF files
├── Dockerfile           # Docker configuration for the application
├── requirements.txt     # Python dependencies required for the project
└── README.md            # Documentation for the project
```

## Requirements

To run this application, you need to have Docker installed on your machine.

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd pdf-processing-app
   ```

2. **Build the Docker image**:
   ```bash
   docker build -t pdf-processing-app .
   ```

3. **Run the application**:
   ```bash
   docker run -v /path/to/pdf/files:/app/Datasets/pdf -v /path/to/output:/app/Datasets/output pdf-processing-app
   ```

   Replace `/path/to/pdf/files` with the path to the directory containing your PDF files and `/path/to/output` with the path to the directory where you want the output to be saved.

## Usage

The application will process all PDF files in the specified input directory and save the results in the output directory. You can monitor the logs for progress and any potential issues.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request with your changes.