# Analyz - Visual Studio Code Extension

Analyz a Code Buddy is a powerful Visual Studio Code extension designed to assist developers during coding sessions, providing real-time code analysis and helpful suggestions for better understanding and efficient coding. Leveraging the Mistral Instruct model fine-tuned on a dataset of over 200 rows, this extension offers comprehensive support for various programming languages and scenarios. With seamless integration into Visual Studio Code, it delivers a user-friendly experience, allowing developers to optimize their code structure and enhance overall coding efficiency. 

# Functionality

### Chatbot

Analyz is a chatbot created to assist users and make coding simpler, readily available right within the vscode. The chatbot is designed to understand what you're asking, generate helpful code snippets, and provide useful information. It uses the Mistral 7b finetuned model, ensuring it generate responses that suit your specific needs.

https://github.com/srujan-landeri/Analyz-VSCode-Extension-Demo/assets/66351075/a52c1560-d510-4abf-b289-e6e0e0f1b340

### Algorithm Complexity Analysis

Algorithm Analysis is one such metric every programmer uses to know how well the function is. Analyz makes this easy, by providing insights on every function by providing the time and space complexity along with suggestions on how can the function be improved further with just a single click.

https://github.com/srujan-landeri/Analyz-VSCode-Extension-Demo/assets/66351075/df498062-df7c-48eb-b37b-ab61bed8e490

### Code Converter

Analyz simplifies the code conversion by allowing users to modify their code directly from within the editor. This user-friendly feature supports programming languages, compatible with more than 70 languages. For increased accuracy and versatility, Analyz leverages the power of OpenAI, ensuring that your code changes are accurate. 

https://github.com/srujan-landeri/Analyz-VSCode-Extension-Demo/assets/66351075/f23e1f3d-71b0-4a3d-9330-c699dec12698

### Flowcharts

The flowchart functionality in Analyz is unique and distinctive. Unlike GPT, Analyz can create flowcharts, offering unique capabilities by using OpenAI. Analyz can effectively create flowcharts to help users understand concepts easily.

https://github.com/srujan-landeri/Analyz-VSCode-Extension-Demo/assets/66351075/a014e466-f8b3-4414-b76d-c7e4b8e71f26

# Fine-tuned model

🔗https://huggingface.co/RachitD15673/mistral-finetuned-7B-instruct-manual

**Fine-Tuned Mistral 7B Model**

In this repository, we detail the process through which the Mistral 7B language model was fine-tuned using a specialized dataset sourced from the Algorithms repository on GitHub.

**Fine-Tuning Process Overview**

The fine-tuning was accomplished by employing the QLoRA (Query-specific LORA) technique, a method that efficiently adapts large language models to new tasks with minimal parameter updates.

**Steps of Fine-Tuning with QLoRA:**

1. *Dataset Acquisition*:
   - We procured a custom dataset of algorithmic content from TheAlgoritms GitHub repository, which provided diverse coding problems and their algorithmic solutions.

2. *Preprocessing*:
   - The dataset underwent preprocessing to structure it appropriately for the model, involving tokenization and formatting suitable for the Mistral 7B's input requirements.

3. *QLoRA Configuration*:
   - We configured QLoRA by specifying the additional parameters to be introduced to the model’s attention mechanism, specifically targeting the query matrices.

4. *Model Initialization*:
   - The pre-trained Mistral 7B model was loaded, and QLoRA was integrated, allowing for efficient fine-tuning without extensive retraining of the original model parameters.

5. *Training*:
   - The training loop, tailored for the QLoRA-augmented model, optimized the newly introduced parameters using the prepared dataset, focusing the model's learning on algorithmic patterns and intricacies.

6. *Validation*:
   - Post-training, the model was evaluated against a set of algorithmic problems it had not seen before to ensure it had effectively learned from the fine-tuning process.

7. *Model Saving*:
   - With fine-tuning complete and the model achieving a high level of performance on algorithmic content, we saved the enhanced model, encapsulating the QLoRA adjustments.

The fine-tuning process allowed us to maintain the breadth of knowledge inherent to Mistral 7B while refining its expertise to understand and generate algorithmic code effectively.
