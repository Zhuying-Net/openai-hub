
# 关于GPTs多模态功能的概述和应用指南

> OpenAI尚未开放GPTs的官方API，但通过逆向工程，可以访问OpenAI官网上的所有GPTs应用。GPTs应用商店已包含数以万计的应用程序，涵盖广泛的用途。

### 如何使用GPTs多模态功能：

1. **模型名称：** 使用格式 `gpt-4-gizmo-gizmo_id` 来指定模型。例如，要调用官方DALL·E，使用的模型ID为 `g-2fkFE8rbu`，因此完整的模型名称是 `gpt-4-gizmo-g-2fkFE8rbu`。

2. **获取gizmo_id：** 你可以访问[这里](/faq/8)获取更多关于如何获得gizmo_id的信息。

3. **在线体验：** 提供在线体验教程，详见[此处](/faq/9)。

4. **GPTs商店：** 探索GPTs商店，浏览众多应用，[点击此处访问](https://www.gptshunter.com/)。

### 调用示例：

#### 官方DALL-E调用示例：

使用以下命令调用DALL-E模型：

```shell
curl https://api.openai-hub.com/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer API_KEY" \
  -d '{
    "model": "gpt-4-gizmo-g-2fkFE8rbu",
    "messages": [
      {
        "role": "user",
        "content": "a Cat"
      }
    ],
    "max_tokens": 3000
  }'
```


#### GPTs应用列表（仅列举部分） 

::: warning DALL-E
DALL-E :gpt-4-gizmo-g-2fkFE8rbu\
将你的想象转化为图像。
:::

::: danger Data Analysis
Data Analysis：gpt-4-gizmo-g-HMNcP6w7d\
放入任何文件，分析和可视化数据。
:::

::: tip ChatGPT Classic
ChatGPT Classic：gpt-4-gizmo-g-YyyyMT9XH\
GPT-4的最新版，无附加功能。
::: 


::: warning Web Browser
Web Browser：gpt-4-gizmo-g-3w1rEXGE0\
浏览网页以收集信息或进行研究。
::: 

::: danger Creative Writing Coach
Creative Writing Coach：gpt-4-gizmo-g-lN1gKFnvL\
 阅读作品并提供反馈以提高写作技能。
::: 