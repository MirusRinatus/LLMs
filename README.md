Semantic Similarity Comparison Tool

Table of Contents
Overview
Features
Demo
Installation
Configuration
Usage
Example Output
Dependencies
Contributing
License
Contact
Overview
The Semantic Similarity Comparison Tool is a Python-based script that demonstrates how to manipulate prompts, interact with OpenAI's GPT-4 API, and evaluate the semantic similarity between AI-generated responses. Specifically, the tool:

Name Substitution: Replaces a predefined name ("Akecheta") with either a randomly selected name from a list (["Ahanu", "Chayton", "Dakota"]) or a fixed name ("User123") within a prompt.
AI Interaction: Sends the modified prompts to OpenAI's GPT-4 model to generate responses.
Response Restoration: Replaces the substituted names back to the original name ("Akecheta") in the received responses.
Semantic Comparison: Computes the semantic similarity between the two final responses using OpenAI's Embedding API and cosine similarity.
This tool is useful for tasks such as ensuring consistency in AI-generated content, evaluating how name substitutions affect response generation, and understanding semantic relationships between different AI outputs.

Features
Random Name Substitution: Dynamically replaces names in prompts with randomly selected alternatives.
Fixed Name Substitution: Allows substitution with a predefined name for consistent comparisons.
AI Integration: Utilizes OpenAI's GPT-4 model to generate contextually relevant responses.
Semantic Similarity Analysis: Employs embedding vectors and cosine similarity to quantitatively assess the similarity between responses.
Robust Error Handling: Gracefully manages API errors and edge cases to ensure smooth execution.
Demo

Note: Replace the above placeholder with an actual demo GIF if available.

Installation
Clone the Repository

bash
Copy code
git clone https://github.com/yourusername/semantic-similarity-comparison-tool.git
cd semantic-similarity-comparison-tool
Create a Virtual Environment (Optional but Recommended)

bash
Copy code
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install Required Libraries

Ensure you have Python 3.7 or higher installed. Install the necessary Python packages using pip:

bash
Copy code
pip install openai==0.28.0 numpy
Alternatively, uncomment and run the installation lines at the top of the script:

python
Copy code
# !pip install openai==0.28.0
# !pip install numpy
Configuration
Obtain OpenAI API Key

Sign up or log in to OpenAI to obtain your API key.
Securely Provide API Key

The script prompts you to enter your OpenAI API key securely at runtime. Ensure you do not hard-code your API key into the script to maintain security.

Usage
Run the Script

Execute the script using Python:

bash
Copy code
python semantic_similarity_tool.py
Enter OpenAI API Key

When prompted, securely enter your OpenAI API key. The input will be hidden for security.

markdown
Copy code
Enter your OpenAI API key: **************
Observe the Output

The script will perform the following steps:

Random Name Substitution: Replace "Akecheta" with a randomly selected name and generate a response.
Fixed Name Substitution: Replace "Akecheta" with "User123" and generate another response.
Semantic Similarity Comparison: Compute and display the semantic similarity between the two responses.
Example Output
vbnet
Copy code
Enter your OpenAI API key: **************

Modified Prompt with Random Name (Chayton):
Prepare a short speech introducing Chayton in three points, highlighting heritage.

Final Response with Original Name (Akecheta):

Hello everyone,

Today, I'd like to introduce Akecheta, whose heritage is rich and inspiring. First, Akecheta comes from a lineage deeply rooted in traditional craftsmanship, showcasing exceptional skill and dedication. Second, their cultural background emphasizes community and collaboration, fostering strong bonds and mutual support. Lastly, Akecheta's heritage includes a profound respect for nature and sustainability, guiding their actions towards a harmonious future.

--------------------------------------------------------------------------------

Modified Prompt with Fixed Name (User123):
Prepare a short speech introducing User123 in three points, highlighting heritage.

Final Response with Original Name (Akecheta):

Good afternoon,

I am pleased to introduce Akecheta, whose heritage is both distinguished and meaningful. Firstly, Akecheta hails from a family with a long history of artistic excellence, contributing beautifully to our cultural tapestry. Secondly, their background instills values of integrity and perseverance, inspiring those around them. Lastly, Akecheta's heritage is marked by a commitment to education and personal growth, paving the way for continuous improvement and success.

--------------------------------------------------------------------------------

Comparing the two final responses for semantic similarity...

Semantic Similarity (Cosine Similarity): 0.9825
Interpretation: The responses are highly similar.
Note: Actual responses and similarity scores will vary based on the GPT-4 outputs.

Dependencies
OpenAI Python Library (openai==0.28.0)
NumPy (numpy)
Getpass (getpass) – Included in Python Standard Library
Contributing
Contributions are welcome! Please follow these steps:

Fork the Repository

Click the "Fork" button at the top right of this page.

Create a New Branch

bash
Copy code
git checkout -b feature/YourFeatureName
Make Changes and Commit

bash
Copy code
git commit -m "Add some feature"
Push to the Branch

bash
Copy code
git push origin feature/YourFeatureName
Open a Pull Request

Navigate to the original repository and click "Compare & pull request."

License
This project is licensed under the MIT License.

Contact
For any inquiries or feedback, please reach out to rinat.mirzaitov@gmail.com.
