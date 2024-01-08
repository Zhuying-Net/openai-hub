<p align="center">
  <img src="/img/logo.webp" width="120" height="120" alt="OpenAI-Hub"/>
  <h1 align="center">OpenAI-Hub</h1>
</p>
<p align="center"><a>Simplified Chinese</a> | <a href="/README.en.md">English</a></p>

<p style="font-size:18px" align="center">Access OpenAI APIs Directly, Globally Accelerated, and at Minimal Cost</p>


> [✨Official Website](https://www.openai-hub.com) | 
> [🔥API Documentation](https://www.openai-hub.com/api/) | 
> [🌟Open Platform](https://api.openai-hub.com)

# Advantages
- Low-cost access to OpenAI APIs
- Globally accelerated with ECDN for ultimate speed anywhere
- No worries about OpenAI account suspension
- No usage time limit
- Access any AI model, just follow OpenAI's request format


# Usage Steps

Start by obtaining your [API key](https://www.openai-hub.com/faq/1.html#如何获取apikey) in the format beginning with `sk-*****************`.

**Update Your API Endpoint**
- Formerly `https://api.openai.com`
- Now `https://api.openai-hub.com` - simply add `-hub` at the end
- Most third-party programs can adjust the API endpoint. If you have a custom system, you'll need to modify it in your code.

**Key Points to Remember:**
- Avoid mixing the API key from the [Console](https://api.openai-hub.com) with keys from other sources.
- Ensure the API key format is without spaces and typically starts with sk-


#### Below, you'll find example code snippets for GPT conversation interfaces in various languages. These have been tested with the gpt-3.5-turbo model. For other models, please modify the `model` parameter. [Model Names](/price/chatgpt.html)

-------
## CURL Example Code
``` shell
curl --request POST 
--url https://api.openai-hub.com/v1/chat/completions 
--header 'Authorization: Bearer Replace_with_your_API_key' 
-H "Content-Type: application/json" 
--data '{
"max_tokens": 4000,
"model": "gpt-4", --Specify the model to call here; change model name for other models
"temperature": 0.8,
"top_p": 1,
"presence_penalty": 1,
"messages": [
        {
        "role": "system",
        "content": "This system content"
        },
        {
        "role": "user",
        "content": "Please, say test!"
        }
    ]
}'

## Community Chat


<p style="float:left;margin:30px;width:100%"><img width="240" height="240" src="/img/群聊二维码.png">
<img width="240" height="240" src="/img/tg.png"></p> 



## If you think this project is good, please give us a star⭐.
