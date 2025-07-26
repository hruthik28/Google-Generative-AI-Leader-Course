# Gen AI: Unlock Foundational Concepts

# Module 1:

## Understanding AI, ML, and generative AI

-Imagine you're teaching a child to paint. Traditional AI is like showing them a painting and saying, "This is a good painting. These are the characteristics of a good painting." The child learns to judge paintings based on those rules. Generative AI is like showing the child many different paintings and providing them with a set of brushes and colors, then asking them to create their own unique painting based on what they've learned.

## Differentiating AI, ML, and generative AI

- Artificial intelligence (AI): The broad field of building machines that can perform tasks requiring human intelligence.
- Machine learning (ML): A subset of AI where machines learn from data.
- Generative AI: An application of AI that creates new content.

## Understanding the importance of data in AI

- How do AI systems, powered by ML, actually accomplish these tasks? 
- It all boils down to the data they're fed.
- Essentially, machine learning models predict the future based on existing data, much like how humans use experience to make educated guesses.
- However, while humans might rely on intuition or gut feelings, these models use probability. 

- ML models analyze the data they've been given, identify patterns, and then calculate the likelihood of different outcomes when presented with new information.

## Data quality

- The quality and quantity of the data ML models learn from is absolutely crucial to how well they perform. There are five factors to focus on when thinking about data quality.

1. Accuracy
    - If the data is inaccurate, the model will learn incorrect patterns and make faulty predictions. Imagine teaching a child about animals using a book with mislabeled pictures—they'd learn the wrong things. The same applies to AI.
2. Completeness
    - Completeness refers to the size of a dataset as well as representation within the dataset. The size of the dataset is important because the model needs enough to make an accurate prediction. If a meteorologist tries to predict weather only based on the data of the past day, it will be a much worse prediction than if it used a much larger sample size.
3. Representative
    - Data needs to be representative and inclusive, otherwise it can lead to skewed samples and biased outcomes. If a dataset about customer preferences is missing information about a certain demographic, the model might make inaccurate or biased generalizations about that group.
4. Consistency
    Inconsistent data formats or labeling can confuse the model and hinder its ability to learn effectively. Imagine trying to assemble a puzzle where some pieces are labeled with numbers and others with letters—it would be a mess.
5. Relevance
    The data must be relevant to the task the AI is designed to perform. For example, data about traffic patterns in London is unlikely to be helpful for predicting crop yields in Kansas.

## Data accessibility

- The ability of AI systems to effectively utilize this data is directly tied to data accessibility. Data accessibility ensures that the necessary data is readily available, usable, and of high quality, allowing for comprehensive model training and reducing potential biases. Without accessible data, even the most sophisticated algorithms are limited in their ability to learn and provide accurate predictions.

1. Availability
    - If the necessary data simply isn't available, the AI model can't be trained. For some problems, the data might exist, but it might be locked behind paywalls or restricted due to privacy concerns.
2. Cost
    - Gathering and cleaning data can be expensive. The cost of acquiring high-quality data can be a significant barrier to AI development, especially for smaller organizations.
3. Format
    - Data needs to be in a format that the AI model can understand and process. Converting data into the appropriate format can be time-consuming and technically challenging.
    
## Data types

- Data is central to many business processes and various data types can be used in machine learning, but data isn’t just about numbers and files. Business datasets help organizations understand customers, optimize operations, and drive strategic decisions.
- Larger datasets frequently improve model performance, particularly for complex generative AI models that produce diverse content. However, a large dataset isn’t the only thing that matters because model performance is heavily dependent on the type of data used for training. This includes the data’s volume and its organization and structure. 
- Understanding your company’s data, its quality, availability, and form is essential for understanding the realm of what will be possible in terms of using that data for AI.

1. Data forms

    - Data comes in various forms, just like information itself. We can broadly categorize this data into two main types: structured and unstructured. Let’s explore this through a fictitious company that sells eco-friendly cleaning supplies called Cymbal Cleaning. 

    - The data they store for customer orders can include information like: 
        1. Customer ID 
        2. Customer name 
        3. Purchase date
        4. Order cost 
        5. Delivery address
        6. Product image
        7. Feedback (on a 1-5 star scale)

2. Structured data

    - Imagine your contact list on your phone. It has names, phone numbers, and maybe addresses, all organized in a list. That's structured data! It's easy to search and find the information you need.

    - This type of data is often stored in something called a relational database, which is like a super-organized digital filing cabinet with information neatly arranged in tables. Other examples of structured data include things like online shopping orders or bank statements.

    - For the cleaning supply company’s database, this would include:
        1. Customer ID
        2. Customer name
        3. Feedback (on a 1-5 star scale)
        4. Purchase date
        5. Order cost

3. Unstructured data

    - Unstructured data lacks a predefined structure. It is messy and complex by nature. It cannot be easily organized into rows and columns, so more sophisticated analysis techniques are required. Examples of unstructured data include things like text documents (PDFs, emails, social media posts), images (photographs, digital artwork, medical scans), audio (speech recordings, music files), and video (movies, YouTube videos, smartphone videos).

    - For the cleaning supply company’s database, this would include:
        1. Feedback (free-form text)
        2. Product image
        3. Email content

## Types of learning

## Machine learning approaches and data requirements

- The quality, accessibility, and form of data are fundamental, but how that data is used for ML depends on the specific learning method. Machine learning has three primary learning approaches: supervised, unsupervised, and reinforcement learning, each with its own data requirements. 
- Supervised models rely on labeled data, unsupervised models work with unlabeled data, and reinforcement learning learns through interaction and feedback.

## Labeled versus unlabeled data

1. Labeled Data 

    - Labeled data has tags, such as a name, type, or number. These tags, whether applied manually or by automated systems, assign meaning to the data. 
    - For instance, an image dataset for training a cat-detection model would label each picture as either a cat or dog. Similarly, a set of customer reviews might be labeled as positive, negative, or neutral. These labels enable algorithms to learn relationships and make accurate predictions.

2. Unlabeled Data

    - Unlabeled data is simply data that is not tagged or labeled in any way. It's raw, unprocessed information without inherent meaning. 
    - Examples of unlabeled data include a collection of unorganized photos, a stream of audio recordings, or website traffic logs without user categorization. In these cases, algorithms must independently discover patterns and structures within the data, as there are no pre-existing labels to guide the learning process.

## Supervised versus unsupervised learning

| Supervised                | Unsupervised |
|--------------------------------------------------------------|--------------------------------------------------------------|
|Supervised machine learning trains models on labeled data, where each input is paired with its correct output, allowing the model to learn the relationship between them. The model's goal is to identify patterns and relationships within this labeled data, enabling it to accurately predict outputs for new, unseen inputs.| Unsupervised ML models deal with raw, unlabeled data to find natural groupings. Instead of learning from labeled data, it dives headfirst into a sea of unlabeled data.|
|Predicting housing prices is a common example of supervised learning. A model is trained on a dataset where each house has labeled data, such as its size, number of bedrooms, location, and the corresponding sale price. This labeled data allows the algorithm to learn the relationship between the features of a house and its price. Once trained, the model can then predict the price of a new house based on its features.| For example, an unsupervised learning algorithm could analyze customer purchase history from your company's database. It might uncover hidden segments of customers with similar buying habits, even though you never explicitly labeled those segments beforehand. This can be incredibly valuable for targeted marketing or product recommendations. Think of it as exploratory analysis. Unsupervised learning helps you understand the underlying structure of your data and uncover insights that you might not have even known to look for.|

## Reinforcement learning

- Reinforcement learning is all about learning through interaction and feedback. Imagine a robot learning to navigate a maze. It starts with no knowledge of the maze's layout. As it explores and interacts with the maze, it collects data—bumping into walls (negative feedback) or finding shortcuts (positive feedback). Through this process of trial and error, the algorithm learns which actions lead to the best outcomes.

- It's like training a pet. You reward good behavior and discourage bad behavior. And over time, the pet learns to perform the desired actions. Similarly, in reinforcement learning, the algorithm learns to maximize rewards and minimize penalties by interacting with its environment.

- This type of learning is particularly useful in situations where you can't provide explicit instructions or labeled data. For example, you could use reinforcement learning to train a self-driving car to navigate complex traffic situations or to optimize the performance of a robot in a manufacturing plant.

## Examples of machine learning approaches on Google Cloud

1. Predictive maintenance with Vertex AI (supervised learning)
    - By training a model on sensor data from machines like temperature, pressure, and vibration, Vertex AI can predict when a machine is likely to fail, enabling proactive maintenance and reducing downtime.

2. Anomaly Detection with BigQuery ML (unsupervised learning)
    - BigQuery ML can analyze historical transaction data (amount, location, time, etc.) to identify patterns and flag unusual transactions that deviate significantly from the norm. This helps prevent fraud and minimize financial losses.

3. Product recommendations with Vertex AI (reinforcement learning)
    - Vertex AI can train a reinforcement learning model to recommend products to users based on their browsing history, purchase behavior, and other factors. The model learns to maximize user engagement and sales by continuously refining its recommendations.

# Turning data into learning using Google Cloud

## Data tools and management for ML workloads

- The key to building an ML model is data. But the journey from scattered data to actionable insights isn't always easy. There are a few key steps that it takes to get to having a working solution, and if you are building a solution for an enterprise, along the way you need to consider many factors such as security, robustness, and scalability. 

- Google Cloud offers a comprehensive suite of data tools and management capabilities tailored for ML workloads. These tools and capabilities are designed to support the entire ML lifecycle, from data preparation and model training to deployment and monitoring. 

## The key stages of making data accessible for AI.

1. Gather your data

    - Data gathering, also called data ingestion, involves collecting raw data from various sources. To effectively train and test your model, determine the data you need based on the outcome you want to achieve.

    - Google Cloud supports data ingestion through several tools. 

        1. Pub/Sub handles real-time streaming data processing, regardless of the structure of the data.
        2. Cloud Storage is well-suited for storing unstructured data.
        3. Cloud SQL and Cloud Spanner are used to manage structured data.

2. Prepare your data

    - Data preparation is the process of cleaning and transforming raw data into a usable format for analysis or model training. This involves formatting and labeling data properly. 

    - Google Cloud offers tools like BigQuery for data analysis and Data Catalog for data governance. These tools help prepare data for ML models. 

    - With BigQuery, you can filter data, correct its inconsistencies, and handle missing values. 

    - With Data Catalog, you can find relevant data for your ML projects. This tool provides a centralized repository to easily discover datasets in your organization.

3. Train your model

    - The process of creating your ML model using data is called model training. Google Cloud's Vertex AI platform provides a managed environment for training ML models. 

    - With Vertex AI, you can set parameters and build your model, using prebuilt containers for popular machine learning frameworks, custom training jobs, and tools for model evaluation. Vertex AI also provides access to powerful computing resources to make the model training process faster.

4. Deploy and predict

    - Model deployment is the process of making a trained model available for use. 

    - Vertex AI simplifies this by providing tools to put the model into action for generating predictions. This includes scaling the deployment, which means adjusting the resources allocated to the model to handle varying amounts of usage.

5. Manage your model

    - Model management is the process of managing and maintaining your models over time. Google Cloud offers tools for managing the entire lifecycle of ML models. This includes the following:

        1. Versioning: Keep track of different versions of the model.
        2. Performance tracking: Review the model metrics to check the model's performance.
        3. Drift monitoring: Watch for changes in the model's accuracy over time.
        4. Data management: Use Vertex AI Feature Store to manage the data features the model uses.
        5. Storage: Use Vertex AI Model Garden to store and organize the models in one place.
        6. Automate: Use Vertex AI Pipelines to automate your machine learning tasks.

## Google Cloud tools work together

- All these Google Cloud tools are designed to work together seamlessly. You can also connect them with your existing tools or build your own custom solutions. And throughout the entire process, Google Cloud's infrastructure ensures your solution is available and reliable. At the same time, Identity and Access Management (IAM) keeps your data safe and ensures only the right people have access.

# Module 2:

# Deep learning, generative AI, and foundation models

## Machine learning 
    
    - A broad field that encompasses many different techniques, one of which is deep learning (DL). 

## Deep learning 

    - A powerful subset of machine learning, distinguished by its use of artificial neural networks. These networks enable the processing of highly complex patterns and the generation of sophisticated predictions.

- Neural networks can leverage both labeled and unlabeled data, a strategy known as semi-supervised learning. They train on a blend of a small amount of labeled data and a large amount of unlabeled data. That way, they learn foundational concepts and generalize effectively to novel examples.

- Generative AI uses the power of deep learning to create new content spanning text, images, audio, and beyond. Deep learning techniques, particularly those centered on neural networks, are the engine behind these generative models.

## Foundation models

- Foundation models use deep learning. They are trained on massive datasets that allow them to learn complex patterns and perform a variety of tasks across different domains. They are incredibly powerful machine learning models trained on a massive scale, often using vast amounts of unlabeled data. This training allows them to develop a broad understanding of the world, capturing intricate patterns and relationships within the data they consume.

- Think of a foundation model as a highly advanced learner. It's like a student who has read everything in an entire library, absorbing knowledge from countless books, articles, and websites. This deep and extensive learning allows foundation models to be adapted to a wide range of tasks.

1. Large language models (LLMs)​​​

    - One particularly exciting type of foundation model is the LLM. These models are specifically designed to understand and generate human language. 

    - They can translate languages, write different kinds of creative content, and answer your questions in an informative way, even if they are open ended, challenging, or strange. This is likely the most common foundation model you've encountered, such as in popular generative AI chatbots like Gemini. They also help power many search engines you use today.

2. Diffusion models

    - Diffusion models are another type of foundational model. They excel in generating high-quality images, audio, and even video by iteratively refining noise (or unstructured/random data and patterns) into structured data.

## Choosing a model

- Factors when choosing a model for your use case

    1. Modality
        - When selecting a generative AI model, it's crucial to consider the modality of your input and output. Modality refers to the type of data the model can process and generate, such as text, images, video, or audio. If your application focuses on a single data type, like generating text-based articles or creating audio files, you'll want to choose a model optimized for that specific modality. For applications that require handling multiple data types, such as generating image captions (processing images and producing text) or creating video with accompanying audio, you'll need a multimodal model. These models can understand and synthesize information across different modalities.
    
    2. Context window
        - The context window refers to the amount of information a model can consider at one time when generating a response. A larger context window allows the model to "remember" more of the conversation or document, leading to more coherent and relevant outputs, especially for longer texts or complex tasks. However, larger context windows often come with increased computational costs. You need to balance the need for context with the practical limitations of your resources.
     
    3. Security
        - Security is paramount, especially when dealing with sensitive data. Consider the model's security features, including data encryption, access controls, and vulnerability management. Ensure the model complies with relevant security standards and regulations for your industry.
      
    4. Availability and reliability
        - The availability and reliability of the model are crucial for production applications. Choose a model that is consistently available and performs reliably under load. Consider factors like uptime guarantees, redundancy, and disaster recovery mechanisms.
    
    5. Cost
        - Generative AI models can vary significantly in cost. Consider the pricing model, which might be based on usage, compute time, or other factors. Evaluate the cost-effectiveness of the model in relation to your budget and the expected value of your application. This is where selecting the right model for the right task is important. Be sure to match the model to the task; bigger isn't always better, and multi-modal capabilities aren't always necessary.
    
    6. Performance
        - The performance of the model, including its accuracy, speed, and efficiency, is a critical factor. Evaluate the model's performance on relevant benchmarks and datasets. Consider the trade-offs between performance and cost.
    
    7. Fine-tuning and customization
        - Some models can be fine-tuned or customized for specific tasks or domains. If you have a specialized use case, consider models that offer fine-tuning capabilities. This often involves training the model further on a specific dataset related to your use case.
    
    8. Ease of integration
        - The ease of integrating the model into your existing systems and workflows is an important consideration. Look for models that offer well-documented APIs and SDKs.

## Google Cloud’s ML models

- Vertex AI streamlines the integration of advanced artificial intelligence capabilities into business applications, allowing for seamless discovery, deployment, and customization. These models empower businesses to leverage cutting-edge AI, providing the flexibility to work with many different models without the need for extensive in-house model development. 

- With Vertex AI you can access models developed by Google including Gemini, Gemma, Imagen, and Veo. You can also access proprietary third-party models, and openly available models.

1. Gemini

    - Gemini, a multimodal model, can understand and operate across diverse data formats, such as text, images, audio, and video. Gemini's multimodal design supports applications that require complex multimodal understanding, advanced conversational AI, content creation, and nuanced question answering.

2. Gemma

    - A family of lightweight, open models is built upon the research and technology behind Gemini. They offer developers a user-friendly and customizable solution for local deployments and specialized AI applications.

3. Imagen

    - A powerful text-to-image diffusion model, it excels at generating high-quality images from textual descriptions. This makes it invaluable for creative design, ecommerce visualization, and content creation.

4. Veo 

    - A model capable of generating video content. It can produce videos based on textual descriptions or still images. Its functionality allows for the creation of moving images for applications such as film production, advertising, and online content.

- Collectively, these Google Cloud foundation models empower businesses to enhance customer experiences through intelligent chatbots and personalized content. They increase productivity by automating tasks and improving information retrieval. They foster innovation by generating new ideas and designs. They also derive data-driven insights for improved decision-making.

## Google strategies for foundation model limitations

- Foundation model limitations

- Foundation models, while groundbreaking, aren't without limitations. Recognizing these limitations is essential for the responsible and effective utilization of these powerful tools.

1. Data dependency

    - The performance of foundation models is heavily data-dependent. They require large datasets, and any biases or incompleteness in that data will inevitably seep into their outputs. It's like asking a student to write an essay on a book they haven't read. If the data or questions are inaccurate or biased, the AI's performance will suffer.

2. Knowledge cutoff

    - Knowledge cutoff is the last date that an AI model was trained on new information. Models with older knowledge cutoffs may not know about recent events or discoveries. This can lead to incorrect or outdated answers, since AI models don't automatically update with the latest happenings around the world. 

    -For example, if an AI tool's last training date was in 2022, it wouldn't be able to provide information about events or information that happened after 2022.

3. Bias

    - An LLM learns from large amounts of data, which may contain biases. You can think of bias as an unbalanced dataset in LLMs. Due to their statistical learning nature, they can sometimes amplify existing biases present in the data. Even subtle biases in the training data can be magnified in the model's outputs.

4. Fairness

    - Even with perfectly balanced data, defining what constitutes fairness in an LLM's output is a complex task. Fairness can be interpreted in various ways. Fairness assessments for generative AI models, while valuable, have inherent limitations. These evaluations typically focus on specific categories of bias, potentially overlooking other forms of prejudice. Consequently, these benchmarks do not provide a complete picture of all potential risks associated with the models' outputs, highlighting the ongoing challenge of achieving truly equitable AI.

5. Hallucinations

    - Foundation models can sometimes experience hallucinations, which means they produce outputs that aren't accurate or based on real information. Because foundation models can't verify information against external sources, they may generate factually incorrect or nonsensical responses. These cause significant concern in accuracy-critical applications. The responses might sound convincing, but they are completely wrong. We will cover this in more detail below.

7. Edge cases

    - Rare and atypical scenarios can expose a model's weaknesses, leading to errors, misinterpretations, and unexpected results. 

## Techniques to overcome limitations

1. Grounding

    - Generative AI models are amazing at creating content, but sometimes they hallucinate. Grounding is the process of connecting the AI's output to verifiable sources of information—like giving AI a reality check. By providing the model with access to specific data sources, we tether its output to real-world information, reducing the risk of invented content. 

    - Grounding is essential for building trustworthy and reliable AI applications. By connecting your models to verifiable data, you ensure accuracy and build confidence. It offers several key benefits, including reducing hallucinations, which prevents the AI from generating false or fictional information. Grounding also anchors responses, ensuring the AI's answers are rooted in your provided data sources. Furthermore, it builds trust by enhancing the trustworthiness of the AI's output by providing citations and confidence scores, allowing you to verify the information.

2. Retrieval-augmented generation (RAG)

    - There are many different options on how you can ground in data. For example, you can ground in enterprise data or you can ground using Google Search. One common grounding method to do this is with retrieval-augmented generation, or RAG.

    - RAG is a grounding method that uses search to find relevant information from a knowledge base and provides that information to the LLM, giving it necessary context.

    - The first step is retrieval. When you ask an AI a question, RAG uses a search engine to find relevant information. This search engine uses an index that understands the semantic meaning of the text, not just keywords. This means it finds information based on meaning, ensuring higher relevance. 

    - The retrieved information is then added to the prompt given to the AI. This is the augmentation phase.

3. Prompt engineering

    - Prompting offers the most rapid and straightforward approach to supplying supplementary background information to models. This involves crafting precise prompts to guide the model towards desired outputs. It refines results by understanding the factors that influence a model's responses. However, prompting is limited by the model's existing knowledge; it can't conjure information it hasn't learned.

4. Fine-tuning

    - When prompt engineering doesn't deliver the desired outcomes, fine-tuning can enhance your model's performance. Pre-trained models are powerful, but they're designed for general purposes. Tuning helps them excel in specific areas. This process is particularly useful for specific tasks or when you need to enforce specific output formats, especially if you have examples of the desired output.

    - Tuning involves further training a pre-trained or foundation model on a new dataset specific to your task. This process adjusts the model's parameters, making it more specialized for your needs. Google Cloud Vertex AI provides tooling to facilitate tuning.

    - Here are some examples of how tuning can be used:

    - Fine-tuning a language model to generate creative content in a specific style.

    - Fine-tuning a code generation model to generate code in a particular programming language.

    - Fine-tuning a translation model to translate between specific languages or domains.

## Humans in the loop (HITL)

- Beyond these techniques, we must remember the invaluable role of humans in the loop (HITL). Machine learning models are powerful, but they sometimes need a human touch. For tasks requiring judgment, context, or handling incomplete data, human expertise is essential. HITL systems integrate human input and feedback directly into the ML process. This collaboration makes models more adaptable, especially in areas like the following.

    1. Content moderation
        - HITL ensures accurate and contextually appropriate moderation of user-generated content, filtering out harmful or inappropriate material that algorithms alone might miss.
    
    2. Sensitive applications
        - In fields like healthcare or finance, HITL provides oversight for critical decisions, ensuring accuracy and mitigating risks associated with automated systems.
    
    3. High-risk decision making
        - When ML models inform decisions with significant consequences, such as medical diagnoses or criminal justice assessments, HITL acts as a safeguard, providing a layer of human review and accountability.
    
    4. Pre-generation review
        - Before deploying ML-generated content or decisions, human experts can review and validate the outputs, catching potential errors or biases before they impact users.
    
    5. Post-generation review
        - After ML outputs are deployed, continuous human review and feedback help identify areas for improvement, enabling models to adapt to evolving contexts and user needs.

|Feature|RAG|Fine-tuning|Grounding|
|-------|-----|---------|---------|
|Definition|Augments LLMs by retrieving relevant information from external knowledge bases and adding it to the prompt.|Further trains a pre-trained model on a new dataset to adapt it to a specific task or domain.|Connects an AI model's output to verifiable sources of information.|
|Process|Retrieve relevant information. → Add it to the prompt. → Generate a response.|Select a pre-trained model. → Gather data. → Train the model. → Evaluate and refine.|Provide access to data sources. → Use RAG or fine-tuning to connect the output.|
|Data sources|External knowledge bases (databases, documents, internet).|Task- or domain-specific datasets.|External knowledge bases or specific datasets.|
|Relationship to grounding|A specific technique for achieving grounding.|Improves a model's ability to be grounded in specific domains.|The overarching goal, achieved through techniques like RAG and fine-tuning.|

# Module 3:

# Secure AI

- Secure AI is about preventing intentional harm being done to your applications. This is about protecting AI systems from malicious attacks and misuse. For all applications, including AI, you need to ensure security throughout the full lifecycle from development through deployment. This includes considering the data, infrastructure, and how and where applications are deployed.

## Machine Learning Lifecycle

1. Gather your data
    - The foundation of any robust AI system is secure data. Therefore, data must be protected and secured at all times. Access controls must be implemented to restrict who can access the data. They are also necessary to restrict who can add or input to the data. This is crucial to prevent data poisoning, a malicious attack where bad actors corrupt your AI model’s training data by introducing manipulated data. This can cause your model to learn incorrect patterns and make flawed (biased, inaccurate, or even harmful) predictions. It's akin to someone secretly swapping out vital ingredients in a recipe, leading to a disastrous final dish.

2. Prepare your data

    - During data preparation, special attention should be paid to confidential or sensitive data that might be present in the training data. Where feasible, anonymization techniques should be applied to this data, mitigating potential privacy risks. Data also should be rigorously validated, using integrity checks and anomaly detection to prevent poisoning. Data should be securely processed with encryption both at rest and in use. Logging and real-time monitoring should also be performed.

3. Train your model

    - Securing the model and the training process is paramount. This means safeguarding both the training data and model parameters from unauthorized access or modification. Model theft, where attackers steal proprietary or sensitive AI models, is a significant threat. Beyond gaining a competitive advantage, the stolen models could be used for malicious purposes, exploiting vulnerabilities or replicating sensitive functionality.

4. Deploy and predict

    - Once your model is trained and ready for action, it's crucial to safeguard it within its operating environment. This means controlling access to the model, determining who can interact with it and how. If you're using a pre-built model, it's essential to verify its source and check for any potential vulnerabilities.

5. Manage your model

    - Continuous monitoring and maintenance of the model's security are essential. Stay up to date on the latest security best practices in the field, specifically for your platform and model, and regularly update to patch vulnerabilities. Monitor model performance and outputs for anomalies or signs of tampering, and regularly review access permissions.

- Think of it like installing a high-tech security system in your office. You wouldn't give everyone the master key, right? Similarly, you need to restrict access to your model and filter the information it receives and sends out. 

- One major risk here is adversarial attacks, where attackers try to trick the model with misleading information. Imagine someone trying to bypass your security system with a fake ID—that's essentially what an adversarial attack does to your AI. Therefore, it's critical to have safeguards in place to filter, sanitize, and check the data coming into your model, ensuring it's not being fed misleading information. Likewise, you need to monitor the information your model sends out. Think of it as screening outgoing messages to prevent any accidental leaks of sensitive data or the spread of harmful content.

- Stay informed
    - Keeping AI applications secure demands constant vigilance and staying informed about the latest security threats and research.

- Applying the Secure AI Framework (SAIF)​
    - Google has developed the Secure AI Framework, or SAIF, to establish security standards for building and deploying AI systems responsibly. This comprehensive approach to AI/ML model risk management addresses the key concerns of security professionals in the rapidly evolving landscape of AI. Following the security practices outlined in SAIF can help your organization find and stop threats, automatically strengthen its defenses, and manage the unique risks of each AI system. The framework is designed to integrate with your company’s existing security, ensuring that AI models are secure by default. For more information, explore Google's Secure AI Framework (SAIF).


- Google Cloud security tools​
    - Platforms such as Google Cloud can facilitate secure development. In addition to the Secure AI Framework, Google Cloud offers a range of tools to ensure applications remain secure throughout their lifecycle. Google Cloud has built security into its core through a secure-by-design infrastructure, encompassing its global network and hardware, as well as robust encryption in transit and at rest. It provides customers with detailed control over access and usage of cloud resources through Identity and Access Management (IAM). Google Cloud Security Command Center provides a centralized view of your security posture across your entire Google Cloud environment, and Google Cloud also offers tools for monitoring various workloads.

## Responsible AI

- Responsible AI means ensuring your AI applications avoid intentional and unintentional harm. It’s important to consider ethical development and positive outcomes for the software you develop. The same holds true, and perhaps even more so, for AI applications.

## Building on security

- The foundation of responsible AI is security. Secure applications protect both your company and your users. Think of it like building a house: if the foundation is weak, the entire structure is compromised, no matter how beautiful the design. Just as a strong foundation ensures a stable and safe house, robust security forms the essential foundation for building truly responsible AI.

1. Transparency is key
    - Transparency is paramount for responsible applications. Users need to understand how their information is being used and how the AI system works. This transparency should extend to all aspects of the AI's operation, including data handling, decision-making processes, and potential biases.

2. Privacy in the age of AI
    - Protecting privacy often involves anonymizing or pseudonymizing data, ensuring individuals can't be easily identified. AI models can sometimes inadvertently leak sensitive information from their training data, so it's crucial to implement safeguards to prevent this.

3. Data quality, bias, and fairness
    - Ethical AI requires high quality data
        - Machine learning and generative AI applications are fundamentally based on data. Therefore, responsible AI requires high-quality data. Inaccurate or incomplete data can lead to biased outcomes. Remember, technology often reflects existing societal biases. Without careful consideration, AI can amplify these biases, leading to unfair and discriminatory results. Beyond data quality, it's crucial to consider the responsible use of the data itself. Was it collected consensually? Could it perpetuate harmful biases?
    - Understanding and mitigating bias​
        - AI systems are not independent of the world they are built in. They can inherit and amplify existing societal biases. This can lead to unfair outcomes, such as a resume-screening tool that favors a certain demographic of candidates due to historical biases in hiring data. It's like training a dog with biased commands; the dog will learn and replicate those biases. To counter this, fairness must be a core principle in AI development.

4. Accountability and explainability
    - Fairness requires accountability​
        - Fairness requires accountability. We need to know who is responsible for the AI's actions and understand how it makes decisions. This is where explainability comes in. Explainable AI makes the decision-making processes of AI models transparent and understandable. This is crucial for building trust, debugging errors, and uncovering hidden biases. Think of it like a judge explaining their verdict; without a clear explanation, it's hard to trust the decision. Tools like Google Cloud’s Vertex Explainable AI can help understand model outputs and identify potential biases. Understanding how your application uses and interprets the AI's output is crucial for ensuring responsible use.

## Legal implications

- Beyond considerations like fairness and bias, AI development is increasingly governed by legal frameworks. Key areas include data privacy, non-discrimination, intellectual property, and product liability. 

    1. Laws mandate responsible data handling, bias mitigation, and transparency in algorithmic decision-making.

    2. Organizations must also adhere to the specific rules and limitations of the AI models they employ, ensuring compliance with licensing agreements and legal standards.

    3. The legal landscape is rapidly evolving, requiring organizations to stay informed and seek legal counsel to ensure compliance.

    4. Legal compliance is not just a regulatory hurdle. Navigating these legal implications is crucial for building trustworthy AI.
