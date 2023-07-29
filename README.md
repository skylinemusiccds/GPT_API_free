<div align="center">
<img src="./images/logo.svg" alt="icon" width="50px"/>
<h1 align="center">GPT-API-free</h1>

Support **GPT-4** / GPT-3.5-Turbo / GPT-3.5-Turbo-16K / embeddings / DALL·E / whisper / text-davinci

Domestic dynamic acceleration direct connection without agent

[Mirror Site](https://chatapi.chatanywhere.cn/) / [Quick Start](#How to use) / [Get Free Key](https://api.chatanywhere.cn/v1/oauth/free/github /render) / [Support Paid Key](https://peiqi.shop/)

[QQ group: 829433227](https://qm.qq.com/cgi-bin/qm/qr?k=pi0iBUwIgrBOH4ndImSQEHpCcWkYfAWj&jump_from=webapi&authKey=H9UwoaXEbgrSK+4ArDlij1Y0/XEEumM+h7+cJPh1OYAkBhch19 cHSycBql+fIh+w3)

</div>

## Privacy Statement

The project takes privacy very seriously and is committed to protecting the privacy of its users. This project does not in any way collect, record or store any text entered by users or returned by OpenAI servers. The project does not provide OpenAI or any third party with any information about the identity of the API caller, including but not limited to IP addresses and user agent strings.

However, OpenAI officially retains data for 30 days according to its [Data Usage Policy](https://platform.openai.com/docs/data-usage-policies).

## 👏 Ads
[Commercial version domestic mirror station deployment authorization](https://docs.chatanywhere.com.cn/) supports integrated deployment of GPT, DALLE, Claude, Azure Openai, Midjourney, etc. In-site recharge and invitation functions are all available, see https://docs.chatanywhere.com.cn/ for details

## Update log
- **June 14, 2023** Adapt to GPT-3.5-Turbo-16K, free key also supports 16k model; paid key follows the official price and reduces the charge.

- **June 15, 2023** Adapted to the new functions of version 0613.

- **June 18, 2023** Added support for language-to-text model Whisper.

## Features
1. Support Models, Embedding, text-davinci, GPT-3.5-Turbo, GPT-3.5-Turbo-16K, ***GPT-4***(not supported in free version), ***DALLE***(free version not supported), ***Whisper*** (not supported in free version). (The free version can support AutoGPT and gpt_academic)
2. The interface standard is completely consistent with the official one, compatible with various software/plug-ins.
3. Support streaming response.
4. The domestic line uses dynamic acceleration, and the experience is far better than using a proxy to connect to the official website.
5. There is no need to scientifically access the Internet, and the domestic environment can be used directly.
6. It is completely free for personal use.

## 🚩 Notes

❗️**Free API Key can only be used for personal non-commercial use, education, non-profit research work. Commercial use is strictly prohibited, and large-scale training of commercial models is strictly prohibited! To train models for scientific research, please join the group and contact us in advance. **

❗️We will block the abused keys from time to time. If you find that your key has been blocked by mistake, please contact us through the QQ group.

For the long-term development of this project, the free API Key limits **120 requests/hour/IP&Key** call frequency, that is to say, if you use multiple Keys under one IP, the total number of requests per hour for all Keys cannot exceed 120; the same Reasonably, if you use a Key for multiple IPs, the number of requests per hour for this Key cannot exceed 120. (**Paid version API does not have this limitation**)

## Free to use

- **🚀[Click to get free API Key](https://api.chatanywhere.cn/v1/oauth/free/github/render)**
- **Forward Host1: `https://api.chatanywhere.cn` (for foreign servers)**
- **Forward Host2: `https://api.chatanywhere.com.cn` (domestic transfer, lower delay, recommended)**

***Do not use the free key on the mirror site https://chatapi.chatanywhere.cn/ will report an error***

We will regularly expand the capacity according to the usage. As long as we are not sanctioned by the government, we will always provide free API. If this project is helpful to you, please give us a ***Star***. If you encounter problems, you can report them in [Issues](https://github.com/chatanywhere/GPT_API_free/issues), and I will answer them when I have time.

The API Key is used to forward the API, and the Host needs to be changed to `api.chatanywhere.cn` or `api.chatanywhere.com.cn` (preferred in China)

## Paid API
- Providing free Keys for pure public welfare is obviously not a sustainable solution, so we introduce paid API Keys to maintain the daily expenses of the project to promote a virtuous circle of the project. We hope you understand.
- [Purchase low-cost paid Key](https://peiqi.shop/)

1. **Support GPT4 API**, the price is only 15% off the official price.
2. High cost performance, the price of other models except GPT4 is equivalent to one-seventh of the price on the official website.
3. The billing strategy is the same as that of the official website. Streaming Q&A uses the tiktoken library to accurately calculate Tokens, and non-streaming Q&A directly uses the official returned Tokens for billing.
4. The balance will not expire and is permanently valid. According to user feedback, 30 yuan is estimated to be able to be used for one year with moderate use of GPT3.5.
5. All interfaces are guaranteed to be forwarded from OpenAI official interfaces, non-peo, plus and other unstable solutions, no moisture, no adulteration, and stability is guaranteed.

## how to use
- Due to frequent malicious requests, we no longer directly provide public free keys, and now you need to bind your Github account to receive your own free keys.
- 🚀[Receive free API Key](https://api.chatanywhere.cn/v1/oauth/free/github/render) or [Purchase Paid API Key](https://peiqi.shop/)***( Do not use the free key for https://chatapi.chatanywhere.cn/ will report an error)***
- Forward Host1: `https://api.chatanywhere.cn` (for foreign servers)
- Forward Host2: `https://api.chatanywhere.com.cn` (domestic transfer, lower delay, recommended)
- Inquiry of balance and usage records (notifications and announcements will also be posted here): [Balance Inquiry and Announcements](https://api.chatanywhere.cn/)
- The forwarding API cannot directly initiate a request to the official interface api.openai.com. It needs to change the request address to api.chatanywhere.com.cn before it can be used. Most plug-ins and software can be modified.

## How to use common software/plugins

### The most convenient way to use
For your convenience, we have built two images based on open source projects:

1. Based on [ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web), domestic deployment, fast and stable. https://chatapi.chatanywhere.cn/
2. Based on [Chuanhu Chat](https://github.com/GaiZhenbiao/ChuanhuChatGPT), it supports networking functions, supports uploading PDF analysis, overseas deployment, and some people's network environment access may be stuck. https://chat1.chatanywhere.cn/

***Due to the access rate limit on IP, do not use the free Key on these two, it will report too many requests***

### **Python openai official library (using AutoGPT, langchain, etc.)**
Please refer to [demo.py](./demo.py) for sample code

***method one***

```python
import openai
openai.api_base = "https://api.chatanywhere.com.cn/v1"
# openai.api_base = "https://api.chatanywhere.cn/v1"
```

***Method 2 (method 1 doesn't work use this)***

Modify the environment variable OPENAI_API_BASE. Please search for how to change the environment variable in each system. If the environment variable does not work after modification, please restart the system.
```bash
OPENAI_API_BASE=https://api.chatanywhere.com.cn/v1
or OPENAI_API_BASE=https://api.chatanywhere.cn/v1
```
### **Open source gpt_academic**
Find the `API_URL_REDIRECT` configuration in the `config.py` file and modify it to the following:
```python
API_URL_REDIRECT = {"https://api.openai.com/v1/chat/completions": "https://api.chatanywhere.com.cn/v1/chat/completions"}
# API_URL_REDIRECT = {"https://api.openai.com/v1/chat/completions": "https://api.chatanywhere.cn/v1/chat/completions"}
```

### **ChatBox(recommended)**

ChatGPT is an open source desktop application that supports all desktop platforms.

Download link: https://github.com/Bin-Huang/chatbox/releases

How to use: Fill in the purchased key in the settings as shown in the figure, and set the proxy to `https://api.chatanywhere.cn` or `https://api.chatanywhere.com.cn`

![](images/chatbox.png)


### **Browser plugin ChatGPT Sidebar**

Official website link: https://chatgpt-sidebar.com/

After installing the plug-in, enter the settings page, modify the settings as shown in the figure, and change the url to `https://api.chatanywhere.cn` or `https://api.chatanywhere.com.cn`.

![](images/sidebar.png)

### **Jetbrains plugin ChatGPT**
<img src="./images/jet1.png" width='200'/>

After installing the plug-in, configure the plug-in as shown in the figure in Settings > Tools > OpenAI > GPT 3.5 Turbo. The key point is to modify the Server Settings to `https://api.chatanywhere.cn/v1/chat/completions` or `https ://api.chatanywhere.com.cn/v1/chat/completions`. And check Customize Server.

![](images/jet2.png)


### **VSCode plugin Code GPT**
<img src="./images/codegpt1.png" width='300'/>

This plug-in is relatively troublesome to modify the Host, and the source code needs to be modified before it can be used.

1. Install the plugin. After installation, press Ctrl+Shift+P, and enter Open Extensions Floder in the pop-up box
![](images/codegpt2.png)

2. Click Extensions: Open Extensions Floder, which will open the plugin directory, find the folder of Code GPT.
![](images/codegpt3.png)

3. After opening, enter and open the file ./src/clients/openai_client.js, search for api.openai.com in the file, and replace it with `api.chatanywhere.cn` or `api.chatanywhere.com.cn`. save document.
![](images/codegpt4.png)

4. Return to vscode again, press Ctrl+Shift+P, enter CodeGPT: Set API KEY in the pop-up box, and click CodeGPT: Set API KEY. Then enter the purchased Key into it.
![](images/codegpt5.png)

5. After the above steps are completed, restart VSCode

- Similar to other VSCode plugins.

### **Raycast plugin ChatGPT (recommended)**

1. Find the ChatGPT plugin in the Raycast Store, and follow the prompts to install it:
![](images/raycast1.png)

2. After the installation is complete, fill in our API Key in `API Key` in the plug-in configuration, and select `Change API Endpoint`, and fill in `https://api.chatanywhere.com` in `API Endpoint` .cn/v1`
![](images/raycast2.png)
![](images/raycast3.png)

3. 🍺enjoy it~
![](images/raycast4.gif)

## API error description
- Overload error

Specific error message:
```
{
   "error": {
     "message": "That model is currently overloaded with other requests. You can retry your request, or contact us through our help center at help.openai.com if the error persists. (Please include the request ID xxxxxxxxxxxx in your message.) ",
     "type": "server_error",
     "param": null,
     "code": null
   }
}
```
This error is caused by the high load of the OpenAI official server and has nothing to do with the forwarding server load. It usually recovers after a period of time, you can wait a few seconds and try again.


[![Star History Chart](https://api.star-history.com/svg?repos=chatanywhere/GPT_API_free&type=Date)](https://star-history.com/#star-history/star-history&Date )
