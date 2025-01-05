# Chatbot with Schedule Management Bahasa Indonesia

This project builds a chatbot that can understand user queries and respond accordingly. It integrates a schedule management feature, allowing users to add, update, delete, and view upcoming events.

## Installation

- Install the required dependencies using pip:

```bash
pip install tensorflow keras nltk pandas openpyxl tabulate PySastrawi
```

   - TensorFlow: For building and training the machine learning model powering the chatbot.
   - Keras: A high-level API for building neural networks on top of TensorFlow.
   - NLTK: Natural Language Toolkit for text processing tasks like tokenization and stemming.
   - Pandas: For data manipulation and analysis.
   - Openpyxl: For interacting with Excel files (schedule management).
   - Tabulate: For creating formatted tables (schedule display).
   - [Sastrawi](https://github.com/har07/PySastrawi): Indonesian language processing library.


## Usage

**Recommended Environment:** For optimal performance and ease of use, it is recommended to run this program in an interactive notebook environment like Jupyter Notebook or Google Colab.

**Steps:**

1. **Launch Jupyter Notebook or Google Colab:**

   - **Jupyter Notebook:** Open the Jupyter Notebook application and navigate to the directory containing the `chatbot.ipynb` file.

   - **Google Colab:** Access Google Colab and upload the `chatbot.ipynb` file.

2. **Execute the Code:**

   - **Jupyter Notebook:** Click on the "Run" button (or use the keyboard shortcut Shift+Enter) within each code cell to execute the code sequentially.

   - **Google Colab:** Click on the "Play" button (or use the keyboard shortcut Shift+Enter) in the "Code" tab to execute the entire notebook code.

3. **Interact with the Chatbot:**

   - Type your message in the notebook cell and execute the code.
   - The chatbot will respond based on its understanding of your query.

**Additional Notes:**

- Ensure that you have installed the required dependencies (listed in the "Installation" section) before executing the code.
- If you encounter any errors or issues, check the notebook's output messages and consult the code for any potential debugging points.
- make sure intents_edit.json has been added to the environment

## Functionality Breakdown

- **Chatbot:**
   - Leverages a pre-trained TensorFlow model to classify user queries and generate responses.
   - Utilizes NLTK for text preprocessing like tokenization and stemming.

- **Schedule Management:**
   - Employs pandas for reading, writing, and manipulating schedule data stored in an Excel file (schedule.xlsx).
   - Enables adding, updating, deleting, and displaying events.

## Acknowledgements

- This project incorporates pre-trained models and libraries from TensorFlow and NLTK.

## License

- This project is licensed under this [LICENSE](LICENSE).

## Program Description

This program contains the main logic for the chatbot and schedule management functionality. It utilizes the following libraries:

- `tensorflow` and `keras`: For building and training the neural network model that powers the chatbot's natural language processing capabilities.
- `nltk`: For text preprocessing tasks like tokenization and stemming, which prepare the user's input for the model.
- `pandas`: For reading, manipulating, and writing data to an Excel file (schedule.xlsx) that stores the user's schedule information.
- `openpyxl`: For interacting with the Excel file (schedule.xlsx).
- `tabula`: For creating formatted tables to display the user's schedule in a clear and organized manner.
- `PySastrawi`: For Indonesian language processing, if applicable.

The program's core functionality revolves around the following steps:

1. **Load Data:** Imports the necessary libraries, loads the pre-trained TensorFlow model, and initializes the schedule management system.

2. **Process User Input:** Receives the user's input as text and preprocesses it using NLTK's tokenization and stemming techniques.

3. **Classify User Intent:** Utilizes the trained TensorFlow model to classify the user's intent, which represents the underlying purpose of their message.

4. **Generate Response:** Based on the classified intent, retrieves the corresponding response from the intents_edit.json file.

5. **Handle Schedule Management:** If the user's input relates to schedule management, delegates the task to the appropriate schedule management functions, such as adding, updating, deleting, or displaying events.

6. **Output Response:** Sends the generated response or schedule information back to the user.

7. **Repeat:** Continues the loop, waiting for the next user input and repeating the process.

## Developer : Dzikri Maulana, Malik Syafi'i

Dzikri Maulana's [linkedin](https://www.linkedin.com/in/dzikrimaulana87/)

Malik Syafi'i's [Github](https://github.com/maliks1)
