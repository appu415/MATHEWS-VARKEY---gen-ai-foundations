# Question 1: The Vector Conflict

Yes, the similarity score can sometimes be higher than expected even when the word "light" is used with completely different meanings. This happens because a basic CountVectorizer only looks at how often words appear and does not understand their actual meaning. Since both sentences contain the word "light", the vectors share common features, which increases the dot product score. In other words, the model sees matching words but cannot recognize that one sentence is talking about something lightweight while the other is talking about illumination.

# Question 2: The Context Blindspot

From a Data Science perspective, the bag-of-words approach has a major limitation because it ignores context and word order. Every word is treated as an independent count, so the model cannot understand the relationship between words in a sentence. This makes it difficult to build intelligent search engines or chatbots because they need to understand what users actually mean, not just which words they use. The key linguistic property that is lost is semantic meaning, which is essential for understanding natural language.

# Question 3: The GenAI Architectural Fix

Modern Large Language Models such as GPT and LLaMA overcome this limitation by creating context-aware embeddings instead of relying on simple word counts. Through self-attention mechanisms, the model examines surrounding words and learns how each word contributes to the meaning of the sentence. Because of this, the word "light" can have completely different vector representations depending on whether it refers to brightness, weight, or health-related qualities. This ability to understand context allows LLMs to generate more accurate responses and better capture the true meaning of language.
