# Module 1:

## Gemini for Google Workspace

- Gemini for Google Workspace
Google Workspace is a collection of cloud-based productivity and collaboration tools that help people create, communicate, and collaborate, such as Gmail, Google Docs, Google Sheets, Google Meet, and Google Slides.

- Gemini is a gen AI model that is then used in many other applications. Some of those applications were built in Google Workspace. You can access Gemini directly within your Workspace apps through Gemini for Workspace.

1. **Gemini for Google Workspace** allows you to use Google's generative AI capabilities. Depending on your version of Google Workspace, you may have access to a different range of features and security protections. For more information, see the Help Center article, [Gemini for Google Workspace.](https://support.google.com/a/answer/13623623)

2. **Google Workspace business and enterprise** licenses come with extra enterprise-grade data protection for your organization. These protections extend to the Gemini for Google Workspace features and the Gemini app (with Gemini Advanced). The licenses also come with administrative features for managing your organization's usage and access.

3. **Gemini side panel**

One way to access Gemini for Workspace is through the Gemini side panel, which is present on the side of many Workspace apps. With the side panel, Gemini can assist you with summarizing, analyzing, and generating content by utilizing insights gathered from your emails, documents, and more—all without switching applications or tabs. 

For example, new employees can use the Gemini in Drive side panel to get up to speed on projects and company initiatives. They can ask Gemini questions like "summarize the goals and current status of Project Phoenix" and easily find the information they need, enabling them to quickly become familiar with the project.

4. **Gemini in Gmail**

Gemini in Gmail uses generative AI to help users write and refine emails more efficiently. 

An HR representative can use Gemini to write a company-wide email announcing a new employee benefit. They can provide a prompt that includes information about the new benefit, who is eligible, and the effective date, and Gemini will generate a draft email.

5. **Gemini in Google Docs**

Gemini in Google Docs helps you streamline the process of content creation, refining, and proofreading right within your document as you write. 

A marketing team member can utilize Gemini to generate captivating taglines and draft social media posts for a new athletic shoe campaign. The user can provide a prompt like "Generate three social media posts that highlight the benefits of our athletic shoes, focusing on comfort and performance." Gemini then generates text options for the posts.

6. **Gemini in Google Slides**

Gemini in Google Slides can help you and your team work more effectively by using AI to generate photorealistic images that enhance your presentations. 

By providing Gemini with a descriptive prompt that outlines the subject, setting, or style you desire, you can quickly create images that otherwise would require time and effort to source or design. This streamlines the presentation creation process and frees up your team to focus on content and delivery.

7. **Gemini in Google Sheets**

Gemini in Google Sheets helps you generate formulas using AI. 

You can provide Gemini with prompts using plain language or generic cell names to create complex formulas. For example, you can ask Gemini to "create a formula to find cell C1 in range D:G and output the value in column G." Gemini then creates the formula.

8. **Gemini in Google Meet**

Gemini in Google Meet can help your global team communicate by providing real-time transcription and translation, facilitating seamless communication in multilingual meetings. It could also automate meeting summaries and action item extraction, saving time and increasing productivity for participants.

- These Gemini for Workspace features allow you to use AI-enhanced workflows in your daily work to become more productive and effective.

## Taking enterprise Workspace farther

Gemini's capabilities also extend to other powerful applications within the Google Workspace ecosystem, like Google Vids and AppSheet.

1. **Google Vids** is an online video creation and editing app available to Google Workspace users through your organization. 

With Help me Create in Vids, you can use Gemini to generate a first draft of your video. As a project manager, you can use Vids to share project updates, timelines, and key insights with your stakeholders to more effectively communicate information than an email or lengthy report can. 

2. **AppSheet** is a no-code app development tool included with Google Workspace enterprise editions. With Gemini in AppSheet, you can quickly create apps using AI by describing your needs in a prompt using natural language.

Gemini can create an app structure with tables, columns, and links based on your description, such as "Manage inspections of my facility." You can then review and edit the app structure before creating the app in the AppSheet app editor.

## Use case: Understood.org

- Adding Gemini for Workspace functionality into your daily workflow can greatly enhance your productivity. Let’s take a look at an example from a company, Understood.org, to bring this to life. 

- Understood.org is a social impact organization that supports people with learning and thinking differences such as ADHD and dyslexia, a critical issue, as it impacts more than 70 million Americans. 

- They leveraged Gemini for Google Workspace and the Gemini app to surface trends, build donor profiles, and tailor its communications. Using natural language, researchers at the nonprofit used Gemini's outputs to tailor their donation outreach. Using Gemini for Workspace has resulted in significant benefits including 10 hours saved per research project and more.

## Prompting techniques

## **Using examples in your prompts**

When it comes to prompting techniques, there are a few different approaches. 
- **Zero-shot prompting** is like asking a foundation model to complete a task with no prior examples, relying solely on its existing knowledge. 

    Example: A customer asks about your return policy. The LLM, drawing on its vast knowledge base, understands the question and provides a response, even though it hasn't received specific training on your company's policies.

- **One-shot prompting** involves showing the foundation model just one example, allowing it to learn and apply that knowledge to similar situations. 

    Example: You prompt with a single example of a customer inquiry, such as a question about shipping times. The output follows this example and accurately tags similar customer questions.

- **Few-shot prompting**, on the other hand, provides the foundation model with multiple examples to learn from, which helps it better understand the task and improve its performance.

    Example:You prompt with a few examples of customer inquiries and effective responses. The output follows these examples and accurately tags similar customer questions. For example, the output might include a discount code when a customer reports a delayed delivery, or provide detailed instructions on how to return a damaged item.

## Role prompting

Role prompting is a technique used to guide the behavior of LLMs by assigning them a specific role or persona. This can be anything from a business analyst or Shakespearean actor to a helpful customer service agent. By instructing the model to adopt a particular role, you influence the style, tone, and focus of its responses.

**Prompt 1**

You are a customer service agent for a telecommunications company with ten years of experience. A customer is inquiring about their latest bill, which is higher than expected.

**LLM output**

The LLM can adopt a helpful and patient tone, explaining potential reasons for the higher bill, offering solutions, and providing information about the company's policies in a clear and concise manner.


**Prompt 2**

You are a marketing copywriter for a new line of athletic wear. Write a product description for a pair of running shoes emphasizing their comfort and performance-enhancing features.

**LLM output**

With a prompt like this, the LLM may generate persuasive and engaging copy highlighting the key benefits of the shoes, using language that appeals to your target audience. It might even craft compelling narratives or tap into emotions that resonate with the target audience, making the product more memorable.

## Prompt chaining
When working in a tool like Gemini, it's important to understand how previous prompts may impact future prompts.

Prompt chaining is a powerful technique for getting more complex and nuanced results from large language models like Gemini. It's like having a conversation with the AI where each response builds upon the previous one, leading to a more sophisticated and refined outcome. 

This is where the concept of a chatbot comes in. You can have a back and forth with Gemini.

# Module 2:

## Reuse prompts with Gemini and Gems

**Sample prompt examples**

1. Marketing manager

    "Write a catchy social media post for [platform] promoting our new [product/service]. Highlight [key features/benefits] and include a call to action to [desired action]."

2. Content writer

    "Write a [content type: blog post, article, script] about [topic]. The target audience is [audience description]. The tone should be [tone: informative, humorous, persuasive]. Include [keywords]."

3. Customer support

    "Respond to this customer email: [paste email content]. Be empathetic and address their concerns about [issue]. Offer a solution that aligns with our [company policy]."

4. Software developer

    Write Python code to [Task]. Use [Libraries/Frameworks] and follow [Coding style guidelines]."

## Prompt chaining
Remember prompt chaining? It lets you continue your conversation in the same chatbot so the chatbot knows your history before continuing on with the new prompt. Well, if you don’t want to keep repeating the same history, you can use the same conversation thread and keep working there. In Gemini, you can even name your chats and pin them for easy access.

**Prompt chaining scenario**

Imagine you're a marketing manager using Gemini to develop a campaign for a new line of organic skincare products. Let’s see prompt chaining in action with two sets of prompts and responses. Note how Gemini remembers the context from the previous prompts.

## Gemini Advanced
**Gemini Advanced** is an upgraded version of Gemini with extra features, making it far more capable at highly complex tasks, like coding, logical reasoning, following nuanced instructions, and creative collaboration. You can adjust your data retention settings to determine how long information is stored and delete your conversation history at any time. For more detailed information, see the help center article, Upgrade to Gemini Advanced.

**Saved info**

Using the same prompts in a chain won’t always work because, sometimes, you just want the gen AI tool to remember the context but not everything in your whole conversation history. For example, maybe you're a sales rep preparing for calls with potential clients. You might want to practice different sales pitches but wouldn't want the AI's feedback to be influenced by your previous practice sessions or specific details about past clients. In these cases, you can actually save information in Gemini that it will always use. 

This is done through your **Settings** in your **Saved info**. You can let Gemini know that you're a sales rep so you do not need to constantly reiterate this in every prompt conversation.

Or let’s say a sales team leader wants to use Gemini to generate weekly sales reports. They can save their team's sales targets, key performance indicators (KPIs), and preferred reporting format in the Saved info. This ensures that Gemini always uses the correct information when generating reports, without the need to re-enter it each time.

**Gems**

But even saved information won’t always work. Because that will apply to all your Gemini chats. Sometimes you need specific context for particular tasks or conversations. This is where Gems come in.

Like agents, these AI assistants can process information and reason over complex ideas within the context of your chosen task. You can have Gems dedicated to:

- **Creative writing:** This Gem could be pre-loaded with your preferred writing style, tone, and commonly used resources. It could even help you brainstorm ideas, generate different creative text formats (poems, scripts, articles), and provide feedback on your drafts.

**Coding:** A coding Gem could be equipped with your favorite libraries, coding conventions, and even access to relevant documentation. It could assist with debugging, suggest code optimizations, and even generate code snippets based on your instructions.

**Marketing:** This Gem could be pre-loaded with your target audience demographics, competitor information, and campaign performance data. It could help you brainstorm campaign ideas, generate different marketing copy (social media posts, email newsletters, website content), analyze campaign performance, and suggest optimizations.

Think of Gems as your personalized AI assistants within Gemini.

## How do Gems work?

**Personalized responses**

Gems can be tailored with specific instructions and information. This allows them to provide responses that are more relevant to your needs and preferences within that particular use case.

**Streamlined workflows**

Gems can help you streamline repetitive tasks by providing templates, prompts, or guided interactions. This can save you time and effort when working on familiar projects or activities.

**Reset context**

You can set the context for a Gem, like giving it background information or specific instructions. Then, you can start multiple chats with that Gem, each with its own focus and flow. These chats remain separate, so information from one won't spill over into another. It's like having different conversations with the same expert, each tailored to a specific purpose.

You can choose to use Google’s existing Gems that were built for many different common tasks, or you can create your own gem tailored to your use case.

## What information can you provide to a custom Gem?
When you create a custom Gem, you provide it with instructions on how to act, what to do, and more. You are essentially prompting the agent or Gem on how to act. It's time to take all that prompting practice to the next level: Prompting to build your agents.

This is a very good place to use role-prompting, where you prompt the Gem to act as though it is in a specific type of role, such as an air traffic controller. 

You can also provide specific documents and resources to a Gem, giving it a focused knowledge base to draw from. Imagine a "code reviewer" Gem that has access to your project's coding style guidelines and best practices documentation. This would allow the Gem to provide feedback grounded in your specific project requirements.

Regardless of your use case, when creating Gems, it's important to be as clear and specific as possible in your instructions. You can also provide examples to illustrate your desired outcomes. Either way, be prepared to refine your instructions over time as you use the Gem and identify areas for improvement. 

## Grounding
Grounding refers to the ability of the AI model to connect its output to verifiable and specific sources of information. 
This is a critical aspect of building trust and reliability in AI systems. This is something you can already do in a Gem or Gemini prompt with no coding at all to improve accuracy and relevance to the task you need your agent to solve.

For example, you can create a Gemini prompt that helps you refine your writing by editing your text to meet your organization’s specific guidelines and standards. You can provide Gemini with resources, such as your company’s style guides within the prompt itself, or by uploading relevant files.

By grounding with this additional information, you provide the AI model with a richer context. This can lead to more accurate and insightful results.

## Rag: Retrieval-augmented generation
One powerful grounding technique is retrieval-augmented generation (RAG). It involves:

1. **Retrieving relevant information:** The AI model first retrieves relevant information from a vast knowledge base (like a database, a set of documents, or even the entire web). This retrieval process is often powered by sophisticated techniques, like semantic search or vector databases.

2. **Generating output:** The model then uses this retrieved information to generate the final output. This could be anything from answering a question to writing a creative story.


**Model only (without RAG)**

The user inputs a prompt.

The model provides output without external knowledge. The output might be outdated, and is more likely to have hallucinations.

**Model with RAG**

The user inputs a prompt.

A query is sent to a backend retrieval system such as a vector database or search engine to find the most relevant information, and embed it as a part of the prompt. 

The model provides the output with the latest external knowledge. The output is much less likely to have hallucinations.

## NotebookLM
NotebookLM is an AI-first notebook, grounded in your own documents, designed to help you gain insights faster. 

It’s a unique tool that is built using Gemini models and is designed to help you learn and understand information better by acting as a virtual research assistant. You can "ground" NotebookLM in specific sources like documents, presentations, or even audio and video files. This means your AI assistant will only use information from those sources to answer your questions and generate summaries.

NotebookLM is your personalized AI research partner who has read the provided source material and can answer any question about it.

It can even create different types of summaries, like bullet points, Q&A formats, or even a creative story!

## NotebookLM Plus

For users who want to take their research to the next level, there's NotebookLM Plus, a subscription plan that offers benefits like increased capacity, customization of response length and style, and usage analytics. 

## NotebookLM Enterprise

NotebookLM Enterprise takes NotebookLM Plus to the next level by adding compliance and administrative features necessary for enterprise environments. This includes extra privacy and security features to give you enhanced control over your data. Your notebook information is only shared with your chosen collaborators, and you can manage access using predefined identity and access management (IAM) roles. To learn more, see the documentation for [What is NotebookLM Enterprise?](https://cloud.google.com/agentspace/notebooklm-enterprise/docs/overview).

## Here's how it works
NotebookLM operates on the concept of "notebooks" to help you organize and interact with your information. Here's a breakdown:

1. **Creating a notebook**

    - Think of a notebook as a container for a specific project, topic, or area of interest.

    - You start by giving your notebook a title and then uploading the relevant source materials (documents, PDFs, even audio or video files) that you want it to learn from.

2. **The chat interface**

    - Within each notebook, you have a single, ongoing chat with the NotebookLM AI.

    - You can ask questions, request summaries, or give instructions, just like you would in a regular chat.

    - NotebookLM will respond using only the information from the sources you've uploaded to that specific notebook.

3. **Saving insights as notes**

    - When the AI provides a response you find valuable, you can save it as a note within the notebook.

    - These notes become an organized collection of key takeaways, summaries, or important points.

4. **Sharing and collaboration**
    
    - You can create "shared notebooks" to collaborate with others.

    - In a shared notebook, everyone can access the same sources, ask questions, and contribute to the notes.

    - This fosters collaborative learning and knowledge sharing.

Imagine you're writing a research paper. You can upload all your relevant documents to NotebookLM and ask it to:

- Summarize key findings from each source.
- Identify connections and contradictions between different perspectives.
- Generate outlines and drafts for your paper.
- Answer specific questions about the topic.

NotebookLM essentially becomes your personal research assistant, helping you navigate complex information and gain deeper insights. It's a powerful tool for students, researchers, and anyone who wants to learn more effectively.

## ​How is NotebookLM different from Gemini and Gems?​
While Gems excel at general tasks and workflows, NotebookLM is designed to help you deeply understand and learn from specific sets of information. It's like having a dedicated expert who has thoroughly analyzed your chosen materials and is ready to answer any question you have.

## NotebookLM versus Gems
- **Hyper-focused knowledge:** Instead of drawing from a broad knowledge base, NotebookLM focuses solely on the sources you provide. This could be anything from research papers and articles to meeting notes and presentations.
- **Interactive learning:** NotebookLM goes beyond simply summarizing information. It encourages active learning by allowing you to ask questions, generate different types of summaries, and even create quizzes to test your understanding.
- **Source-based answers:** Every answer and insight provided by NotebookLM is directly grounded in your uploaded sources. This ensures accuracy and allows you to easily trace back to the original information. If you ask NotebookLM a question that isn't covered in the materials you've provided, it will honestly tell you that it can't answer. It won't invent information or speculate. This ensures that the information you get is always grounded in your sources and reliable.

## Use cases

1. **Create training materials and documentation**

    Onboard new team members and facilitate knowledge transfer by creating a central repository for essential resources. Create a dedicated notebook to share with new hires with relevant onboarding materials (employee handbook, product documentation, training presentations). The new employees can then use NotebookLM to ask questions, clarify information, and gain a deeper understanding of their role and the company.

2. **Researching a new topic**

    Gather articles and videos on a subject you're interested in and have NotebookLM create a comprehensive summary or answer specific questions you have.

3. **Learn by listening to audio**

    With audio overviews in NotebookLM you can learn about the material covered in your sources through a podcast-like experience. NotebookLM will  summarize your material, connecting topics, and produce a downloadable audio with back-and-forth conversation between two AI hosts.

4. **Preparing for a presentation**

    Feed NotebookLM your presentation slides and ask it to generate speaker notes or practice questions to help you rehearse.

5. **Summarize documentation**

    Investment firms and legal teams need to thoroughly analyze documents and data. Upload financial statements, legal documents, and market research reports into NotebookLM. The team can then use the AI to quickly identify key information, summarize findings, and flag potential risks or inconsistencies.

6. **Project proposals and plans**

    Keep everyone aligned and informed by creating a shared NotebookLM with all project-related information.

## NotebookLM in action

A venture capital firm specializing in early-stage technology companies needs to make informed decisions about where to allocate capital. They have a mountain of data at their disposal:

- Market research reports on emerging technologies and industry trends.
- Financial statements from numerous startups seeking funding.
- Economic forecasts and analyses impacting the tech sector.
- Competitor portfolio assessments and funding strategies.

But sifting through all this information to pinpoint the most promising startups and identify potential risks is a daunting task. The team risks getting lost in the data, wasting valuable time and potentially missing crucial insights. Furthermore, these documents might be scattered across different departments and platforms, hindering collaboration and creating information silos.

This is where NotebookLM becomes invaluable. The team uploads all their relevant documents into a shared NotebookLM workspace. This shared workspace is key because it allows everyone on the team to access and analyze the same information, fostering a single source of truth and breaking down those information silos. Now, they can:

- Ask targeted questions: "What are the projected growth rates for the AI-powered healthcare sector?" or "What are the key risk factors associated with investing in this particular startup?"
- Analyze specific aspects: "Summarize the financial performance of startup X over the past year, focusing on user acquisition costs."
- Uncover hidden connections: "Identify any correlations between early adoption rates and long-term success in this market segment."

NotebookLM analyzes the uploaded documents and provides concise, insightful answers grounded in the data. It can even generate different types of summaries, highlighting key trends and potential investment opportunities.

The result? The venture capital team quickly identifies a promising new investment opportunity in a startup developing cutting-edge AI-driven medical diagnostics. The firm achieves significant gains and strengthens its reputation for making data-driven investment decisions. More importantly, they've experienced the power of collaborative analysis and knowledge sharing, leading to faster decision-making and better investment outcomes.

What critical business challenges are you facing? How can NotebookLM help you unlock the knowledge hidden within your data? Explore the possibilities and transform your workflows with the power of AI-driven research.


By centralizing these resources in a shared NotebookLM, your team can:

- Ask questions and gain a deeper understanding of the material together.
- Generate collaborative summaries and reports that leverage everyone's insights.
- Identify connections and contradictions between different perspectives more easily.
- Stay up-to-date with the latest information and changes.

Shared NotebookLM notebooks foster a culture of collaborative learning and knowledge sharing, empowering your team to work smarter and more effectively. It's like having a collective "brain" that everyone can contribute to and benefit from.

# Module 3:

## Gemini for Google Cloud 
Just like with Google Workspace, Gemini is revolutionizing how we interact with Google Cloud. From simplifying data analysis to boosting developer productivity, Gemini for Google Cloud offers a suite of AI-powered tools designed to enhance your cloud experience.

## Always on enterprise security with Gemini for Google Cloud
Gemini for Google Cloud does not use your prompts or Gemini’s responses to train models. It comes with the standard Google Cloud enterprise protections.

**Gemini Cloud Assist**

Gemini Cloud Assist is like having an AI expert on your team who helps you design, manage, and optimize applications on Google Cloud. It provides personalized guidance and is integrated with your Google Cloud environment to provide application lifecycle management assistance. It analyzes your cloud environment, your resources deployed, as well as metrics and logs to deliver actionable insights tailored to your needs.

**Gemini in BigQuery**

Gemini in BigQuery makes data analysis easier and more accessible. It can help you write code, understand your data, and even generate insights automatically, regardless of your SQL experience. This means faster and more efficient data exploration.

**Gemini Code Assist**

Gemini Code Assist acts as an AI pair programmer, helping developers write better code, just like when two programmers work together to solve problems. Gemini Code Assist can provide code suggestions, generate code blocks, and even offer explanations. It supports over 20 popular programming languages, code editors, and developer platforms, all of which help developers increase productivity.  

**Gemini in Colab Enterprise**

A Colab Enterprise notebook is an interactive environment that lets you write and execute code. Gemini in Colab Enterprise can use AI to help you write Python code in your notebook by suggesting code segments as you type and generating code based on your descriptions. This streamlines your data analysis and machine learning workflows.

**Gemini in Databases**

Gemini in Databases helps developers and database administrators manage their databases more effectively. It uses AI to simplify many aspects of using a database, from building applications with natural language to managing an entire fleet of databases from a single interface.

**Gemini in Looker**

With Gemini in Looker, you can analyze data and gain insights faster. As an intelligent assistant, it helps you understand your data, create visualizations, and even generate reports, making data exploration more intuitive.

**Gemini in Security**

Gemini in Security helps security teams detect, contain, and stop threats from spreading. It provides near-instant analysis of security findings and potential attack paths. Gemini in Security also summarizes prevalent tactics, techniques, and procedures used by threat actors, giving customers around the world detailed and timely threat intelligence.

These applications demonstrate how gen AI, specifically the Gemini model, can be integrated into various tools. For more information on Google Cloud's enterprise protections, review the article "[Creating trust through transparency](https://cloud.google.com/transparency#:~:text=When%20you%20use%20Google%20Workspace,customer%20data%20to%20third%20parties)."


## Use case: Gemini in action

Consider Cymbal Retail, a growing retail chain with a wealth of data stored in BigQuery. Their marketing team wants to analyze customer demographics, purchasing patterns, and campaign performance to refine their strategies. However, they rely heavily on the data analytics team to extract and interpret the data, creating a bottleneck and delaying crucial insights.

Cymbal Retail turned to Gemini in BigQuery with function calling to empower their marketing team. By building a user-friendly app, they enabled their marketers to explore the BigQuery database using natural language. Now, instead of writing complex SQL queries, they can simply ask questions like: 

"What are the top-selling products in the Northeast region?" "Show me the customer demographics for our latest marketing campaign." "How did our holiday promotions perform compared to last year?"

Gemini in BigQuery translates these natural language queries into SQL, retrieves the relevant data, and presents it in an easily understandable format.

The results were transformative for Cymbal Retail.

- **Increased agility:** The marketing team gained direct access to data, enabling faster decision-making and campaign adjustments.

- **Improved collaboration:** Data analysts were freed from routine data extraction tasks, allowing them to focus on more strategic initiatives.

- **Enhanced data literacy:** Business users gained a deeper understanding of their data, leading to more data-driven insights and innovation.

Imagine the possibilities for your organization. 

Cymbal Retail turned to Gemini in BigQuery with function calling to empower their marketing team by building a user-friendly app and enabled their marketers to explore the BigQuery database using natural language. 


What is a key benefit of Gemini in BigQuery?

    It makes data analysis easier and more accessible, regardless of your SQL experience.

How does Gemini Code Assist improve developer productivity?

    It acts as an AI pair programmer, offering code suggestions, generating code blocks, and providing explanations.

What is unique about how Gemini for Google Cloud handles user data?

    Google doesn't use your prompts or Gemini's responses to train models, ensuring your data remains private.