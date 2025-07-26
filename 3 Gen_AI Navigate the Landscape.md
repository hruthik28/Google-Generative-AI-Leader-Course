# Module 1:

## The building blocks of generative AI
Generative AI is a powerful technology composed of interconnected layers, each playing a vital role in its capabilities. Let's explore these layers—from the foundational infrastructure to the user-facing applications

Gen AI as being composed of five layers. 
1. infrastructure
2. models
3. platform
4. agents
5. gen AI powered applications.

- **Gen AI powered application layer** is The user-facing part of generative AI, or the frontend. This is the layer that allows users to interact with and leverage the capabilities of AI. Examples of gen AI powered applications include the Gemini app, Gemini for Workspace, or NotebookLM.  

- **Agent layer** An agent is a piece of software that learns how to best achieve a goal based on inputs and tools available to it. This layer focuses on autonomous action, which describes the ability to independently set goals and carry them out within a defined environment. Agents analyze situations, use multiple tools, and make informed decisions without requiring constant human input. They are also capable of handling multi-step tasks that a model alone cannot, such as researching a topic, troubleshooting code, or accessing a system by chaining together actions. You can have a variety of agents, such as customer agents, code agents, data agents, and many more.  

- **Platform layer** typically sits between agents and models, providing the infrastructure for them to interact. For now, let's jump ahead and focus on the models themselves, and we'll come back to platforms shortly. 

- The "brain" of the agent is the **AI model**. These models are complex algorithms trained on vast amounts of data. They learn patterns and relationships in the data, allowing them to generate new content, translate languages, answer questions, and much more.  

- **Infrastructure layer** is the foundation upon which everything else rests. It provides the core computing resources needed for generative AI. This includes the physical hardware (like servers, GPUs, and TPUs) and software needed to store and run AI models and training data. 

- **Platform layer** sits above the model and infrastructure layers, providing the necessary tools and infrastructure for AI development. It offers APIs, data management capabilities, and model deployment tools. This layer acts as the backbone of the system, bridging the gap between models and agents while simplifying the complexities of managing the underlying infrastructure. 

From the foundational infrastructure to the user-friendly applications, each layer of generative AI plays a crucial role in its capabilities. 

## Agents and gen AI powered applications

- Gen AI agents can process information, reason over complex concepts, and take actions. They can also be used in a variety of applications, including customer service, employee productivity, and creative tasks.

- A gen AI agent is an application that tries to achieve a goal by observing the world and acting upon it using the tools it has at its disposal.

- With generative AI, you have the flexibility to leverage either pre-built agents and applications, or create custom ones tailored to your specific needs. No matter which path you choose, you can apply generative AI's capabilities in a way that best aligns with your objectives.

- Google Cloud tools like AI Applications help teams create AI agents using natural language rather than having to write complex code to do the same thing.

## Agents relate to gen AI powered applications
Think of agents as the intelligent pieces within a larger gen AI powered application. They bring specific capabilities to the table.

1. **Understanding and responding to natural language**
This allows applications to have more intuitive interfaces, like chatbots that can actually understand complex requests.

2. **Automating complex tasks**
Agents can handle multi-step processes within an application, such as gathering information, making decisions based on that information, and taking action.

3. **Personalization**
Agents can learn user preferences and tailor the application experience accordingly.

## Role of agents in gen AI powered applications
Think of gen AI powered applications as the user-facing layer. They provide the structure and context for agents to operate within. They define the user interface, the overall goals, and the specific tasks that agents will help with. Often, multiple agents with different specializations work together within a single application to create a richer, more dynamic user experience. This is known as a multi-agent system. You can review some examples below.

1. **A travel booking app**
An agent could handle the complex task of finding the best flights and hotels based on user preferences, while another agent might specialize in suggesting relevant activities and attractions at the destination. Then, the application provides the user with the interface for browsing options and making reservations.

2. **A customer support app**
An agent could answer common questions, troubleshoot problems, and escalate complex issues to human representatives. The application would provide the chat interface and integrate with other support systems.

3. **A personalized learning app**
An agent could assess a student's knowledge, recommend relevant learning materials, and even generate personalized exercises. The application would provide the structure for lessons and track progress.

## How agents work 
**Conversational and workflow agents**

While there are many ways to use gen AI agents, most will fall under two categories:
1. Conversational agents 
2. Workflow agents.

## Conversational agents

**How it works**

Conversational agents are designed to understand what you mean, not just what you say, and respond in a way that makes sense. 

- **You provide input:** You can type a message or speak to the agent.
- **The agent understands:** Using powerful AI, it figures out the meaning and intention behind your words.
- **The agent calls a tool:** Based on your request, the agent might need to gather additional information or perform an action.This could involve searching the web, accessing a database, or interacting with another software application.
- **The agent generates a response:** It formulates an answer that's relevant to your request and sounds natural.
- **The agent delivers the response:** You'll see or hear the answer depending on how you interacted with it.

**Examples**

- **Answering questions:** Imagine you're curious about the weather in Paris. You ask a conversational agent, "What's the weather like in Paris?" And it instantly provides you with the current temperature, forecast, and even suggests what to pack if you're traveling there.
- **Casual conversation:** Feeling bored? A conversational agent can engage in lighthearted banter, tell you jokes, or even discuss your favorite books and movies, just like a friend would.
- **Accessing information:** Need to know the capital of Australia? Or maybe you want a quick summary of the French Revolution? A conversational agent can access a vast amount of world knowledge and provide you with concise and accurate information.

## Workflow agents

**How it works**

Workflow agents are designed to streamline your work and make sure things get done efficiently and correctly by automating tasks or going through complex processes.

- **You provide input:** You define a task or trigger a process like submitting a form, uploading a file, initiating a scheduled event, or even ordering a product online.
- **The agent understands:** The agent is the software that automates those steps. It interprets the task's requirements and defines the series of steps needed to complete the task.
- **The agent calls a tool:** Based on the workflow's definition, the agent executes a series of actions. This could involve data transformation, file transfer, sending notifications, integrating with external systems, or initiating other automated processes using APIs.
- **The agent generates a result/output:** It compiles the outcome of the executed actions, which might be a report, a data file, a confirmation message, or an updated status within a system.
- **The agent delivers the result/output:** The agent delivers the output to the designated recipient(s) or system(s), such as via email, a dashboard, a database update, or a file storage location.

**Examples**

- **Ecommerce order fulfillment:** An agent automatically processes orders, updates inventory, sends shipping notifications, and handles returns.
- **Customer onboarding:** An agent guides new customers through account setup, provides tutorials, and answers frequently asked questions.
- **Automated research:** An agent can conduct in-depth research on a given topic by autonomously browsing the web, summarizing relevant content, and generating comprehensive reports. (Try this out with Gemini Deep Research.)
- **Security Log Parsing:** An agent that inspects incoming security logs for abnormalities and can flag them, open a ticket, begin triage, and assign to humans for review when necessary.

## Agent use cases
Both conversational and workflow agents can cover a broad range of use cases:

1. **Customer service agents** can answer questions, resolve issues, and provide personalized recommendations.

2. **Employee productivity agents** can help workers find information, manage tasks, and automate workflows.

3. **Creative agents** can generate new ideas, create content, and translate languages.

4. **Code agents** can assist developers in writing, reviewing, and debugging code, and even generating code from natural language descriptions.

5. **Data agents** can analyze large datasets, identify trends, and extract insights from data.

6. **Security agents** can automate tasks like summarizing case information, researching threats, generating security-related queries, and even taking actions like creating detection rules.

## Gen AI agents: Beyond just models
Agents incorporate things like the reasoning loop and tools to become dynamic problem solvers and tackle complex tasks that go beyond the capabilities of standard language models.

- AI agents are designed to observe, act, and achieve goals. While AI agents utilize models, they represent a significant leap beyond their capabilities.  

- Agents incorporate two key elements that distinguish them from standalone models: a reasoning loop and tools. The reasoning loop is the agent's "thinking process." It's a continuous cycle of observing, interpreting, planning, and acting. This iterative process enables agents to analyze situations, plan actions, and adapt based on outcomes.  

- Tools are functionalities that allow the agent to interact with its environment. Tools can be anything from accessing and processing data to interacting with software applications or even physical robots. This empowers agents to connect with real-world information and services, much like apps on our phones.  

- For example, an agent could use tools to: Access and update a company's inventory. Schedule meetings by checking calendars. Automatically order new supplies when stock is low. Or communicate with a robot’s sensors and actuators.  

- By combining reasoning and tools, AI agents transcend the limitations of large language models (LLMs). They move beyond text generation to solve complex problems, manage multi-step tasks and produce results beyond just text or media. When solving complex problems, agents analyze information, gather data using tools, and make informed decisions with minimal human intervention. 

- When managing multi-step tasks, agents excel at complex workflows that LLMs alone can't handle, such as: conducting in-depth research, troubleshooting code, and automating tasks across multiple systems.  

- The reasoning loop is the heart of an AI agent's operation. It's an iterative process where the agent:  

- **Observes:** Gathers information about its environment and the task at hand. 
**Interprets:** Processes the information and assesses the current situation. 
**Plans:** Plans a course of action to achieve its goal. 
**Acts:** Executes the planned action.  

- This loop continues until the agent reaches its goal or a stopping point. The complexity of the loop varies depending on the agent and its task. Some agents have simple, rule-based processes, while others use more complex logic, potentially involving additional algorithms or probabilistic reasoning.

## Advanced prompt engineering frameworks
The reasoning loop often utilizes advanced prompt engineering frameworks to guide its decision-making process. These frameworks can include:

- Simple rule-based calculations
- Complex thought chains
- Machine learning algorithms
- Probabilistic reasoning techniques

Examples of such frameworks include ReAct or chain-of-thought (CoT) prompting, which we discuss in more detail in Course 5 of this learning path.

# Module 2:

## 1. The platform layer

## Key features and benefits of Vertex AI

The platform layer provides the foundation for building and scaling your AI initiatives. 

Vertex AI is Google Cloud's unified machine learning (ML) platform designed to streamline the entire ML workflow. It provides the infrastructure, tools, and pre-trained models you need to build, deploy, and manage your ML and generative AI solutions.

1. **Open and flexible**

Vertex AI supports open frameworks, allowing you to use your preferred tools and models without vendor lock-in.

2. **Powerful infrastructure**

Leverage Google Cloud's scalable and reliable infrastructure to handle your ML workloads.

3. **Pre-trained models**

Choose from a wide variety of pre-trained models or build your own.

4. **Comprehensive tooling**

Develop, deploy, and manage your models with ease using Vertex AI's integrated tools.

5. **Customization**

Fine-tune and adapt models to your specific needs using the built-in IDE.

6. **Easy integration**

Integrate your models into applications seamlessly using available APIs.

## MLOps for efficient workflows
Operationalizing model training can be challenging and involves thinking about infrastructure and security. By using Vertex AI, you get a fully managed compute infrastructure, high-performance ML optimized training jobs, distributed training, hyperparameter optimization, and enterprise security.

## Vertex AI's MLOps tools
Vertex AI also includes ML operations (MLOps) tools built in to help you orchestrate end-to-end ML workflows, perform feature engineering, run experiments, manage and iterate your models, track ML metadata, and monitor and evaluate model quality. MLOps helps automate, standardize, and manage the ML project lifecycle, enabling better collaboration and continuous improvement.

1. **Feature store**

Share, serve, and reuse ML features to maintain consistency and efficiency.

2. **Model registry**

Manage model versions, track changes, and organize your models throughout their lifecycle.

3. **Model evaluation**

Quickly evaluate and compare model performance to identify the best model for your use case.

4. **Workflow orchestration**

Automate ML workflows, from data preprocessing to deployment, using Vertex AI Pipelines.

5. **Model monitoring**

Monitor models for performance degradation, detect input skew and drift, and trigger updates or retraining.

## 2. The model layer

**What is an AI model?**

At the heart of every AI and machine learning system lies the model. Think of it as the brain of the operation. These aren't just any algorithms. They're sophisticated mathematical structures trained on massive amounts of data. This training process allows them to learn patterns and relationships, ultimately enabling them to perform a wide range of tasks, such as generating content, analyzing data, and classifying information.

## Vertex AI: A model hub

Within the Vertex AI platform, you have multiple options for how to handle AI models for your project. You can choose to build a model from scratch or use an existing model.

**Use models with Model Garden**

For many use cases, your organization won’t need to develop a new model. There are many AI models that already exist today that you can fine-tune and leverage for so many different use cases. Model Garden on Vertex AI is a service that lets you discover, customize, and deploy existing models from Google and Google partners.

Model Garden gives you options to pick from over 160 models and offers options of Google models, third-party models, and open-source models. With Vertex AI, you can customize these models with your own data and deploy them to your custom applications. Additionally, some pre-trained models can be used out-of-the-box without tuning.

1. **First-party foundation models**

Leverage state-of-the-art models from Google including Gemini models and task-specific models for image generation, speech-to-text, and more.

- Gemini Pro, Flash, and more. [View Gemini specs](https://cloud.google.com/vertex-ai/generative-ai/docs/models#gemini-models)
- Imagen for text-to-image. [View Imagen specs](https://cloud.google.com/vertex-ai/generative-ai/docs/image/overview)
- Veo for text-to-video and image-to-video. [View Veo specs](https://cloud.google.com/vertex-ai/generative-ai/docs/model-reference/veo-video-generation)
- Chirp 2.0 for speech-to-text. [View Chirp specs](https://cloud.google.com/vertex-ai/generative-ai/docs/speech/speech-to-text)

2. **First-party pre-trained APIs**

Build and deploy AI applications faster with our pre-trained APIs powered by the best Google AI research and technology.

- [View Speech-to-Text specs](https://cloud.google.com/speech-to-text?hl=en) 
- [View Natural Language Processing (NLP) specs](https://cloud.google.com/natural-language?hl=en)
- [View Translation specs](https://cloud.google.com/translate?hl=en)
- [View Vision specs](https://cloud.google.com/vision?hl=en)

3. **Open models**

Access a variety of enterprise-ready open models.

- [View Gemma 2 specs](https://console.cloud.google.com/vertex-ai/publishers/google/model-garden/gemma2)
- [View CodeGemma specs](https://console.cloud.google.com/vertex-ai/publishers/google/model-garden/codegemma)
- [View PaliGemma specs](https://console.cloud.google.com/vertex-ai/publishers/google/model-garden/paligemma)
- [View Meta's Llama 3.1 specs](https://cloud.google.com/blog/products/ai-machine-learning/llama-3-1-on-vertex-ai) 
- [View Meta's Llama 3.2 specs](https://cloud.google.com/blog/products/ai-machine-learning/llama-3-2-metas-new-generation-models-vertex-ai)
- [View Mistral AI specs](https://cloud.google.com/blog/products/ai-machine-learning/codestral-and-mistral-large-v2-on-vertex-ai)
- [View Mistral AI21specs](https://console.cloud.google.com/vertex-ai/publishers/ai21/model-garden/jamba-1.5-large)
- TII's Falcon BERT, FLAN-T5, ViT, EfficientNet. - [View TII's Falcon specs](https://www.tii.ae/)

4. **Third-party models**

Model Garden supports third-party models from partners with foundation models.

[View Anthropic's Claude Model Family specs](https://console.cloud.google.com/vertex-ai/model-garden?pageState=%28%22galleryStateKey%22:%28%22f%22:%28%22g%22:%5B%22providers%22%5D,%22o%22:%5B%22ANTHROPIC%22%5D%29,%22s%22:%22%22%29%29)

## Build models with Vertex AI

With Vertex AI, you have two options for training and using your own models. You can go fully custom and create and train models at scale using any ML framework (PyTorch, TensorFlow, scikit-learn, or XGBoost), or you can use AutoML to create and train models with minimal technical knowledge and effort.

AutoML allows you to build these types of models:

|Data type|Supported objectives|
|---------|--------------------|
|Image data|Classification, object detection.|
|Video data|Action recognition, classification, object tracking.|
|Text data|Classification, entity extraction, sentiment analysis.|
|Tabular data|Classification/regression, forecasting.|

**Follow this standard workflow when creating your models in Vertex AI.**

1. **Gather your data**

Determine the data you need for training and testing your model based on the outcome you want to achieve.

2. **Prepare your data**

Make sure your data is properly formatted and labeled.

3. **Train**

Set parameters and build your model.

4. **Manage your model**

Review model metrics to evaluate the model’s performance and monitor changes over time.

5. **Deploy and predict**

Make your model available to use.

## Generative AI in action: a manufacturing use case

- Cymbal Aerospace, a manufacturer of critical jet engine components, faced a challenge: their vast library of 3D CAD models held a wealth of vital information, but accessing it was a time-consuming and inefficient process. Let's explore how they leveraged generative AI on Vertex AI to overcome this obstacle and transform their operations. Cymbal Aerospace faced a challenge familiar to many manufacturers: extracting critical information from complex 3D CAD models was a tedious and error-prone process. Engineers struggled to quickly access details like material composition, dimensions, and stress points, hindering their ability to efficiently design, analyze, and manufacture components. This manual and time-consuming workflow hindered their efficiency and increased the risk of errors.

- To overcome this challenge, Cymbal Aerospace decided to build a custom generative AI solution that could analyze 3D CAD models to automatically generate concise summaries or answer questions. They did this by using a two-layered approach, combining the power of AutoML and Gemini within Vertex AI. First, they leveraged AutoML, which streamlined the process of training a machine-learning model capable of extracting key metadata from the CAD files. This eliminated the need for deep machine-learning expertise, allowing Cymbal Aerospace to quickly build a powerful and specialized model tailored to their specific needs. This custom AutoML model acted as an intelligent interpreter, capable of understanding the intricacies of the CAD files and identifying critical information such as material composition, dimensions, and tolerances.

- To further enhance the usability of this information, they integrated Gemini within Vertex AI using MLOps tools like Vertex AI Pipelines. Gemini transformed the raw metadata extracted by the AutoML model into clear, concise, and insightful summaries in natural language. This allowed engineers to easily understand and interpret the information, facilitating faster and more informed decision-making. For example, an engineer could ask the system, "What is the tensile strength of the turbine blade?" and receive an immediate, understandable, and accurate answer extracted from the complex CAD file.

- By using Vertex AI, Cymbal Aerospace was able to simplify model development. Vertex AI's AutoML handles the complexities of model training, making it easy for the company to build a high-performing model without needing deep machine-learning expertise. Customize solutions: The company was able to train a model tailored to their specific needs and data, ensuring accurate and relevant summaries. Scale efficiently: Vertex AI provides the infrastructure to deploy and scale the generative AI model, enabling the company to process large volumes of CAD files quickly and efficiently. And streamline deployment: The company easily deployed its models using a serverless infrastructure. Vertex AI handled key machine-learning operations (MLOps), such as scaling and infrastructure management, which allowed the company's employees to focus on model and application development.

- With the generative AI solution deployed on Vertex AI, Cymbal Aerospace experienced significant improvements. Product development cycles accelerated by 15%, design review times were reduced by 20%, and manufacturing planning bottlenecks were eliminated. This faster time-to-market allowed them to respond more rapidly to customer demands and introduce innovative products ahead of their competitors. Cymbal Aerospace is using generative AI to transform their manufacturing process. By using Vertex AI, companies can unlock the power of generative AI to streamline workflows, improve decision-making, and drive innovation.

## 3. The infrastructure layer

## The foundation of gen AI solutions

- The "infrastructure layer" is the foundation upon which any AI system is built. It's the combination of hardware and software that provides the necessary computing power, storage, and networking capabilities to train, deploy, and scale AI models. This layer is crucial for handling the massive datasets and complex computations involved in modern AI, especially with the rise of large language models and generative AI.

- Google has invested heavily in building a robust and cutting-edge AI infrastructure, designed to handle the most demanding AI workloads. Here are some key components.

## High performance computing

Imagine your company wants to undertake a new, bold gen AI project. However, the engineering team hits a major roadblock. Training the complex model requires significant processing power, far beyond the capabilities of your company's in-house servers. It takes hours, if not days, to train your specialized models and the long training times have started to hinder the team's progress to the point where it's delaying the product launch. Your existing infrastructure simply can't keep up, and the cost of scaling their own hardware is prohibitive. This is where high-performance computing, the heart of Google's AI infrastructure, comes in.

1. **GPUs and TPUs**

These specialized processors are the workhorses of AI. They excel at parallel processing, or doing multiple things at once, which is crucial for training large neural networks quickly and efficiently. GPUs were originally designed for graphics rendering, but since they offer general-purpose parallel processing power they’ve increasingly been used in the AI domain. TPUs are Google's custom-designed chips specifically optimized for AI tasks.

2. **Hypercomputers**

A hypercomputer is essentially a supercomputer built by connecting many individual computers (nodes) together. These nodes contain GPUs and TPUs. By linking them with high-speed networks, they work together as one massive computing unit. They provide the massive scale necessary for training and running the most demanding generative AI models.

## High performance storage

Having high-performance storage is essential when building gen AI apps. Gen AI models are data hungry because they learn by analyzing massive datasets, often petabytes in size, containing text, images, code, and other forms of data. This storage provides the capacity and speed to store and access these enormous datasets efficiently. Without it, training would be incredibly slow or even impossible.

1. **Large-scale storage systems**

Google Cloud's storage infrastructure is optimized for AI workloads, offering high throughput (the amount of work done within a specific period of time), scalability, and the ability to create dense compute clusters for faster training and inference. As AI models and datasets grow, the system can scale seamlessly to accommodate the increasing demands. Losing data due to storage failures can be catastrophic, so the storage is highly reliable to ensure data durability.

2. **Fast storage access**

The storage systems also need to provide fast read and write speeds to keep up with the demands of the training process. Otherwise, if storage access is slow, it can significantly hinder the training process.

## Networking

- Fast and efficient communication is essential for coordinating the work all of the processors in a high performance computing cluster are undertaking. Google's global fiber network provides high-bandwidth, low-latency connectivity, ensuring smooth data flow and efficient communication between different parts of the AI infrastructure.

- Using Google Cloud infrastructure can benefit teams in several ways, particularly with respect to scalability, performance, and cost-effectiveness.

# Module 3:

## AI on the edge

**Edge computing**

- While hosting infrastructure on the cloud is powerful, it's not always the ideal solution. Imagine a self-driving car needing to make split-second decisions. It can't wait for data to travel to the cloud and back. That's where edge computing comes in.

- Google provides the tools to deploy your AI models in these different locations, giving you more control and flexibility.

- Edge computing runs AI on devices or servers closer to the data source or point of need.

## Why go local or edge?

- Imagine a drone navigating a complex environment. It needs to react instantly to obstacles, making cloud processing too slow. Running AI locally on the drone ensures real-time responsiveness. Other benefits include increased data privacy and reduced reliance on internet connectivity.

- To run powerful AI models on edge devices and mobile phones, Google provides tools like Lite Runtime (LiteRT). Think of LiteRT as a platform that helps machine learning models work efficiently on your device. To learn more about Google's high-performance runtime for on-device AI, check out the article, Lite Runtime (LiteRT) Overview. 

- One example of an AI model designed for edge is Gemini Nano.

## **Gemini Nano**

- Gemini Nano is Google's most efficient and compact AI model, specifically designed to run on the edge on devices like smartphones and embedded systems. It's part of the larger Gemini family of models. Think of Gemini Nano as a miniature version of the powerful AI that usually lives in Google's data centers. This "on-device" or edge approach offers several benefits.

    1. **Privacy**

    Your data stays on your device, enhancing your privacy.

    2. **Speed**

    You get fast responses since there's no need to send data to the cloud.

    3. **Offline Access**

    Gemini Nano can work even without an internet connection.

- Gemini Nano brings the power of AI directly to your devices, making them smarter, more helpful, and more privacy-focused. It is currently being integrated into various Google products and services, including:

    1. **Pixel phones**

        Gemini Nano powers features like Call Notes, which summarizes phone conversations and Pixel Recorder, which summarizes voice recordings.
    
    2. **Android**

        Gemini Nano is available to Android developers through the AI Edge SDK, enabling them to build innovative AI experiences into their apps.

Even when your goal is to deploy on the edge, Vertex AI provides a powerful platform for building, training, and refining your models. You can leverage Vertex AI's capabilities for tasks like data preparation, model training, tuning, model evaluation, collaboration, and MLOps.

Once your model is ready for the edge, Vertex AI offers tools to streamline the deployment process.

You can:

- **Convert models:** Convert your models to Lite Runtime (LiteRT) for optimal performance on edge devices.

- **Package and deploy:** Package your models and dependencies into containers for deployment on various edge hardware.

- **Manage and monitor:** Manage your edge deployments, track their performance, and gather insights to improve your models over time.

Google provides the tools to deploy your AI models in these different locations, giving you more control and flexibility.

## Gen AI project resources: People, cost, and time


## Roles and responsibilities

- It is important to understand the resources you have available to build out your solution. Let’s dig deeper into some of the roles and responsibilities at each layer of the stack. 

- The AI stack is designed to support different roles with specific needs. Before jumping into building out a solution, ensure you have the proper expertise and talent for what you want to build. Business users can improve their tasks, developers can build custom AI solutions, and AI practitioners can develop and deploy advanced AI models responsibly and securely. This collaborative ecosystem allows your organization to leverage the full potential of AI across various business functions.

1. **Business leaders**

    Business leaders typically interact with pre-built gen AI solutions to enhance daily operations and improve customer experiences. For example, Gemini for Google Workspace can be used for content creation, data analysis, and document summarization.

2. **Developers**
    Developers in your organization are responsible for building and deploying custom AI agents and integrating AI capabilities into existing applications. They can use AI Applications for custom agent creation, AI code generation, and AI-driven data processing. Developers can also leverage pre-trained APIs to rapidly integrate AI into applications, or they can use the Vertex AI platform which is designed to help developers build and deploy AI agents with tools for orchestration, grounding, and action.

3. **AI practitioners**
    AI practitioners play a valuable role in customizing, deploying, and optimizing generative AI models. They leverage tools within Vertex AI to accelerate development and ensure responsible AI practices. Their expertise extends to scaling AI workloads, integrating models with BigQuery, and implementing responsible AI measures such as bias detection and adversarial testing.

## Cost

The pricing model of gen AI can vary based on which part of the gen AI landscape you are looking at or even which specific product or company you are using. It is important to have a realistic budget and understanding of the cost for your project.

When building gen AI solutions, you pay for three primary activities:

- Training the model.
- Deploying the model to an endpoint.
- Using the model to make predictions.

Training and deploying models often involve paying for the compute time used as well as the storage for the training data and model outputs.

## Pricing for using models

1. **Usage-based**

    You pay for the amount you use, often measured in tokens or characters processed. This is common for APIs like Google’s PaLM & Gemini APIs.

2. **Subscription-based**
    
    You pay a recurring fee for access to the model, often with tiers based on usage limits or features.

3. **Licensing fees**
    
    One-time or recurring fees for using a model, especially for commercial purposes or embedding in products.

4. **Free tiers**
    
    Some providers offer free access with limited usage for experimentation or non-commercial purposes.

## Pricing metrics for using models

Here are some metrics you may see for usage-based pricing models.

1. **Tokens**

A token represents a piece of text, like a word or part of a word.

2. **Characters**

Some providers, like Google, charge based on the number of characters processed.

3. **Requests**

Sometimes you can be charged per request, regardless of the complexity or volume of the task.

4. **Compute time**

The time taken to process your requests can also factor into the cost, especially for resource-intensive tasks.

## Factors affecting cost 

Here are some factors affecting cost when using models.

1. **Model size and complexity**

Larger, more capable models generally cost more.

2. **Context window**

A larger context window (the amount of text the model can consider) can increase costs.

3. **Features**

Specialized features like fine-tuning or embedding can have separate pricing.

4. **Deployment**

Depending on where you deploy your model and application, you may have compute based costs.

## Time

It probably won’t surprise you to learn that the more custom your solution is, the more time and resources it takes to build. Using a prebuilt gen AI application takes seconds. Building your own custom solution with a custom AI model, can take months. Choosing to build a custom agent with AI Applications takes much less time. 

Think about your project timelines and evaluate them against your needs and requirements. Determine if the timeline is realistic based on your requirements.

## Gen AI solution needs

## Scale
Is this for individual use, a small team, a large company, or millions of customers?

1. **Small scale**

As an individual user or small team, you can go very far with pre-built tools. Try to leverage existing gen AI powered applications.

2. **Large scale**

When building out solutions for millions of customers, you'll likely need a more robust and customized solution. Pick solutions that offer scalability and security. Factor in details to your decision like infrastructure costs, data storage, and potential latency challenges.

## Customization

How specialized does your solution need to be? Powerful foundation models are constantly improving, making custom model development less necessary in many cases.

1. **Start with existing models**

Explore pre-trained models available through APIs or open-source libraries. Fine-tune these models on your specific data to achieve better performance for your tasks.

2. **Identify your unique needs**

What sets your project apart? Does it require specialized knowledge, handle complex tasks, or demand a unique user experience? This will help you determine the level of customization needed.

3. **Consider data specificity**

If your project deals with specialized domains like law or medicine, consider fine-tuning with domain-specific datasets or exploring models specifically trained for those areas.

4. **Consider task complexity**

Think about the complexity of the task itself. Are you aiming for simple tasks like text summarization or more intricate ones like code generation or creative writing? This influences model choice and training approaches.


## User interaction

Think about how users will interact with your AI and design an intuitive and engaging experience.

1. **User interface (UI)**

Seamlessly integrate the AI into your existing workflows. This might involve a dedicated interface (e.g., a chatbot widget on your website) or embedding AI capabilities within your current applications.

2. **User experience (UX)**

Aim for a user-friendly experience. Is it conversational, informative, or task-oriented? Consider the level of guidance and feedback users might need.

## Privacy

How sensitive is the data you are working with?

1. **Data security**

What measures will you implement to protect data during processing and storage? Implement robust security measures to protect data during processing and storage. Consider encryption, access controls, and secure data centers.

2. **Compliance**

Are there specific regulations (GDPR, HIPAA, etc.) that your project needs to adhere to?

## Other considerations

How specialized does your solution need to be? Powerful foundation models are constantly improving, making custom model development less necessary in many cases.

1. **Latency**

What are the acceptable response time limits?

Tip: Consider real-time requirements. Do you need instantaneous responses, or can you tolerate some delay? If real-time interaction isn't critical, you have more flexibility in choosing models and infrastructure.

2. **Connectivity**

Will the solution always have internet access?

Tip: Consider offline functionality. Are there scenarios where the solution needs to function without internet access?

3. **Accuracy**

How crucial is the accuracy of the AI's output? What are the acceptable error tolerances?

Tip: Define acceptable tolerances. Determine the level of accuracy required for your AI's output. This will influence model selection, training data, and evaluation metrics.

4. **Explainability**

Do you need to understand the reasoning behind the AI's decisions? 

Tip: Transparency is key. In certain domains, understanding the AI's reasoning is crucial. Consider using models or techniques that offer explainability features, especially in healthcare or finance.

## Making decisions

You understand your needs and resources. Now it’s time to make decisions such as what model you will use. By carefully considering the factors covered below and conducting thorough research, you can make informed decisions about gen AI pricing and choose the most cost-effective solution for your needs.

**1. Comparing different companies and models**
- **Evaluate model capabilities:** Look for benchmarks and comparisons to assess the quality and performance of different models.
- **Compare pricing structures:** Consider your expected usage and calculate the costs based on the pricing models and metrics of each provider.
- **Factor in additional costs:** Account for potential costs like data storage, API calls, and fine-tuning.
- **Read the fine print:** Pay attention to usage limits, data privacy policies, and other terms of service.

**2. Key resources for comparison**
- **Provider websites:** Check the pricing pages of different companies.
- **Research papers and benchmarks:** Look for independent evaluations and comparisons of different models.
- **Community forums and discussions:** Engage with other users and experts to learn about their experiences and pricing insights.

## Maintenance

Building a generative AI solution is a journey, not a destination. To maximize your long-term success, it's essential to consider the ongoing maintenance and evolution of your project from the beginning.

- How will your project be maintained?
- Do you have the resources in place to maintain the project over time?
- What specific maintenance needs will your project have?

**Key maintenance considerations**

By proactively planning for maintenance, you'll ensure the long-term success and sustainability of your generative AI solution. Google Cloud provides a fully managed environment, which allows developers to focus on agent development rather than infrastructure and maintenance. With the platform handling deployment and model improvement, developers can maximize their return on investment and avoid costly issues down the road.
    
1. **Model monitoring and retraining**

Establish a system to continuously monitor your model's performance and retrain it periodically with updated data.

2. **Data updates**

Plan for regular data updates to keep your model fresh and relevant. This might involve adding new data sources, cleaning existing data, or adapting to evolving data formats.

3. **Software updates and bug fixes**

Stay informed about updates to your chosen AI platform, libraries, or frameworks, and implement them promptly to ensure optimal performance and security.

4. **Hardware and infrastructure**

Consider the maintenance needs of your hardware and infrastructure. This includes server maintenance, security updates, and capacity planning to accommodate growing data and user demands.

5. **Security and compliance**

Maintain a vigilant approach to security. Regularly review and update your security measures to protect against evolving threats. Ensure ongoing compliance with data privacy regulations as they change.

