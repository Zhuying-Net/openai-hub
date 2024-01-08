
<p align="center">
  <img src="/img/logo.webp" width="120" height="120" alt="OpenAI-Hub"/>
  <h1 align="center">OpenAI-Hub</h1>
</p>
<p align="center"><a>English</a> | <a href="/README.md">简体中文</a></p>

<p style="font-size:18px" align="center">无需代理服务器&amp;低成本访问OpenAI接口</p>


> [官方地址](https://www.openai-hub.com) | 
> [接口文档](https://www.openai-hub.com/api/) | 
> [开放平台](https://api.openai-hub.com)

# 使用步骤

首先获取你的 [APIkey](https://www.openai-hub.com/faq/1.html#如何获取apikey) 格式为 `sk-*****************` 开头

**更改你的接口地址**
- 原来 `https://api.openai.com`
- 现在 `https://api.openai-hub.com` 只需要在后面加上`-hub`即可
- 市面上99%的程序都可以更改接口地址。如果是自己开发的系统，需要在代码里面修改。

**有几个注意的地方：**
- [控制台](https://api.openai-hub.com)的APIkey不能和其他渠道的APIkey混用
- [APIkey](/faq/1.html#如何获取apikey)不能带空格，格式通常为sk-开头的


#### 以下是GPT对话接口各语言示例代码，仅测试gpt-3.5-turbo模型，其余模型请更改model参数 [模型名称](/price/chatgpt.html)

-------
## CURL 示例代码
``` shell
curl --request POST 
--url https://api.openai-hub.com/v1/chat/completions 
--header 'Authorization: Bearer 替换为你的APIkey' 
-H "Content-Type: application/json" 
--data '{
"max_tokens": 4000,
"model": "需要调用的模型",
"temperature": 0.8,
"top_p": 1,
"presence_penalty": 1,
"messages": [
        {
        "role": "system",
        "content": "This system content"
        },
        {
        "role": "user",
        "content": "pls,say test!"
        }
    ]
}'
```

## 交流群

<img width="240" height="240" src="/img/群聊二维码.png">
