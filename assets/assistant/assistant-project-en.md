# Project-Based Assistant
A project or product based assistant can be served as a consult of your product for your customers or users. You can add your own dataset to tain this assistant, such product mannuals, QAs, .etc.

## Create Project-Based Assistant

Creating a project-based assistant is quite straightforward, you should login in first, and the creation button(a plus icon with circle) will show on right up corner of top bar.

1.  Click the create button, and select project/application assistant

2.  Fill the information needed in basic step of creation wizard.
   + **Name**: type a name for this assistant, such as Kubernetes Assistant, Nginx Assistant, .etc.
   + **Description**: a description message of this assistant, will be displayed on assistant card. Markdown format is also supported, if you want to insert an image, use markdown format for image insertion.
   + **Avatar**: upload an avatar for this assistant if needed, click the editor button on right down corner of default avatar.

3.  **Project Detail**: Click next button, specify the details of your project or application
   + **Project Name**: The name of your project or application, such as Kubernetes
   + **Project Description**: specify the description of your project, such as: Kubernetes is an open-source container orchestration system for automating software deployment, scaling, and management. 

4.  **Advanced**: Click next button, fill up information needed in advanced step
   + **Visibility**: select private or public if you want to share this assistant.
   + **Email Notification** : when enabled, you will get an email notification by our system bot when some one is interacting with this assistant. The notification message in email body only contains user name who are talking to this assistant and nothing else. 
   + **Credits**: you can specify a credits number to charge users who want to chat with this assistant, if you have some credential formations that feded to it, or only fans scenario. The credits will be added to your account and you can request an payout when you want.
   + **Model**: select a LLM model in drop down list, for context aware, select chat model from openai or google, if you want to add your own dataset, only chat model from openai are supported, also, you can specified your own fine-tuned model from openai, in this mode, you should specify your own api key from openai to access this model. Note, if you select the 32k model of gpt4, you should specify your own api key in your setting page, for now, we havn't apply access for this model from openai.
   + **Category**: select a category for this assistant, for exploring and quick search.
5. Click Create button to submit.