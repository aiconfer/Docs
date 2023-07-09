# Custom Assistant
A custom assistant is defined by your own system prompt, if you are good at prompt engneering, you can create a custom assistant by you need. 

## Create Custom Assistant

Creating a custom assistant is quite straightforward, you should login in first, and the creation button(a plus icon with circle) will show on right up corner of top bar.

1.  Click the create button, and select custom

2.  Fill the information needed in basic step of creation wizard.
   + **Name**: type a name for this assistant, such as QR Generator, .etc.
   + **Description**: a description message of this assistant, will be displayed on assistant card. Markdown format is also supported, if you want to insert an image, use markdown format for image insertion.
   + **Gender**: select a gender, it will be used for voice output.
   + **Avatar**: upload an avatar for this assistant if needed, click the editor button on right down corner of default avatar.

3.  **System Prompt**: Click next button, specify the system prompt of this assistant
   + **prompt**: you can specify your own well-defined prompt or get one from [github.com/awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts), .etc.

4.  **Advanced**: Click next button, fill up information needed in advanced step
   + **Visibility**: select private or public if you want to share this assistant.
   + **Email Notification** : when enabled, you will get an email notification by our system bot when some one is interacting with this assistant. The notification message in email body only contains user name who are talking to this assistant and nothing else. 
   + **Credits**: you can specify a credits number to charge users who want to chat with this assistant, if you have some credential formations that feded to it, or only fans scenario. The credits will be added to your account and you can request an payout when you want.
   + **Model**: select a LLM model in drop down list, for context aware, select chat model from openai or google, if you want to add your own dataset, only chat model from openai are supported, also, you can specified your own fine-tuned model from openai, in this mode, you should specify your own api key from openai to access this model. Note, if you select the 32k model of gpt4, you should specify your own api key in your setting page, for now, we havn't apply access for this model from openai.
   + **Category**: select a category for this assistant, for exploring and quick search.
5. Click Create button to submit.
