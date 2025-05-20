# Research-On-LLM-s
 Enhancing Algorithmic Reasoning in Language Models Using In-Context Learning

 
## Phase 1 ✅
   In the first phase, I focused on studying the main research paper: Teaching Algorithmic Reasoning via In-context Learning, along with related works that build on or reference it. I created a summary to better understand the paper’s motivation, the core problem it addresses, and the proposed prompting strategies for improving algorithmic reasoning in language models. This background search helped me understand the problem statement better before starting with the practical phase.

## Phase 2 ✅
   Next, I moved to the practical side of the research by working in Google Colab. I tested the six prompting techniques discussed in the papers using the GSM8K dataset. These techniques aim to improve the reasoning ability of language models by structuring prompts in different ways. The goal was to compare their effects on model performance and identify which methods work best for arithmetic and logical reasoning tasks.

## Phase 3 ✅
   In this phase, I used OpenAI’s vector embedding model text-embedding-ada-002 to embed a set of basic arithmetic word problems. Then, for a new question, I searched for the most similar example from the embedded set. The retrieved example was included in the prompt to help the model solve the new question. This approach was tested to see if giving the model an example from the embedded file would help the model generate a more accurate response.

## Phase 4
   The current phase involves extending the logic from Phase 3 to the GSM8K dataset. The plan is to first create a baseline by evaluating how well the model performs on 500 GSM8K test questions with no additional context. Then, we will use embeddings from 4000 GSM8K training examples to retrieve similar problems for each test question. By comparing the performance with and without similar prompts, we can see how much retrieval improves reasoning on more complex tasks.
