# English Dictionary API

Welcome to the English Dictionary API! This Flask web application provides a simple API to retrieve definitions for English words. The data is sourced from a CSV file named `dictionary.csv`. The API offers endpoints to access word definitions.

## Getting Started

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/TUR14CUS/dictionary-api.git
   cd dictionary-api
   ```

2. Install the required dependencies:

   ```bash
   pip install Flask pandas
   ```

3. Run the Flask application:

   ```bash
   python main.py
   ```

   The application will start running on `http://127.0.0.1:5001/`. You can access the API endpoints described below.

## API Endpoints

### 1. Get Home Page

- **Endpoint:** `/`
- **Method:** GET
- **Description:** Displays the home page.

   Example: [http://127.0.0.1:5001/](http://127.0.0.1:5001/)

### 2. Get Definition for a Specific Word

- **Endpoint:** `/api/v1/<word>/`
- **Method:** GET
- **Parameters:**
  - `<word>`: The English word for which you want to retrieve the definition.
- **Description:** Retrieves the definition of a specific word.

   Example: [http://127.0.0.1:5001/api/v1/hello/](http://127.0.0.1:5001/api/v1/hello/)

## Data Source

The word definitions are sourced from a CSV file named `dictionary.csv`. Ensure that this file is present and contains the necessary columns (`word` and `definition`).

## Usage

To use the API, simply make a GET request to the appropriate endpoint with the desired word. The API will return a JSON object containing the word and its definition.

## Example Response

```json
{
  "word": "example",
  "definition": "A representative form or pattern."
}
```

## Notes

- Adjust the CSV file name and column names in the code if they differ from the provided example.
- Customize and extend the API based on your specific requirements.
- If you encounter any issues or have suggestions for improvement, feel free to open an issue or submit a pull request.

Enjoy exploring the English language with this simple and handy dictionary API! 📚📖
