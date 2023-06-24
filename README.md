# Pinecone hack

## Python setup

```sh
# Install deps
sudo apt install python3-pip
sudo apt install python3.11-venv

# Create env
python3 -m venv ./venv
source ./venv/bin/activate

# Exit venv
deactivate
```

## CUDA setup

```sh
sudo apt install nvidia-driver-530 nvidia-dkms-530 nvidia-cuda-toolkit -y && reboot
```

## Potential ideas

- Chess cheat detection: No labelled data to work on. Already made by https://github.com/clarkerubber/irwin which analyses principle variance (PV) by running stockfish. Also not original.
- Skin cancer detection: cringe
- Add voice support to your whatsapp chatbot. Transcribe audio to text format, then feed to chatbot
- Dota coach: Analyse minimap and player movements to suggest strategy. Eg. TP to mid, blink and ravage etc. Needs training data, not a hackathon project.
- Zoom flex: analyze confidence levels and status symbols in a zoom meet.

## AI companies

- character.ai: ChatGPT but with chat with characters you create- eg Mario, waifu etc.
- insitro: Drug discovery. Predicts pathways that are more likely to yield.
- Repl.it: Has its own Github copilot
- hippocraticai.com: Specialist LLM for medicine, outperforms GPT-4.
- cohere.ai: Pre-trained models behind API. Has generation LLMs (GPT), representation LLMs (BERT), classification API, similarity API. Examples provided:
  - Customer support / intent recognition: classify customer emails into different categories like inquiry, cancellation etc.
  - Text summarization
  - Sentiment analysis / toxicity detection
- replicate.com: Cloud to run models
-

## Stack structure

- Infra (compute): Nvidia, replicate (hosting)
- Infra (storage): Pinecone
- Model builders: Eg. GPT by OpenAI, voice generation model by ElevenLabs. Given input X, output Y. Outputs are either generative (new text or image), or representative (metadata extraction, vector)
- Model as API, eg. cohere. For enterprises (B2B)
- Consumer AI, eg. Alexa, ChatGPT.


## Cohere capabilities

- Text: generation, summarization, classification, search, moderation
- Entity extraction

