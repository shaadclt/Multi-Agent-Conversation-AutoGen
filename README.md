# 🤖 Algebra Tutor Simulation using AutoGen + Groq API
This project demonstrates a conversational AI simulation between a high school student and a math tutor using the AutoGen framework and the Groq API (with LLaMA 3 model). The use case focuses on helping students understand quadratic equations through a multi-turn dialogue.

# 🚀 Features
- 🤝 Agent-to-agent conversation using ConversableAgent from AutoGen.

- 🧠 LLaMA 3.3 70B Versatile model hosted via Groq API.

- 🎓 Realistic tutoring scenario: Student asks for help, tutor responds with explanations.

- 🔍 Easy to extend for different subjects or more complex tutoring simulations.

# 📁 Project Structure
```bash
├── multi_agent_conversation.ipynb   # Main notebook (Google Colab)
├── README.md                        # Project documentation
├── LICENSE.txt                      # License file
```

# 🛠️ Requirements
## Install the required packages:

```bash
pip install -q pyautogen groq
```

# 🔐 API Key Setup
Store your GROQ_API_KEY securely using Google Colab’s userdata:

```python
from google.colab import userdata
# Set via Colab > Code > "Insert" > "Add user secret" 
api_key = userdata.get("GROQ_API_KEY")
```

# 🧑‍🏫 How It Works
1. Two agents are created:

    - Student Agent: Mimics a student struggling with quadratic equations.

    - Tutor Agent: Acts as a knowledgeable, patient math tutor.

2. Student initiates the conversation with a question.

3. Agents converse using the LLM backend powered by Groq’s LLaMA-3.3-70B.

4. Chat history, cost, and summary are printed at the end.

# 📦 Sample Output
```python
pprint.pprint(result.chat_history)
pprint.pprint(result.cost)
pprint.pprint(result.summary)
```

# 💡 Example Use Cases
- AI-powered educational simulations

- Testing LLM-to-LLM communication

- Creating adaptive learning environments

- Evaluating LLM behavior in instructional roles

# 📌 Notes
This setup runs within Google Colab using Groq's LLaMA model.

You can modify the agent roles and system prompts for different learning scenarios (e.g., physics, coding, history).

# 📃 License
[MIT License](LICENSE.txt)

