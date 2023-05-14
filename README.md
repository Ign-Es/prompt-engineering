# Prompt Engineering for Devs
These are my notes from the "ChatGPT Prompt Engineering for Developers" course offered by OpenAI & DeepLearningAI

## Two types of Large Language Models (LLMs)
* __Base LLM__: 
Predict the next word based on text training data. 
* __Instruction Tuned LLM__: Tries to follow instructions. Fine-tune on instructions and good attempts at following them.

Models like ChatGPT start as a BaseLLM and then is further trained as an Instruction Tuned LLM, fine tuned with Reinforced Learning with Human Feedback(RLHF).

Treat those models as a very intelligent person, but not a mind reader. If the output is not what you wanted, then you need better instructions (usually). Be clear and specific.

## Guidelines
### Principles
1. Write clear and specific instructions.
    1. Use delimiters such as:
        * Triple quotes """
        * Triple backticks ```
        * Triple dashes ---
        * Angle brackets <>
        * XML tags \<tag>\</tag>
    2. Ask for structured output.
    3. Check whether conditions are satisfied.
    4. Few-shot prompting: give succesful examples of completing tasks, then asks the model to perform the task.
2. Give the model time to think.
    1. Specify the steps required to complete a task.
    2.  Instruct the model to work out its own solution before rushing to a conclusion

### Limitations
The model can "Hallucinate" when you give them a task that is plausible but is not actually "real". For example when you ask it to describe a fake product from real company.

## Iterative Process 
Generating a succesful prompt is an iterative process. 
![Iterative Process](images/iterative_process.png)

