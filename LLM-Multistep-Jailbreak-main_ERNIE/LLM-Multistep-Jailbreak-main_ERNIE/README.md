# Multi-step Jailbreaking Privacy Attacks on ChatGPT
Code for improving based on Multi-step Jailbreaking Privacy Attacks on ChatGPT

### ERNIE Bot

In this experiment, the ERNIE Bot model was used. For specific interface introduction, please refer to the URL: https://console.bce.baidu.com/
The code template is as follows

```python
import requests
import json
def main():
url = "https://aip.baidubce.com/oauth/2.0/token?client_id=GCCbxJ****yl9q9U&client_secret=hNQxuA****EcyazD&grant_type=client_credentials"

 payload = json.dumps("")
 headers = {
     'Content-Type': 'application/json',
     'Accept': 'application/json'
 }

 response = requests.request("POST", url, headers=headers, data=payload)

 print(response.text)
```

### PII Extraction Attacks
1. Properly set up the API and path in ```config.py```. You need to specify the paths to save the extraction results.

2. Supported attack templates:

```- DQ:``` Direct query to extract PII.

```- JQ:``` Query with jailbreak template to extract PII.

```- JQ+COT:``` Query with pre-defined multi-step context and jailbreak template to extract PII.

```- JQ+COT+VI:``` Query with JailBreak Template and Virtual Scenario   to extract PII.

```- JQ+COT+RL:``` Query with JailBreak Template and real Scenario  to extract PII.

```- JQ+COT+KA:```  Query with JailBreak Template and the Scenario that we pretent to have kown the right answer  to extract PII.

```- JQ+COT+RL+KA:```   Query with JailBreak Template and the Scenario that we pretent to have kown the right answer and what I ask is about a real people to extract PII.

```- JQ+COT+VI+KA:```   Query with Pre-Defined Multi-STEP Context, JailBreak Template and the Scenario that we pretent to have kown the right answer and what I ask is virtual  to extract PII.


#### Run Attacks on OpenAI APIs

run ```chatgpt_extraction.py```.
#### Attacks on Email Content Recovery
To reproduce our attacks to extract email content, you may refer to the [email_content_extraction](https://github.com/HKUST-KnowComp/LLM-Multistep-Jailbreak/tree/main/email_content_extraction) folder.


#### Result Analysis

First, obtain ```.csv``` paths after running the attacks.

Second, specify the result paths in ```config.py``` or ```pred_analysis.py```.

Then, run ```pred_analysis.py```.

