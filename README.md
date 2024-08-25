# Celebrity Search Application using LangChain and OpenAI

This project is a demonstration of building a simple celebrity search application using LangChain, Streamlit, and OpenAI API. The application is designed to search for information about celebrities using a custom large language model (LLM) and provides a seamless user experience with a conversational interface.

## Features

- **LangChain Integration**: Utilizes LangChain to build and manage custom LLMs for the application.
- **Streamlit Interface**: Implements a user-friendly web interface using Streamlit.
- **Prompt Engineering**: Custom prompts and sequential chains are used to refine search queries and outputs.
- **Memory Buffers**: Stores conversation history to maintain context across multiple queries.
- **Sequential Chains**: Chains multiple prompts to create a logical flow of information from one query to the next.

## Installation

To get started with the project, follow these steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/celebrity-search-langchain.git
    cd celebrity-search-langchain
    ```

2. **Set Up the Environment**:
    - Ensure you have Python 3.8.1 or higher installed.
    - Create a virtual environment:
      ```bash
      conda create -n langchain_env python=3.9
      conda activate langchain_env
      ```
    - Install the required packages:
      ```bash
      pip install -r requirements.txt
      ```

3. **Configure OpenAI API**:
    - Obtain your OpenAI API key and add it to `constants.py`:
      ```python
      OPENAI_API_KEY = 'your-api-key-here'
      ```

## Usage

1. **Run the Application**:
    ```bash
    streamlit run main.py
    ```

2. **Search for a Celebrity**:
    - Enter the name of a celebrity in the search bar.
    - The application will return information about the celebrity, including their date of birth and significant events related to them.

3. **Explore the Code**:
    - `main.py`: Contains the main application logic, including the LangChain integration and Streamlit interface.
    - `constants.py`: Stores configuration variables like the OpenAI API key.
    - `requirements.txt`: Lists all dependencies required to run the project.

## How It Works

### Prompt Engineering
The application uses custom prompt templates to generate responses based on user input. By creating sequential chains, the application can process complex queries by passing the output from one prompt as the input to the next.

### Memory Buffers
Memory buffers are used to store conversation history, allowing the application to remember past interactions and provide more contextually accurate responses.

## Future Enhancements

- **Advanced Prompt Engineering**: Implement more sophisticated prompt templates for complex queries.
- **Custom Data Integration**: Allow users to train the model with their own datasets.
- **Enhanced UI**: Improve the Streamlit interface for a more interactive user experience.

## Contributing

Contributions are welcome! Please fork this repository, create a new branch, and submit a pull request with your changes. For major changes, please open an issue first to discuss what you would like to contribute.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [LangChain Documentation](https://github.com/langchain-ai/langchain)
- [Streamlit Documentation](https://streamlit.io/)
- [OpenAI API Documentation](https://beta.openai.com/docs/)
