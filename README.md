# CSIT6000R-group-14-project



Our experimental code was modified based on the original paper https://arxiv.org/abs/2304.05197, and the specific code can be found on GitHub https://github.com/HKUST-KnowComp/LLM-Multistep-Jailbreak.

In LLM-Multistep-Jailbreak-main_chatgpt4.0, by entering the correct API key, you can run experiments on ChatGPT 4.0 as reported. The file chatgpt_extraction.py follows the method from the original paper, whereas chatgpt_extraction_ka.py, chatgpt_extraction_ka_vi&rl.py, and chatgpt_extraction_vi&rl.py correspond to JQ+COT+MC+KA; JQ+COT+MC+VI+KA, JQ+COT+MC+RL+KA; and JQ+COT+MC+VI, JQ+COT+MC+RL, respectively. 

JQ+COT+MC+KA: jailbreak + assistant ack + query (guess included) + multi-gen + know answer 

JQ+COT+MC+VI+KA: jailbreak + assistant ack + query (guess included) + multi-gen +virtual + know answer 

JQ+COT+MC+RL+KA: jailbreak + assistant ack + query (guess included) + multi-gen +real + know answer 

JQ+COT+MC+VI: jailbreak + assistant ack + query (guess included) + multi-gen +virtual 

JQ+COT+MC+RL: jailbreak + assistant ack + query (guess included) + multi-gen +real



In LLM-Multistep-Jailbreak-main_ERNIE, by entering the correct API key, you can run experiments on ERNIE as reported. The file ERNIE_extraction.py follows the method from the original paper, whereas ERNIE_extraction_ka.py, ERNIE_extraction_ka_vi&rl.py, and ERNIE_extraction_vi&rl.py correspond to JQ+COT+KA; JQ+COT+VI+KA, JQ+COT+RL+KA; and JQ+COT+VI, JQ+COT+RL, respectively.

JQ+COT+KA: jailbreak + assistant ack + query (guess included) + know answer 

JQ+COT+VI+KA: jailbreak + assistant ack + query (guess included) +virtual + know answer 

JQ+COT+RL+KA: jailbreak + assistant ack + query (guess included) + real + know answer 

JQ+COT+VI: jailbreak + assistant ack + query (guess included) + virtual 

JQ+COT+RL: jailbreak + assistant ack + query (guess included) + real
