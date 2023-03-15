
```
Currently, this plugin is only suported on versions of Unity 2022.x and above
```

# Installation

This plugin is provided as a custom Unity package that you can import into any existing project with the Unity version 2022.x and above.

Once you've downloaded the Unity package, you can them import it into your project which will subsequently add a new `NTY` navigation tab where the Unity ChatGPT window can be accessed, as seen below.

A video can be found [through this link](https://youtu.be/GJyrNXCUan8) showing the package import process (if you're having trouble).

---

# Setup

This plugin provides an in-engine interface to be able to use ChatGPT from within Unity.

The focus here is purely convenience in being able to access ChatGPT without leaving Unity. This helps to facilitate asking questions, exploring topics, generating ideas, and sometimes debugging issues.


### Step 1: Login to your OpenAI account and copy your secret key
To get started (once you have the plugin imported), you will first need to fetch your OpenAI API key, which can be found in your `User Settings` under `API Keys`. Here, you can create a new secret key and copy the value (you will use this secret key inside the Unity Editor).

![](/images/openai-api-key-location.png)

### Step 2: Add your OpenAI secret key to your Unity Project Settings
Back in Unity open `Project Settings`, navigate to `Unity ChatGPT` from the sidebar and then input your OpenAI secret key in the `API Key` field. Once this is done, you can safely close the `Project Settings` window.

![](/images/unity-chatgpt-project-settings.png)


### Step 3: Open the Unity ChatGPT Window and start using
In the navigation bar you will see an `NTY` menu option which will contain the `Unity ChatGPT` tool. Click this to open the Unity ChatGPT editor window and dock this window wherever you would like.

![](/images/unity-chatgpt-dockable-window.png)


# Usage
When you enter a prompt and send it, you will see a loading icon appear at the bottom right of the window while the API is busy consuming the request and returning the response.

When ChatGPT has completed a response, you will see it display in the output log above the prompt input.

```
Note that each time you send a prompt, a new chat request is sent to OpenAI. 
What you see in the output log is a history of responses to the prompts you
have sent. It is not a continuous conversation as you would experience in a
single chat session within the ChatGPT application.
```

![](/images/unity-chatgpt-output.png)

You can then write another prompt and send it, which will add the response of that prompt to the existing output log with each response being separated by a line of dashes. The history of responses will be maintined in the output log until you either (A) close Unity or (B) clear the output log. To clear the output log, you only need to click the `Clear Text` button.

Enjoy!
