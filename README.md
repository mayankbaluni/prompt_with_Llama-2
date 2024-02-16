# prompt_with_Llama-2
Prompt engineering is using natural language to produce a desired response from a large language model (LLM).

This interactive guide covers prompt engineering & best practices with Llama 2.

1 - Explicit Instructions
Detailed, explicit instructions produce better results than open-ended prompts:

* Stylization
    * Explain this to me like a topic on a children's educational network show teaching elementary students.
    * I'm a software engineer using large language models for summarization. Summarize the following text in under 250 words:
    * Give your answer like an old timey private investigator hunting down a case step by step.
* Formatting
    * Use bullet points.
    * Return as a JSON object.
    * Use less technical terms and help me apply it in my work in communications.
* Restrictions
    * Only use academic papers.
    * Never give sources older than 2020.
    * If you don't know the answer, say that you don't know.


2 - Zero-Shot Prompting
Large language models like Llama 2 are unique because they are capable of following instructions and producing responses without having previously seen an example of a task. Prompting without examples is called "zero-shot prompting".


Examples: Prompt: "Write a blog post about the latest trends in social media marketing for small businesses."

Prompt: "Explain the basics of using generative AI in digital marketing in a simple, easy-to-understand way."


3 - Few-Shot Prompting
Adding specific examples of your desired output generally results in more accurate, consistent output. This technique is called "few-shot prompting".

Example: Content Creation: Blog Post about Social Media Marketing for Small Businesses
* Example 1: "Here's a blog post about how small businesses can leverage Instagram for growth."
* Example 2: "This is an article discussing the benefits of Facebook advertising for local businesses."
* Prompt: "Now, write a blog post about the latest trends in social media marketing for small businesses."

Example: Educational Material: Basics of Generative AI in Digital Marketing
* Example 1: "Here's a simple explanation of how AI is used in data analysis."
* Example 2: "This is an easy-to-understand overview of AI in customer service automation."
* Prompt: "Explain the basics of using generative AI in digital marketing in a simple, easy-to-understand way."


4 - Role Prompting
Llama 2 will often give more consistent responses when given a role. 

Example: Prompt: "As a social media influencer with a large following in the health and wellness space, suggest creative ways to use Instagram for building a brand presence."

Prompt: "Imagine you are a successful entrepreneur who has built multiple businesses. Share your top five strategies for effective time management and productivity."


5 - Chain-of-Thought
Simply adding a phrase encouraging step-by-step thinking "significantly improves the ability of large language models to perform complex reasoning

Example: Add this to any prompt ”Let's think through this carefully, step by step.”


6- Self-Consistency
Self-Consistency  introduces enhanced accuracy by selecting the most frequent answer from multiple generations.

Think of self-consistency in AI like asking a group of experts the same question and then seeing what most of them agree on. The AI gives several answers to one question, and then we look for the answer that pops up most often. It's like believing what the majority says, assuming that if most experts (or in this case, AI responses) agree on something, it's probably the most accurate or reliable answer.

Example: Prompt: "Provide five separate recommendations for pricing a new AI-powered educational tool for entrepreneurs. Determine the most frequently suggested price range from these recommendations."


7 - Retrieval-Augmented Generation
Retrieval-Augmented Generation (RAG) is a technique where AI enhances its responses by first gathering information from a large database of texts and then using that information to answer questions or generate content.

Prompt:  Research the latest models of electric cars released in 2024. Compare their features, prices, and consumer reviews, and suggest the best options for city commuters.
