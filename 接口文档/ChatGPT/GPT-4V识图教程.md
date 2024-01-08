---
title: GPT-4V识图教程

meta:
  - name: keywords
    content: GPT-4 Turbo, 视觉功能, API使用, 示例代码, 类型展示, 官方文档
  - name: description
    content: 本教程提供了GPT-4 Turbo具有视觉功能版本的使用方法，包括注意事项、示例代码和相关类型展示。它详细介绍了如何通过API调用进行图像分析，以及如何利用这一功能进行图片比较和内容解释。
---
# GPT4V识图教程

::: tip 注意
- 具有视觉功能的 GPT-4 Turbo 的行为可能与 GPT-4 Turbo 略有不同，他会自动将系统消息插入到对话中
- 具有视觉功能的 GPT-4 Turbo 与 GPT-4 Turbo 预览模型相同，在文本任务上表现同样出色，但增加了视觉功能
- 视觉只是该模型具有的众多功能之一

[点击前往官方文档](https://platform.openai.com/docs/guides/vision)
:::



#### 示例代码
``` shell
curl https://api.openai-hub.com/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer $OPENAI_API_KEY" \
  -d '{
    "model": "gpt-4-vision-preview",
    "messages": [
    {
      "role": "user",
      "content": [
        {
          "type": "text",
          "text": "What are in these images? Is there any difference between them?",
        },
        {
          "type": "image_url",
          "image_url": {
            "url": "https://upload.wikimedia.org/wikipedia/commons/thumb/d/dd/Gfp-wisconsin-madison-the-nature-boardwalk.jpg/2560px-Gfp-wisconsin-madison-the-nature-boardwalk.jpg",
          },
        },
        {
          "type": "image_url",
          "image_url": {
            "url": "https://upload.wikimedia.org/wikipedia/commons/thumb/d/dd/Gfp-wisconsin-madison-the-nature-boardwalk.jpg/2560px-Gfp-wisconsin-madison-the-nature-boardwalk.jpg",
          },
        },
      ],
    }
  ],
    "max_tokens": 300
  }'

```

#### 类型展示
