```markdown
<p align="center">
  <img src="/img/logo.webp" width="120" height="120" alt="OpenAI-Hub"/>
  <h1 align="center">OpenAI-Hub</h1>
</p>
<p align="center"><a>简体中文</a> | <a href="/README.en.md">English</a></p>

<p style="font-size:18px" align="center">لا حاجة لخادم وكلفة منخفضة للوصول إلى واجهة برمجة تطبيقات OpenAI</p>


> [Official Address](https://www.openai-hub.com) | 
> [API Documentation](https://www.openai-hub.com/api/) | 
> [Open Platform](https://api.openai-hub.com)

# عملية الاستخدام

أولاً، احصل على [مفتاح الواجهة البرمجية (API key)](https://www.openai-hub.com/faq/1.html#如何获取apikey) الخاص بك، الشكل يبدأ بـ `sk-*****************`

**قم بتغيير عنوان الواجهة الخاصة بك**
- السابق `https://api.openai.com`
- الآن `https://api.openai-hub.com` كل ما عليك هو إضافة `-hub` في نهاية الرابط
- يمكن تغيير عناوين الواجهة في 99% من البرامج المتوفرة. إذا كان النظام الخاص بك مطوراً من قبلك، فسيتعين عليك تعديل الشيفرة.

**هناك بعض النقاط التي يجب مراعاتها:**
- لا يمكن استخدام [مفتاح الواجهة (API key)](https://api.openai-hub.com) من لوحة التحكم مع مفاتيح API من مصادر أخرى
- [مفتاح الواجهة (API key)](/faq/1.html#如何获取apikey) لا يجب أن يحتوي على مسافات، الشكل المعتاد يبدأ بـ sk-

#### هنا أمثلة لشفرات الأنماط المتعددة لواجهة GPT للحوار، يتم اختبار النموذج gpt-3.5-turbo فقط، يرجى تغيير معلمة النموذج [اسم النموذج](/price/chatgpt.html)

-------
## شفرة مثال CURL
``` shell
curl --request POST 
--url https://api.openai-hub.com/v1/chat/completions 
--header 'Authorization: Bearer استبدل بمفتاحك الشخصي لواجهة البرمجة' 
-H "Content-Type: application/json" 
--data '{
"max_tokens": 4000,
"model": "النموذج الذي ترغب في استخدامه",
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

## مجموعة النقاش

<img width="240" height="240" src="/img/群聊二维码.png">
--------------------------------
```