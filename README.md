```markdown
# Document Query Assistant

A Python script designed to answer questions based on the contents of documents in a specified directory. The script uses LangChain and OpenAI embeddings for natural language processing, enabling efficient query handling and document parsing.

---

## 🚀 Features

- **Multi-format Document Parsing**: Supports `.pdf`, `.docx`, `.txt`, and `.xlsx` files.
- **Intelligent Query Processing**: Leverages LangChain and OpenAI's LLM for answering queries.
- **Dynamic Text Chunking**: Splits large document content into manageable chunks for processing.
- **Interactive Console**: Real-time question-answering with user-friendly prompts.

---

## 🛠 Prerequisites

- **Python 3.x** installed on your system.
- Required Python libraries:
  - `langchain`
  - `openai`
  - `PyPDF2`
  - `docx`
  - `openpyxl`
  - `python-dotenv`
  - `faiss-cpu`
- Access to OpenAI's API (API key in `.env` file).

---

## 📥 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/document-query-assistant.git
   cd document-query-assistant
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Add your OpenAI API key to a `.env` file:
   ```env
   OPENAI_API_KEY=your_openai_api_key
   ```

4. Update the script with your desired directory path for document processing.

---

## ⚙️ Configuration

### File Directory

Set the path to the folder containing your documents:
```python
train_directory = 'train_files/'
```

### Supported File Formats

The script supports the following file types:
- `.pdf`
- `.docx`
- `.txt`
- `.xlsx`

Ensure that all files you want to process are placed in the directory specified by `train_directory`.

---

## ▶️ Usage

1. Run the script:
   ```bash
   python document_query_assistant.py
   ```

2. Enter your questions when prompted. For example:
   ```plaintext
   Enter your question: What is the procedure for client onboarding?
   ```

3. The script will:
   - Search for relevant text chunks in the documents.
   - Generate an answer using OpenAI's LLM.
   - Provide an alternate response if the LLM lacks confidence in its answer.

4. To exit, type:
   ```plaintext
   exit
   ```

---

## 📁 Directory Structure Example

```plaintext
document-query-assistant/
│
├── document_query_assistant.py
├── requirements.txt
├── .env
├── train_files/
│   ├── file1.pdf
│   ├── file2.docx
│   ├── file3.txt
│   └── file4.xlsx
├── README.md
```

---

## 📊 Output Example

### Query Input:
```plaintext
Enter your question: What are the company policies on remote work?
```

### Response:
```plaintext
Query: What are the company policies on remote work?
Response: Remote work policies are outlined in the employee handbook under Section 5.2.
```

### OpenAI Callback Metrics:
```plaintext
Tokens Used: 124
Total Cost: $0.0024
```

---

## 🔔 Notes

- Ensure your documents are properly formatted for accurate parsing.
- Responses that cannot be confidently generated will direct users to the helpdesk:
  ```plaintext
  Please reach out to security validation at (321) 521-4387 option 5 for helpdesk.
  ```
- The script clears the console after each query for a clean interactive experience.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 🧑‍💻 Author

_“Empowering insights from your documents.”_
```
```
