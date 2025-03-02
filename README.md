# DeepSeek-Unity
> Currently, this plugin is only suported on versions of Unity 2022.x and above

# Installation

This plugin is provided as a custom Unity package that you can import into any existing project with the Unity version 2022.x and above.

Once you've downloaded the Unity package, you can import the `Example` scene inside the `DeepSeek` folder. 

---

# Setup

DeepSeek provides an alternative to ChatGPT for Unity developers. Here's a quick guide to setting up DeepSeek:

- Setup Guide: [Watch the YouTube tutorial](https://www.youtube.com/watch?v=Z6MFqIzOHK0&ab_channel=UnityGameStudio)


### Step 1: Login to your DeepSeek account and copy your secret key
To get started you will first need to fetch your DeepSeek API key, which can be found the DeepSeek Platform under `Get API Key` (or through [this direct link](https://platform.deepseek.com/api_keys)). Here, you can create a new secret key and copy the value (you will need to your secret key for the next step).

![](/Images/ScreenShot4.JPG)

### Step 2: Open the Unity Editor, configure the package, and start using DeepSeek
Inside the package, you will find an `Example` Scene. Inside this scene, there is a game object with a `UnityAndDeepSeek.cs` script attach to it. Add your API Secret Key inside the `API Key` field. And, you can start using DeepSeek.

![](/Images/Chatbot.JPG)

![](/Images/ScreenShot8.JPG)


# Functions

This plugin provides one main function. 

ChatWithDeepSeek Function: 

The script contains an IEnumerator function that appends a List of chats, and sends it to the DeepSeek API and prints the response to the console by calling Debug.Log().

Unity connects with [DeepSeek API](https://api.deepseek.com/chat/completions). 

`IEnumerator SendDeepSeekRequest()`


# Usage
The unity package was made to directly use the function with a User Interface. Therefore, the best way to interact with it, it is through the `Example` Scene. After hitting on play, the `Example` Scene grabs the text you put inside the Input field, and sends it to the DeepSeek API when hitting the button "Send Message". 

> Note that DeepSeek is a paid API, I recommend using [Gemini](https://github.com/UnityGameStudio/Gemini-Unity-Package) instead, which is free upon certain amount of requests.
