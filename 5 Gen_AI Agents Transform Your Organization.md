# Module 1:

## A brief history of agents

There are generally two kinds of agents: deterministic and generative. So those agents that you described can be referred to as traditional or deterministic agents.

A deterministic agent is an agent that is based on predefined paths and actions. It is typically workflow-based and event-driven, and it offers a high degree of control and predictability. 

Today’s generative AI agents can achieve a goal by observing the world and acting upon it using the tools it has at its disposal. This wasn't always the case. Early virtual agents were limited to predefined paths and lacked true understanding. But thanks to advances like generative AI and retrieval augmented generation (RAG), today's agents can understand your intent, access relevant information, and provide much more helpful and natural interactions. All due to the connections of the three components of an agent.

## Review the components of an agent

1. **Foundational model**

This is the underlying language model (LLM) that powers the agent. It could be a small or large language model, a Google model like Gemini, or a model from another provider. The key is to select a model with training data relevant to the agent's intended use case.

2. **Tools**

Tools enable the agent to interact with the outside world. These can include extensions that connect to APIs, functions that act as mock API calls, and data stores like vector databases. Tools allow the agent to not only observe the world but also act upon it.

3. **Reasoning loop**

This is the core of the agent, responsible for making decisions and taking actions. It's an iterative process where the agent considers its goal, the available tools, and the information it has gathered. Frameworks like ReAct (Reason and Act) are commonly used to guide the reasoning process.


## Using models
Keep in mind that generative AI agents are powered by generative AI models. These models are the brains of the operation.

Previous courses in this learning path have covered aspects of building and tuning AI models. In this lesson, we will focus on how to effectively use your gen AI model in your agent.

Once your AI models are trained and ready to go, there are still ways to improve your desired results. One such way is by adjusting certain parameters and settings.

## Sampling parameters and settings
Sampling parameters act as settings that influence the AI model's behavior, giving you more customized results. Think of these as knobs and dials you can adjust with your prompt input to impact the model's output. By tweaking these settings, you can ensure the model's output aligns with your specific needs, whether it's generating more creative text, providing more concise summaries, or staying within a certain tone.

Let's explore some of the most common parameters you can adjust.

1. **Token count**

Imagine each word and punctuation mark in your text as a character. These characters are grouped into smaller units called tokens, which represent meaningful chunks of text. Models have limits on how many tokens they can handle at once. A higher token count allows for longer and more complex conversations, but it also requires more processing power. For example, one token is roughly equivalent to four characters in English. So, a hundred tokens would be about sixty to eighty words.

2. **Temperature**

This parameter controls the "creativity" of the model, because it adjusts the randomness of word choices during text generation, influencing the diversity and unpredictability of the output. A higher temperature makes the output more random and unpredictable, while a lower temperature makes it more focused, deterministic and repeatable.

3. **Top-p (nucleus sampling)**

"Top-p" stands for the cumulative probability of the most likely tokens considered during text generation. This is another way to control the randomness of the model's output. It concentrates the probability on the most likely tokens, making the output more coherent and relevant. A lower top-p value leads to more focused responses (i.e. only the most probable tokens), while a higher value allows for more diversity (i.e. extending to lower probability tokens as well).

4. **Safety settings**

These settings allow you to filter out potentially harmful or inappropriate content from the model's output. You can adjust the level of filtering based on your specific needs and preferences.

5. **Output length**

This determines the maximum length of the generated text. You can set it to a specific number of words or characters or allow the model to generate text until it reaches a natural stopping point.

By experimenting with these parameters, you can significantly influence the AI model's behavior. For example, if you need a concise and factual answer, you might use a lower temperature and a smaller output length. If you're looking for a more creative and open-ended response, you could increase the temperature and top-p values.

## Adding prompt engineering to your reasoning loops

## The reasoning loop
The reasoning loop is a key component of a generative AI agent that governs how the agent takes in information, performs internal reasoning, and uses that reasoning to inform its next action or decision. It is an iterative, introspective process that continues until the agent achieves its goal or reaches a stopping point. The complexity of the reasoning loop can vary greatly depending on the agent and the task it is performing.

The key aspects of the reasoning loop:

1. Iterative process
    - The reasoning loop is not a one-time operation, but rather a cyclical process where the agent continuously evaluates its progress and determines the next best action to take. This loop involves steps for action, tool selection, and observation.

2. Internal reasoning
    - The agent uses its underlying language model to think through the steps it needs to take to complete a task. The language model provides the agent with reasoning and logic capabilities.

3. Decision making
    - Based on its internal reasoning, the agent decides on the next course of action. This involves choosing the appropriate tools to use and determining the necessary inputs for those tools.

4. Reasoning frameworks
    - The reasoning loop utilizes various prompt engineering frameworks and techniques to guide its reasoning and planning.

## Prompt engineering techniques
There are many different prompting techniques that one can use, but we will highlight two of the most common for this course: ReAct prompting and chain-of-thought (CoT) prompting.

**ReAct prompting**
- ReAct is a prompting framework that allows the language model to reason and take action on a user query, with or without in-context examples.

**Chain-of-thought (CoT)**
- Chain-of-thought prompting is a technique where you guide a language model through a problem-solving process by providing examples with intermediate reasoning steps, helping it learn to approach new problems in a more structured and logical wa

## ReAct prompting
ReAct, which stands for "reasoning and acting," is like giving an LLM a brain and a pair of hands. It allows the LLM to not only think about a problem but also take actions to solve it. This is a big step up from traditional prompting, where the LLM could only passively generate text.

Imagine you're asking an LLM to find you a good Italian restaurant nearby. With ReAct, the LLM can:

1. **Think:** Okay, I need to find Italian restaurants that are close by and have good reviews.
2. **Act:** I'll search online for Italian restaurants in this area.
3. **Observe:** Ah, here are some options with high ratings.
4. **Think:** Which one is the best fit based on the user's preferences?
5. **Act:** I'll check the menus and see which one has the most appealing dishes.
6. **Observe:** This one has delicious-looking pasta!
7. **Respond:** I recommend [restaurant name]. It has great reviews, is located nearby, and has a fantastic pasta selection.

This "thought-action-observation" loop allows the LLM to interact with the real world and gather information, making it much more powerful than a traditional LLM.

## Why is ReAct important?
- **Dynamic problem solving:** ReAct allows LLMs to tackle complex tasks that require interacting with external resources and adapting to new information.
- **Reduced hallucination:** By grounding the LLM's reasoning in real-world data, ReAct can help reduce the risk of generating incorrect or nonsensical information.
- **Increased trustworthiness:** The ability to see the LLM's reasoning process and how it interacts with external sources makes its responses more transparent and trustworthy.

## Key components of ReAct
- **Think:** The LLM generates a thought about the problem, similar to CoT.
- **Act:** The LLM decides what action to take, such as searching the web, accessing a database, or using a specific tool; the LLM specifies the input for the action, like a search query or database command.
- **Observe:** The LLM receives feedback from the action, such as search results or database entries.
- **Respond:** The LLM generates a response, which could involve providing an answer to the user, taking further actions, or formulating a new thought for the next iteration.

## ReAct in action
ReAct has been successfully used in various applications, including:
- **Question answering:** LLMs can use ReAct to access external knowledge sources and answer questions more accurately.
- **Fact verification:** LLMs can verify claims by searching for evidence online.
- **Decision making:** LLMs can use ReAct to gather information and make informed decisions in interactive environments.

The agent provides a prompt to the model, asking it to generate the next step and its corresponding output, which may include a thought, an action (including a tool choice), an action input, and an observation.

## Chain-of-thought (CoT)
Remember prompt chaining? Where you keep prompting in the same thread so the LLM keeps your chat history and learns more as you go? Well, you can do something very similar behind the scenes for your user using chain-of-thought (CoT) prompting. CoT enables reasoning capabilities through intermediate steps. 

Think of CoT as a way to make LLMs even smarter by teaching them to think step-by-step, just like a human would. Instead of just giving the LLM a prompt and expecting an answer, you guide it through the reasoning process. You provide examples of how to solve similar problems, showing the steps involved. This helps the LLM learn to approach problems in a more logical and structured way. It is similar to teaching a student to think out loud. You're teaching the LLM to think out loud. By showing it the intermediate steps, you're helping it develop a "chain of thought" that leads to the correct answer.

## Why is CoT important?
CoT is a powerful technique that helps LLMs think a bit more like humans. By guiding them through the reasoning process, we can unlock their full potential and achieve even more impressive results.
- **Improved reasoning:** CoT helps LLMs solve complex problems that require logical thinking.
- **Better accuracy:** By breaking down problems into smaller steps, CoT can lead to more accurate results.
- **Enhanced explainability:** CoT makes it easier to understand how the LLM arrived at an answer, which is important for building trust and transparency.

## Key components of CoT
Just like there are different ways to solve a problem, there are different ways to implement CoT. Some popular techniques include:
- **Self-consistency:** Encouraging the LLM to generate multiple solutions and choose the most consistent one.
- **Active-prompting:** Allowing the LLM to ask clarifying questions or request additional information.
- **Multimodal CoT:** Combining text with other forms of data, like images or videos, to enhance reasoning.

## CoT in action
Chain-of-thought prompting has been successfully used in various applications, including:
- **Complex reasoning tasks:** LLMs can use CoT to break down complex problems into smaller, more manageable steps, leading to more accurate solutions in tasks like math word problems or logical reasoning puzzles.  
- **Explanation generation:** LLMs can use CoT to generate step-by-step explanations for their answers, making their reasoning process transparent and understandable, which is crucial for building trust and identifying potential errors.
- **Multi-step planning:** LLMs can use CoT to plan and execute complex tasks that require multiple steps, such as writing a story, planning a trip, or debugging code.

## Choosing a prompting framework
There are many other frameworks and techniques that can be used for prompt engineering and within your reasoning loop. All these different techniques can be combined and leveraged in different ways depending on the use case. 

The best framework for you will depend on your use case. For example, while both ReAct and CoT enhance LLM reasoning, they have different strengths:
- CoT focuses on internal reasoning, guiding the LLM through a chain of thought.
- ReAct focuses on external interaction, allowing the LLM to gather information and take actions in the real world.

In fact, ReAct and CoT can be combined for even more powerful results. By integrating both techniques, we can create LLMs that are capable of both deep reasoning and dynamic interaction with the world around them.

## Q & a
- **Finding a highly-rated Italian restaurant near a current location.** ReAct as this would require reasoning and acting to get external information.
- **Summarizing a long article about the history of artificial intelligence.** CoT as this involves understanding and distilling information.
- **Brainstorming ideas for a new product.** CoT as this involves creative ideation, internal thought processes.
- **Searching for research papers on a particular scientific topic.** ReAct as this would require reasoning and acting to get external information from academic databases.

## Adding in tooling

## Types of agent tools
Agent tooling equips agents with the resources they need to be effective. Think of it as providing the agent with the right skills, connections, and knowledge to achieve its goals. These tools allow agents to access information, perform actions, and interact with various systems.

We can categorize agent tools into four key types.
- **Extensions (APIs)** 
    - Extensions bridge the gap between an agent and external APIs. APIs (application programming interfaces) are sets of rules that govern how software interacts. Extensions provide a standardized way for agents to use APIs, regardless of the API's specific design. This simplifies API interaction, making it easier for agents to access external services and data.
    - Example: An agent designed to book travel might use an extension to interact with a travel company’s API. The extension handles the complexities of communicating with travel company’s systems, allowing the agent to focus on the task of finding and booking flights.

- **Functions**
    - Functions are like specialized tools within the agent's toolbox. They represent specific actions the agent can perform. An agent's reasoning system selects the appropriate function based on the task at hand. Functions can encapsulate complex logic or interactions, making them reusable and manageable.
    - Example: A "calculate_price" function might take flight details and passenger information as input and return the total cost. The agent can call this function whenever it needs to calculate a price.

- **Data stores**
    - Data stores provide agents with access to information. This can include real-time data, historical data, or knowledge bases. Data stores ensure that the agent's responses are accurate, relevant, and up-to-date.
    - Example: An agent might use a data store to access current weather conditions, stock prices, or a database of customer information.

- **Plugins**
    - Plugins extend the agent's capabilities by adding new skills or integrations. They can connect the agent to specific services, provide access to specialized tools, or enable interaction with particular platforms.
    - Example: A plugin could enable an agent to interact with a calendar application, allowing it to schedule appointments. Another plugin might integrate with a payment gateway, enabling the agent to process transactions.

## How the reasoning loop works with tools
The ReAct (reasoning and acting) cycle prompting technique describes how agents use tools:
1. **Reasoning (tool selection)**
    - The agent analyzes the task and determines which tools are needed. It considers the available extensions, functions, and data stores to choose the most appropriate resources.
2. **Acting (tool execution)**
    - The agent executes the selected tool. This might involve calling an API via an extension, invoking a function, or querying a data store. The agent provides the necessary inputs to the tool.
3. **Observation**
    - The agent receives the output from the tool. This output becomes the "observation" in the ReAct cycle.
4. **Iteration (dynamic iteration)**
    - Based on the observation, the agent reasons about the next steps. It might need to select different tools, refine its approach, or gather more information. This cycle repeats until the task is complete.

## Example: Scheduling a garden consultation
- **Reasoning**
    - The agent needs to find an available time slot for a garden consultation. It selects the scheduling plugin, which integrates with the gardener's calendar.
- **Acting**
    - The agent uses the scheduling plugin to check the gardener's availability for the next week, specifying the desired consultation duration (e.g., 30 minutes) and the client's preferred days (e.g., weekdays). It also accesses the customer database (via a data store) to retrieve the client's name and contact information to include in the appointment details.
- **Observation**
    - The scheduling plugin returns a list of available time slots.
- **Iteration**
    - The agent presents the available slots to the client. If the client requests a specific time that's unavailable, the agent might use a function to suggest alternative times or offer to put the client on a waiting list. Once the client confirms a time, the agent uses the scheduling plugin again to book the appointment and sends a confirmation email to both the client and the gardener. This cycle continues until the consultation is successfully scheduled.

## Google’s tooling
Whether building your agents inside or outside of Google Cloud, the options for tooling are extensive. You can custom-build tools, leverage third-party solutions, or, as we'll focus on here, utilize the powerful suite of tools available within Google Cloud.

While this lesson won't cover every single Google Cloud product and feature, it will highlight some key options to spark ideas for the kinds of integrations you can create. It's important to note that many of these tools can be used even if you choose to build your core agent logic outside of Google Cloud.

## Key Google Cloud tool for agents
Here are some of the most relevant Google Cloud services for agent tooling:
- **Cloud Storage**
    - A highly scalable and durable object storage service. Use Cloud Storage to store and retrieve data that your agent needs.
- **Databases (Cloud SQL, Cloud Spanner, Firestore)**
    - Google Cloud offers a variety of database solutions to suit your needs. Your agent can use these databases to store and retrieve information, manage user data, or track its own progress.
- **Cloud Run functions**
    - Create serverless functions that act as specialized tools for your agent. Cloud Run functions can be used to connect to databases, call external APIs, perform complex calculations, or handle other specific tasks. They are easily triggered by your agent and scale automatically.
- **Cloud Run**
    - For more complex agent tools that require containerized environments, Cloud Run  provides a serverless platform for deploying and running stateless containers. This is ideal for custom tools that have specific dependencies or require more control.
- **Vertex AI**
    - Agents can use other agents as tooling. You can use Vertex AI to create models or agents that are called as tooling by other agents.

## Pre-built AI APIs
Along with these services, Google Cloud also offers a wide range of pre-built APIs that provide powerful functionalities for your agent. These APIs can be used for tasks like understanding natural language, analyzing images, translating text, and more.
- **Speech-to-Text API**
    - The Speech-to-Text API accurately converts speech into text. This is useful for transcribing meetings, customer service calls, or even video content.
- **Text-to-Speech API**
    - The Text-to-Speech API converts text into natural-sounding speech, which is helpful for creating voice user interfaces in devices and applications, and for personalized communication.
- **Translation API**
    - The Translation API can translate text, documents, websites, and even audio and video files into more than 135 languages.
- **Document Translation API**
    - The Document Translation API can translate formatted documents while keeping the original layout.
- **Document AI**
    - The Document AI API allows businesses to extract data from various document formats. It can be used to automate data capture and document processing. This is useful for many kinds of documents, from invoices to contracts to medical records. Document AI can also summarize large documents using generative AI.
- **Cloud Vision API**
    - The Cloud Vision API allows developers to understand the content of an image by applying powerful machine learning models. It can detect objects, faces, and landmarks, and even read text within images (OCR). This API is useful for a wide range of applications, including image tagging, content moderation, and visual search.
- **Cloud Video Intelligence API**
    - The Cloud Video Intelligence API allows developers to analyze video content and extract meaningful information. It can identify objects, actions, and events within a video, and even transcribe spoken words. This API can be used for applications like content recommendation, video search, and media analysis.
- **Natural Language API**
    - The Natural Language API helps derive insights from unstructured text using Google's machine learning. This API can be used to understand the sentiment of text, classify content, and extract important entities such as people, places, and events. This API can also analyze text in multiple languages.

## Other APIs
Google Cloud also offers a vast API Library with APIs linked to many other Google products such as Google Maps, Google Workspace, YouTube, Google Photos, and more. For additional information, check out the [API Library](https://console.cloud.google.com/apis/library).

## Agent tooling example: Meeting location planner
Scenario: A user uploads a document (e.g., a meeting invitation or a list of potential conference venues) and asks the agent to suggest the most convenient meeting location for attendees.

Using Document AI to understand document content and the Google Maps API for location analysis, the agent can provide users with helpful meeting location recommendations based on unstructured data.

1. **Document processing (Document AI API)**
    - The agent uses the Document AI API to process the uploaded document and identify addresses mentioned within the document.
2. **Geocoding (Google Maps Geocoding API)**
    - The agent takes the extracted addresses and uses the Google Maps Geocoding API to convert them into latitude and longitude coordinates to calculate distances and travel times
3. **Location analysis (custom logic)**
    - The agent uses custom logic implemented within a Cloud Function to analyze the geocoded addresses and determine a suggested location.

## Q & A
- **Extensions:** Connect to external services (via APIs).
- **Functions:** Define specific actions or tasks.
- **Data stores:** Provide access to information.
- **Plugins:** Add new skills and integrations

## Building applications from your agents

## Using the API

To use the API within your application, follow the directions for each tool:
- Google AI Studio: [Generate an API key](https://ai.google.dev/gemini-api/docs/quickstart?lang=python&_gl=1*137cca2*_ga*MTkwMzA3NTI4Ny4xNzMyNTg0ODcz*_ga_P1DBVKWT6V*MTczMjU4NDg3My4xLjEuMTczMjU4NTUyNy42MC4wLjYyODc0NTIyOQ)
- Vertex AI Studio: [Set up authentication & authorization](https://cloud.google.com/vertex-ai/generative-ai/docs/model-reference/inference)

Once you have your API or code, you can then leverage your agent within applications.
- **Cloud Run functions**
    - Small pieces of code that run in the cloud. They're triggered by specific events, like a new image being uploaded or a message being posted. You can use Cloud Run functions to automatically process these events using the Gemini API. For example, you could have a Cloud Run function that uses Gemini to automatically generate captions for uploaded images. The key benefit is that you don't have to manage any servers. Google takes care of all the infrastructure.
- **Cloud Run**
    - A service that lets you run your applications in containers. Containers are like self-contained packages that include everything your application needs to run. Cloud Run makes it easy to deploy and scale these containerized applications. This is useful for more complex applications that might require specific software or configurations. For example, you could use Cloud Run to host a web application that uses the Gemini API to power a sophisticated chatbot.

You can integrate the Gemini API into virtually any application that can make HTTP requests. This can be a wide range of environments, including web applications, mobile apps, desktop software, and even embedded systems.

You can also leverage your API or code through some of Google’s no code and low code tooling, such as:
- **Apps Script**
    - A cloud-based platform that lets you automate Google Workspace tasks by leveraging a combination of JavaScript code and Google's built-in services. You can use the Gemini API with Apps Script to build add-ons that enhance features in Google Workspace using generative AI.
- **AppSheet**
    - AppSheet is a no-code platform for building custom business apps. You can use Apps Script to extend the capabilities of your AppSheet applications using custom logic or by integrating APIs. With the Gemini API, for example, you can automate tasks, generate content, or provide intelligent assistance directly within your AppSheet app.

## Multi-agent applications​
When leveraging agents into your application, consider situations when you may need multiple agents.
- These systems utilize multiple agents, each potentially specialized for a specific task, to create more efficient and capable applications. For instance, a travel booking app might use one agent to search for flights, another to find hotels, and a third to suggest local attractions.
- These agents can work independently or interact with each other to provide a seamless booking experience. This modular approach not only improves efficiency but also allows for greater flexibility and scalability. Even more interestingly, an agent itself can be a tool within another agent. A sentiment analysis agent, for example, could be used by a customer service agent to gauge user satisfaction during an interaction.

# Module 2:

## Retrieval-augmented generation (RAG) and tooling
**Pre-RAG history**

Before retrieval-augmented generation (RAG), models could not directly learn from tool data. They could use tools to fetch information, but lacked the ability to process and integrate that data into their knowledge. Their understanding was limited to their training data, and tool-retrieved data was used only for the immediate query, not for learning. RAG solves this by enabling models to retrieve and learn from data provided by tools.

## How the model works with tools
Retrieval-augmented generation (RAG) enhances the capabilities of large language models (LLMs) by grounding their responses in external knowledge sources. This process allows the model to access and process information beyond its training data, leading to more accurate, relevant, and up-to-date responses.

After the user submits a query or request to the LLM, here's how RAG works with tools.
1. Retrieval
    - The LLM, equipped with retrieval tools, identifies relevant information from external sources. These tools can include:
        - **Data stores:** These can be internal databases or other sources of structured and unstructured data.
        - **Vector databases:** These databases store embeddings (numerical representations) of text, allowing the LLM to find semantically similar information to the user's query. The LLM uses the user query to create an embedding and searches the vector database for matching documents or passages.
        - **Search engines:** The LLM can use search engines (via extensions or APIs) to find relevant web pages, articles, or other online content.
        - **Knowledge graphs:** These structured databases store information about entities and their relationships. The LLM can query knowledge graphs to retrieve facts and relationships relevant to the user's query.
    - The LLM uses these tools to retrieve a set of potentially relevant documents or passages.
2. Augmentation
    - The retrieved information is then incorporated (or "augmented") into the prompt that is fed to the LLM. This augmented prompt now contains both the user's original query and the relevant context retrieved from external sources.
3. Generation
    - The LLM processes the augmented prompt and generates a response. Because the prompt includes relevant external information, the LLM can generate a more informed, accurate, and contextually appropriate response. It can also cite the sources of its information, increasing transparency and trustworthiness.

teration
In some RAG systems, the LLM might iterate on the retrieval process. For example, if the initial retrieval doesn't yield satisfactory results, the LLM might refine its query or use different retrieval tools to find more relevant information. It could also ask clarifying questions of the user. This iterative process allows the LLM to continuously improve the quality and relevance of its responses.

## Example: Answering a question about a recent event

1. **User query:** "What were the main developments at the recent climate conference in Dubai?"
2. **Retrieval:** The LLM uses a combination of tools:
    - It queries a vector database of news articles related to climate change.
    - It uses a search engine to find recent news reports and official conference documents.
3. **Augmentation:** The LLM combines the user's query with the retrieved information (summaries of key discussions, agreements, and announcements from the conference).
4. **Generation:** The LLM generates a response summarizing the main developments at the climate conference, citing the news articles and conference documents it used as sources. Because it has access to up-to-date information, the LLM's response is more accurate and comprehensive than if it had relied solely on its training data.
5. **Iteration (optional):** If the initial search results are insufficient, the LLM might try different search terms or query other data sources to get more complete information.

- By combining the power of LLMs with the ability to access and process external knowledge, RAG systems create more powerful and reliable AI agents.

## Data stores
RAG allows LLMs to access and process information beyond their training data, making them more accurate and relevant. A key component of this process are data stores in AI Applications. They act as structured and unstructured knowledge bases that your agent can draw upon.

You can access a variety of data store options to connect your agent to your data through AI Applications, including:
- **Websites:** Access and process information directly from web pages, enabling your agent to stay up-to-date with current events or access publicly available information.
- **Structured data:** Connect to information organized in tables or JSON format, such as product catalogs, customer databases, and internal knowledge bases. Vertex AI can automatically understand the structure of your data or allow you to define it.
- **Unstructured data:** Utilize files in various formats such as HTML, PDF, and DOCX, making it possible for your agent to access information from a wide range of sources.

## Try it: RAG in action
Test out using grounding with Google Search to see how RAG can impact outputs by providing more accurate and relevant information, drawing from real-time web data.
1. **Open Google AI Studio**
    - To begin experimenting with AI in Google AI Studio, complete the following steps:
        1. If you haven’t already, log into your Google account and open Google AI Studio. (Note: If prompted, you’ll need to accept the terms and conditions order to proceed.)
        2. Select Try Gemini.
2. **Run a prompt**
    1. Locate the prompt input area and Run button on the page. This is used to send your prompt to the Gemini model.
    2. Enter a prompt into the prompt input such as “What are the latest trends in generative AI?”.
    3. Press Run to generate a response to your prompt.
3. **Get grounded results**
    1. To activate grounding, go to Run settings > Tools and toggle on the Grounding using Google Search option.
    2. Re-enter the same prompt you just provided and press Run to generate a new result.

## The power of search agents

## Vertex AI Search
Vertex AI Search offers both search and recommendation solutions.

## Search solutions
Search allows you to create a powerful search experience for your public website. It can index and search across a variety of data types, including structured data in BigQuery and unstructured documents stored in Google Cloud Storage. This ensures your users can easily find the information they need on your website, regardless of how it's stored.

Search also extends to include some specific forms of search such as:
1. Document search
    - If your primary need is to search across a large repository of unstructured documents stored in Google Cloud Storage, this is the ideal solution. It's optimized for understanding and retrieving information from text-heavy data, making it perfect for internal knowledge bases, document archives, and more.
2. Media search
    - For organizations dealing with rich media libraries, media search provides specialized capabilities. It's designed to understand and search within images, videos, and audio files. This allows users to find specific media assets based on their content, metadata, or even spoken words within audio or video.
3. Healthcare search
    - Addressing the unique needs of the healthcare industry, this option enables searching across healthcare data while supporting regulatory compliance. It allows professionals to access patient records, research articles, and medical guidelines efficiently and securely.
4. Search for commerce
    - Specifically designed for e-commerce, this option focuses on building a search app for your retail catalog. It optimizes for product discovery, understanding product attributes, and handling complex product queries.

## Recommendation solutions
The general purpose recommendation engine can be used to recommend similar content within websites, documents, and other structured content. It analyzes user behavior and content attributes to provide personalized recommendations, increasing user engagement and content discovery.

This also extends to include some specific forms of recommendations such as:
1. Media recommendations
    - Tailored for consumer-focused media applications like audio/video streaming and digital publishing, this option provides specialized recommendations. It understands user preferences and consumption patterns within media content to suggest relevant audio, video, articles, and more.
2. Retail recommendations
    - Optimized for e-commerce, this solution drives sales by providing personalized product recommendations. It leverages user browsing history, purchase data, and product attributes to suggest items that are likely to be of interest to each individual shopper.

## How Vertex AI Search works
Regardless of the specific search or recommendation option you choose, Vertex AI Search operates on a foundation of intelligent data connection, grounding, and generative AI. It seamlessly connects to your existing data stores, whether they are structured databases, unstructured document repositories, or a combination of both. This connection is crucial as it allows Vertex AI Search to act as an agent, observing the user's query or context (the environment) and acting by retrieving relevant information or suggesting relevant items (using the data stores as tools) to achieve the goal of providing the right information or recommendation at the right time.

- A key strength of Vertex AI Search lies in its ability to ground gen AI LLM responses with your first-party data, curated third-party data, and even Google's knowledge graph (Grounding with Google Search), minimizing "hallucinations" and ensuring trustworthy information.
This grounding is where the connection to RAG comes in. By using your own data sources as the foundation for LLM responses, Vertex AI Search implements a RAG approach, ensuring that the information provided is relevant, accurate, and grounded in the context of your specific data.
- Vertex AI Search also gives you the options of adding extra generative AI features to your search functionality.
    - **Search summaries:** Vertex AI Search can generate concise and informative summaries of search results, saving users time and effort. These summaries can be tailored to different needs, providing a quick overview of a document, a comparison of multiple products, or a synthesis of key findings from a set of search results.
    - **Answers and follow ups:** Vertex AI Search can add AI generated answers to your search results. Users can ask questions in natural language to your website’s search and get AI generated answers based on the search results. Users can then follow up with further questions.
- Vertex AI Search is built for enterprise and offers granular access controls to help ensure data security. It also provides advanced analytics to understand search trends and user behavior and scalable infrastructure to handle large volumes of data and search requests. It's designed to meet the demanding requirements of organizations of all sizes. Vertex AI Search is built to easily integrate with existing enterprise systems through APIs and SDKs. Whether you're building a customer-facing search experience or an internal knowledge base for employees, Vertex AI Search can be seamlessly integrated into your workflow.

## Use case: Enhancing the shopping experience with Vertex AI Search
Let’s hear how Vertex AI Search is helping one forward-thinking clothing company create a more intuitive and personalized online shopping experience.
- The clothing company recognized that their existing search functionality was falling short. Customers struggled to find what they were looking for, often abandoning their searches in frustration.
- The challenge was twofold:
    - Traditional keyword search often failed to capture the nuances of customer intent, leading to irrelevant results. Think about how people describe clothing—they might use vague terms or focus on visual characteristics. 
- In a physical store, a sales associate can understand what a customer is looking for even if they don't know the exact name of the item. Online search was needed to bridge this gap.
- To address these challenges, the company turned to Vertex AI Search. This powerful tool leverages advanced AI and machine learning to understand customer intent and deliver highly relevant search results.
- Vertex AI Search goes beyond simple keyword matching. It understands the meaning behind search queries, including synonyms, related terms, and even misspellings, to deliver more accurate and comprehensive results. This means customers are more likely to find what they're looking for, even if they don't know the exact name of the product.
- One of the most exciting features is the AI-powered image search. Customers can now simply upload a photo of an item they like—perhaps an old favorite they're trying to replace, or a style they spotted on social media—and Vertex AI Search will find visually similar products in the company's current catalog. Imagine a customer taking a picture of their favorite worn-out sweater and instantly getting recommendations for similar styles and colors available now. This transforms how shoppers interact with the online store.
- Vertex AI Search retail recommendations learns from customer behavior, including past purchases, browsing history, and search queries, to provide personalized product recommendations. This helps customers discover new items they might love, increasing engagement and driving sales.
- The implementation of Vertex AI Search has yielded significant results for the clothing company. Customers are finding what they want more easily, leading to increased purchases. The enhanced search experience has resulted in happier and more loyal customers. Personalized recommendations and image search have encouraged customers to explore more products and spend more time on the website.
- This clothing company's transformation demonstrates the power of Vertex AI Search. By leveraging AI and machine learning, they were able to create a more intuitive, personalized, and engaging online shopping experience.

## Google’s Customer Engagement Suite
- Websites, even with the best search, are not necessarily enough for your company. Customers frequently don’t want to search. They want to connect with your company directly to get the answers and support they are looking for.
- These points of communication can be a pain point between customers and companies, but they are also an extremely important point of connection. Positive customer engagement could be the difference between the success and failure of your company.
- Google’s Customer Engagement Suite has tools designed to support your company in engaging with customers effectively. The tools are built using conversational AI, some of which is also generative AI.
- With the Customer Engagement Suite, you can build:
    1. Conversational Agents
        - Conversational Agents to act as effective chatbots communicating with your customers.
    2. Agent Assist
        - Agent Assist to support your live human contact center agents.
    3. Conversational Insights
        - Conversational Insights to gain insights into all your communications with customers (through chatbot agents or human agents).

All of this can be built on top of Google’s Contact Center as a Service (CCaaS), an enterprise-grade contact center solution that is native to the cloud. Let’s dive deeper into the details of how these all work and where generative AI fits in.

## Conversational Agents
- You may be a bit skeptical of customer service chatbots. But the types of conversational agents you can build today have come a long way.
- Remember, there are two primary methodologies you can use when building conversational agents: deterministic and generative.
- While deterministic AI alone can be rigid, and generative AI alone may lack structure, their combination creates a powerful solution. A hybrid approach allows you to build conversational agents that can handle a wide range of customer needs effectively.
- With Conversational Agents in Google Cloud, you have flexible options for building and integrating your agents with your existing tools. Create simple agents with generative AI by using natural language to instruct your agent or complex hybrid agents with custom rules and logic.
    1. Deterministic
        - Deterministic is more associated with some historical agents. It is a rule-based, very defined system for your chatbot agents to follow. It will use very defined logic such as if the user presses this number, go to this route. Everything you want a deterministic agent to do needs to be explicitly defined. Deterministic agents usually require low to medium code to build.
    2. Generative
        - Generative is based on new generative AI technology. It uses large language models to give a real conversational feel to your chatbot. These agents will determine what to do on their own based on your prompt unless you specifically tell it otherwise. Generative agents usually require prompting and either no code or low code to build.
    3. Hybrid
        - Google Cloud Conversational Agents empowers you to build hybrid agents that combine the strengths of deterministic and generative AI. This approach offers strict control while leveraging generative AI's flexibility to better address customer needs.

## Use case: Conversational agents 
Let’s explore how a company, Cymbal Retail, leveraged the generative AI tooling of Conversational Agents to build their personal shopping assistant for customers.

- Cymbal Taxes, a rapidly growing online tax preparation service, faced a challenge. Their customer base was expanding, but their customer service team was struggling to keep up with the increasing volume of inquiries during the busy tax season. They needed a solution that could provide instant, personalized support to their customers 24/7. 
- Cymbal Taxes turned to Conversational Agents to create a personalized tax assistant for their website and app. They used Conversational Agents to design an agent that could understand and respond to customer inquiries in a natural and engaging way.
- To ensure the AI assistant could access and process relevant information without needing every single potential conversational flow created, Cymbal Taxes integrated generative AI playbooks into their AI assistant with Conversational Agents.
- Generative playbooks allow them to give instructions in natural language for how they want the AI assistant to behave and connect it to their Vertex AI data store.
- The data store allows the assistant to tap into their vast knowledge base of tax laws, FAQs, and customer data. The AI assistant could now answer questions about specific tax forms, provide personalized advice based on a users’ tax situation, and even assist with filing and payment.
- Let’s see how that played out for Cymbal Taxes’ customers:
    - Customer: "Hi, I need help figuring out if I can claim my home office deduction."
    - AI assistant: "Sure, I can help with that. Can you tell me more about your home office setup? Do you use it exclusively for work, and what percentage of your home does it occupy?"
    - Customer: "I use it exclusively for work, and it takes up about 10% of my home."
    - AI assistant: "Great! Based on the information you provided, it sounds like you may be eligible for the home office deduction. However, there are a few other factors that could affect your eligibility, such as whether you are self-employed or an employee. Would you like to answer a few more questions to determine your eligibility for sure?"
    - Customer: "Yes, please."
    - AI assistant: "Great, based on your answers, it looks like you are eligible to claim the home office deduction. Would you like me to guide you through the process of calculating and claiming the deduction on your tax return?"
    - Customer: "I need to know the deadline to file my taxes."
    - AI assistant: "The deadline to file your federal income tax return is April 15. However, if you need more time, you can file for an extension until October 15. Keep in mind that an extension only gives you more time to file, not to pay any taxes owed."
- With the AI assistant in place, Cymbal Taxes saw a significant improvement in customer satisfaction. Their net promoter score (NPS) jumped by 15 points, with customers praising the speed and helpfulness of the assistant in post-interaction surveys. The customer service team reported a 20% reduction in call volume and a 30% decrease in email inquiries, freeing them to focus on more complex issues like handling tax audits and addressing customer complaints. The AI assistant also proved to be a valuable tool for increasing customer engagement and retention.
- Cymbal Taxes' success story demonstrates how Conversational Agents empower businesses to create truly personalized customer experiences. By leveraging the power of natural language understanding and accurate information retrieval, companies can build AI assistants that not only enhance customer satisfaction but also drive tangible business results.

**Agent Assist**

There will always be use cases where conversational agents are not enough or tricky situations where the human touch is needed. This is where live agents come in. But using human agents comes with its own challenges. Not all human agents are the same and they have different levels of experience. There can be a lot of training needed, especially when a new agent starts.

This is where Agent Assist comes in. It is a tool that supports live human agents with in-the-moment assistance, generated responses, and real-time coaching to help them resolve customer issues faster and with greater accuracy. Using AI and generative AI, Agent Assist can recommend agent responses to customers, suggest the appropriate knowledge base content to solve a customer’s issue, transcribe or translate calls in real time, summarize conversations and more.

**Conversational Insights**

Whether using live or virtual agents, these connections with your customers provide lots of value and insights for your company. Conversational Insights analyzes conversational data from across the customer journey to provide contact center leaders and managers with the data-driven insights to boost efficiency, improve agent performance, and create better customer experiences. This tool uses machine learning analytics to provide you with information such as agent and caller sentiment, entity identification, and call topics. It can automatically identify interesting customer interactions in need of further review.

With Generative FAQ in Insights, you can also see the common questions that customers are asking your contact center and how these questions are being answered. This information can help you identify gaps in your FAQs, track trending questions, and improve customer service responses.

**Contact center as a service (CCaaS)**

Today's contact centers are complex, needing to handle 24/7 communication across multiple channels (phone, text, email, etc.) while maintaining security and customer privacy.

CCaaS, part of Google's Customer Engagement suite, simplifies this by providing a complete contact center solution. It manages the infrastructure, integrates with CRMs, and offers omnichannel support (consistent experience across all channels, like websites, apps, phone, and text). CCaaS handles simultaneous multichannel communication, channel switching, multimodal interactions (text, voice, images), and agent routing, freeing businesses to focus on customer experience. CCaaS seamlessly integrates with other Customer Engagement Suite tools, including Conversational Agents for automated support, Agent Assist for real-time agent guidance, and Conversational Insights for valuable data analysis.

## Q & A

- **Conversational Agents:** Uses deterministic and generative AI.
- **Agent Assist:** Supports live human agents.
- **Conversational Insights:** Analyzes customer sentiment.
- **CCaaS (Contact Center as a Service):** Provides omnichannel support.

## Build your own agent (optional exercise)

**Creating playbooks**
When building a generative AI agent with Conversational Agents, you create what is called a playbook for how you want your agent to act. In the playbook, you define your agent's goal, such as providing customer support, answering user questions, or even generating creative content. You then provide detailed instructions on how the agent should act and any rules you would like it to follow. In the playbook, you also have the option to link it to external tools such as data stores. Once your playbook is defined, you are ready to go and can start testing your agent and interacting with it.

## Try it: Build your own agent
Cymbal Manufacturing is a leading producer of high-quality machinery. The company wants to implement an AI-powered chatbot on their website to assist customers with common inquiries, provide product information, and offer basic troubleshooting.

In this activity you learn to use Google AI Studio to build a context-aware chatbot. You explore how to define the chatbot's persona, knowledge, and behavior using system instructions, focusing on a use case for Cymbal Manufacturing.

**STEP 1: Understanding system instructions in Google AI Studio**

- Go to Google AI Studio via aistudio.google.com. 
- Chat should be pre-selected in the left-hand options menu. If it's not, you'll need to select it.
- At the top, select select System instructions. (Note: The icon may resemble a clipboard or assignment).

Why are system instructions important?

With system instructions, you can provide context, persona, and constraints to an LLM before any user input is provided to guide the model's behavior and ensure its responses align with your desired outcome.
- Consistency: Ensure the chatbot maintains a consistent tone and persona.
- Accuracy: Ground the model in specific knowledge, reducing hallucinations.
- Relevance: Keep responses focused on the intended domain (e.g., Cymbal Manufacturing).
- Safety: Prevent the model from generating inappropriate or unhelpful content.

**STEP 2: Add your own system instructions** 

In this activity, instead of directly building a virtual agent that answers customer service questions, you're building an AI that helps developers create other virtual agents. Complete the following steps to get started:
- In the System Instructions input box, paste the following prompt to create the expert system instruction writer:

You are an expert at building virtual agent assistants. For the provided company, role, and other information, provide a system prompt that a developer can use. You always fulfill the user's request to the best of your ability. Create a distinct goal and set of instructions for this system prompt.
- In the left panel, select Enable save to allow your work to be saved as you make changes.
- Then, at the top, select Save (represented by a floppy disk icon. Provide a Prompt name like Agent instruction writer, and then click Save again.

**STEP 3: Prompt to request a system prompt for your conversational agent**

Now, within your Agent instruction writer, enter a prompt at the bottom to request a system prompt for Cymbal Manufacturing’s conversational agent. Here is a prompt you can use:

```text
Your task: Build a system prompt for a virtual agent optimized for an LLM that would be appropriate for to assist an end user with the following job:

End user’s company: Cymbal Manufacturing

Use case to be developed: Cymbal Manufacturing builds storage containers primarily. However, Cymbal is also capable of doing custom machining based on request. If the user needs custom machining done, they should call the company directly. You may answer any question which seems reasonable within the scope of container manufacturing, but do not take too many guesses. Our containers are typically blue or green, but they can occasionally be red. Make sure to always keep a respectful tone and admit when you don’t know the answer to a user’s question. Cymbal’s phone number is (333) 333-3333.
```

Then select Run. Then select Save.

You now have a goal and instructions for your Cymbal Manufacturing chatbot.

**STEP 4: Create your Cymbal Manufacturing chatbot using the system prompt**

Copy the system prompt output from Step 3 above, which includes the goal and instructions for your Cymbal Manufacturing chatbot. In the lefthand menu, under Library, select the Cymbal Manufacturing chatbot you created in Step 1.

Paste the system prompt output into the System Instructions for the Cymbal Manufacturing chatbot.

Select Save.

**STEP 5: Test your conversational agent**

In the prompt box at the bottom of your Cymbal Manufacturing chatbot, write different prompts to converse with the Cymbal Manufacturing conversational agent, selecting “Run” as needed.

List of things you can try:

•  Say hello.
•  Ask about the storage container product such as the color or size.
•  Ask about custom manufacturing.
•  Ask about something completely random like the weather.

Note: Remember this is a very basic sample of a conversational agent and how you might start to create one. It does not represent the depth of a fully developed agent using a tool such as Conversational Agents.

**Tip**

You may not realize it, but you actually were using a prompting technique called metaprompting in this lesson. In steps two and three, you generated the prompt that you then used as the system instructions for your final conversational agent. Metaprompting is about creating prompts that guide the AI to generate, modify, or interpret other prompts.

Metaprompting is a powerful tool for interacting with AI, enabling more dynamic, flexible, and adaptable prompt creation and interpretation. It's a key technique for unlocking the full potential of large language models.

## Agentspace
One of the most powerful ways to transform your organization isn’t necessarily through products for your external customers, but actually through supporting your internal knowledge workers and employees.

Often, employees search across multiple sources for information within their organization. Examples of such sources include software used for analytics, productivity, content, customer relationship management, communications, portfolio management, supply chain, and enterprise planning.

One way to support knowledge workers is by making information across your enterprise more discoverable.

Google Agentspace is designed to help you and your team use your company's information more effectively. It uses AI to create customized agents that can access and understand data from various sources, regardless of where that data is stored. These agents can then be integrated into your organization’s internal websites or dashboards. Think of it as a way to give your employees their own personal research assistants, but for work.

## Google Agentspace use case
Let’s explore how Google Agentspace can help a personal wealth management advisor generate new trade ideas and effortlessly conduct deep research on a trending topic.

First, I'll ask Agentspace to search for recent reports put out by my company, Cymbal Investments.

In seconds, Agentspace has searched all its available data sources, including connected apps, Cymbal-curated data stores, the Cymbal internet and public websites.

It surfaces a few PDF reports stored in SharePoint, and I can click to see the full set of results. Keep in mind that Agentspace respects ACLs and will only show me data I have access to.

I'm interested in the first three, so let's go ahead and add them as context for the agent to reference throughout the session.

Now I'll ask Agentspace to summarize and compare these reports, highlighting any key market indicators.

The top themes are clearly outlined with the option to view the specific sources for each point. Very interesting.

Now I am wondering how these findings might impact how I advise my client, Rohit.

I've started keeping NotebookLM notebooks of client notes. So let's go ahead and attach Rohit's to the session. The notebook’s been added and I can open it directly in Agentspace to verify its contents. As expected, this one contains our notes from two meetings in December.

Now let's have Agentspace evaluate how, based on what we've talked about in the past, the report findings might impact Rohit's investment plan. Tying back to the reports, I see that Rohit's European and Canadian investments have been underperforming and given the latest outlook, he is light in Japan.

I also see that Rohit's daughter is starting private school. This was mentioned in the meeting notes contained in the attached notebook. With that I can adjust my recommendations worksheet and have Agentspace validate my approach.

Cymbal’s Custom Client analytics tool gives Agentspace access to client portfolio data. Let's use that tool and have Agentspace compare Rohit's current portfolio to my recommendation as outlined in the local spreadsheet I'm about to upload.

The answer shows my recommendation means bumping Japan and pulling back in the U.S. and Canada. There's even a generated chart letting me see the changes at a glance.

Next, I want to think through the impact of any rebalancing before I make a recommendation to Rohit. Luckily, Cymbal has approved mathematical models that can assist with these types of calculations, highlighting things like exposure and risk.

Let's go ahead and ask for the analysis using the Cymbal Risk Calculator tool. The custom calculator sends back chart and table data, including balance simulators and expected annual returns. I feel good about the recommendations, so let's ask Agentspace to draft an email to the client and find time for us to meet to discuss it next week. Agentspace drafts a detailed outlook email with the recommendation, rationale and summary of the trades. I can edit as I see fit and send it off directly from Agentspace. And the same goes for sending a meeting invite.

Now let's use Agentspace for something a bit different. There's a lot happening in the news with U.S. tariffs on Mexico and Canada, and I'd like to draft a report on the subject. First, I'm going to limit the data sources Agentspace uses for this task. Let's have it focus on a few curated sources, including a custom repository of government reports. 

With the sources set, let's ask Agentspace to draft the report. This prompt kicks off a deep research process. Given the task, the agent generates a plan for itself and presents it to me for verification. Once confirmed, the agent searches thousands of sources to find answers to its questions and comes up with new questions along the way based on its findings. Once satisfied, the agent generates a detailed report, complete with source links and an accompanying audio summary.

As you can see, partnering with Agentspace helps financial advisors optimize their workflows, increase efficiency, and improve client outcomes.

## Agentspace is a launch point for all your enterprise-ready expert agents.

- **Connect to NotebookLM Enterprise**
    - Connect to NotebookLM Enterprise so employees can upload information to analyze, get insights, and listen to audio summaries of data.
- **Connect to multimodal search agents**
    - Connect to multimodal search agents grounded in your data (structured and unstructured) across multiple systems (Google Drive, Confluence, Jira, ServiceNow, and more) so your employees can find relevant information within your company.
- **Add generative AI assistants**
    - Add generative AI assistants that are grounded in your enterprise data and can be prompted to take actions through connectors (tools). For example, creating Google Calendar events or editing issues in Jira Cloud.
- **Add custom agents**
    - Add custom agents through Conversational Agents.

## How is Agentspace different from NotebookLM? 
While Agentspace can connect to NotebookLM Enterprise, they serve different core purposes. Think of NotebookLM Enterprise as your specialized AI tool for diving deep into specific documents and web sources – asking questions, summarizing, and creating new content based only on those sources. Agentspace, on the other hand, is your comprehensive enterprise AI assistant. It uses AI agents and unified search to automate tasks and find information across all your connected business systems, not just specific documents you upload.

## Strategy: Planning ahead

## Plan for generative AI integration
To effectively integrate gen AI into your organization, consider the following key steps:

- **Establish a clear vision**
    - Define how gen AI integrates with your overall corporate strategy. Secure buy-in from leadership and appoint a champion to drive adoption.
- **Prioritize high-impact use cases**
    - Focus on opportunities that align with business goals, considering factors like technical feasibility, data readiness, and potential for transformation.
- **Invest in capabilities**
    - 
Develop the necessary skills within your organization through a combination of upskilling, recruitment, and training. Foster a culture of learning and experimentation to empower teams to leverage gen AI effectively.
- **Drive organizational change**
    - Proactively manage the shifts in workflows, roles, and mindsets that accompany gen AI implementation. Encourage agile collaboration and knowledge sharing to scale best practices.
- **Measure and demonstrate value**
    - Track, measure, and assess the impact of gen AI initiatives. Use data-driven insights to continuously improve and demonstrate the value of your efforts.
- **Champion responsible AI**
    - Develop and implement a robust framework for responsible AI, ensuring fairness, transparency, privacy, and security in all generative AI initiatives.

## Plan for impact
We have discussed the importance of measuring and demonstrating value from gen AI projects, but until now, we haven’t really discussed how.

- **Define key metrics**
    - Start by identifying the metrics most relevant to your goals. Are you aiming for a return on investment (ROI), increased revenue, reduced costs, improved efficiency, enhanced customer experience, or improved security? 
    - The key is to select metrics that align with your overall business objectives. If it’s a return on investment (ROI) that’s important to your organization, calculate the financial benefits of your gen AI initiatives against their costs. If it’s increased revenue, measure the direct impact of gen AI on sales and profits.
- **Collect and analyze data**
    - Once you've defined your key metrics, it's time to gather data. Set up tracking mechanisms, conduct surveys, or analyze existing data to understand the impact of your gen AI initiatives. 
    - For example, if you're tracking customer experience, you might compare satisfaction scores before and after implementing a gen AI powered chatbot. Look for patterns and trends to identify areas where gen AI is making a difference.
- Iterate and improve
    - The beauty of gen AI is its adaptability. Use the insights from your data analysis to refine your gen AI strategy and optimize performance. If you're not seeing the desired ROI, consider why you aren't seeing the desired ROI, what are the practical issues or pain points? Then adjust your approach. This may include fine-tuning your models, updating training data, improving prompting techniques, or integrating gen AI more effectively into your workflows.

## Plan for change
Even when your gen AI solutions are working and successful, you still need to be prepared to adapt. Technology is constantly changing with new models, tools, and techniques emerging rapidly. Your customers and employees expect you to keep up.

Staying up-to-date requires a proactive approach to learning and development. It also entails fostering a culture of continuous learning and improvement within your organization. Here are some tips on the best ways to stay ahead of the curve with gen AI.
- **Regularly review and refine your strategy** based on the latest advancements and your organization's specific needs.  
- **Stay informed** about new models, tools, and techniques by actively following industry news, research publications, and expert opinions.  
- **Engage with the generative AI community** through conferences, workshops, and online forums to learn from others and share your knowledge. 
- **Invest in training and development** programs to upskill your workforce and equip them with the knowledge and skills needed to thrive in the generative AI era.  
- **Attract and retain top talent** by creating a stimulating and rewarding work environment that fosters creativity and professional growth.  

