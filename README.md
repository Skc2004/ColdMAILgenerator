# ColdMAILgenerator

ColdMAILgenerator is a web application that leverages the Llama 3.1 8B Instant model to automate the creation of personalized cold emails. It enables companies to efficiently reach out to potential clients by generating tailored emails based on job postings.

## Features

- **Job Posting Analysis**: Extracts key information from provided job postings to understand client needs.
- **Portfolio Matching**: Utilizes a vector database to align your company's projects with the client's requirements.
- **Email Generation**: Crafts professional and customized cold emails using the Llama 3.1 8B Instant model.
- **Streamlit Interface**: Offers an intuitive web interface for seamless user interaction.

## System Architecture

The application follows a streamlined workflow:

1. **Input**: User provides a job posting URL or text.
2. **Data Extraction**: System extracts job details from the input.
3. **Portfolio Retrieval**: Relevant projects are fetched from the vector database.
4. **Email Generation**: A personalized email is generated using the Llama 3.1 8B Instant model.
5. **Output**: The crafted email is displayed for user review and customization.

## Installation

To set up the ColdMAILgenerator locally:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/Skc2004/ColdMAILgenerator.git
   cd ColdMAILgenerator
   ```


2. **Set Up a Virtual Environment**:

   ```bash
   python -m venv env
   ```


3. **Activate the Virtual Environment**:

   - On Windows:

     ```bash
     .\env\Scripts\activate
     ```

   - On macOS/Linux:

     ```bash
     source env/bin/activate
     ```

4. **Install Dependencies**:

   ```bash
   pip install -r requirements.txt
   ```


5. **Set Up Environment Variables**:

   Obtain an API key from [Groq](https://console.groq.com/keys) and add it to the `.env` file in the `app` directory:

   ```
   GROQ_API_KEY=your_api_key_here
   ```


6. **Initialize the Vector Database**:

   Ensure your portfolio data is stored in `my_portfolio.csv`. Run the `chromadb.ipynb` notebook to populate the vector database.

7. **Launch the Application**:

   ```bash
   streamlit run app/main.py
   ```


   Access the application at `http://localhost:8501`.

## Usage

1. **Input Job Posting**: Enter the URL or paste the text of the job posting into the application.
2. **Generate Email**: Click the "Generate Email" button to create a personalized cold email.
3. **Review and Customize**: Modify the generated email as needed before sending.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch:

   ```bash
   git checkout -b feature-name
   ```


3. Commit your changes:

   ```bash
   git commit -m 'Add new feature'
   ```


4. Push to the branch:

   ```bash
   git push origin feature-name
   ```


5. Submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgements

Special thanks to the developers of Llama 3.1 and the contributors to the open-source tools utilized in this project. 
