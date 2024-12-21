# 📍 Product Introduction
  ### Eternal Tales: 멀티모달 AI 챗봇과의 대화를 통한 펫로스 극복 서비스
![1 (7)](https://github.com/eternal-tales/.github/assets/59727077/f621615c-ecc5-4589-8bb8-27da76c8cb78)

`Eternal Tails` is a service that helps people who experience loss by leaving their pets they have spent together as family members to experience and remember their precious daily lives with their pets again, and eventually to help their pets recover to a healthy daily life.

`이터널 테일즈` 는 가족 구성원으로서 함께 지낸 반려동물을 먼저 떠나보내면서 상실감을 경험하는 이들을 위해, 반려동물과 함께했던 소중한 일상을 다시금 경험 및 추억하고, 최종적으로는 이후 반려인이 다시 건강한 일상으로 회복할 수 있도록 보조하는 역할을 수행하는 서비스입니다.



# 📍 My contribution
## AI Modelling ( Multi-modal Chatbot )

### 1. Task
Real-time Text and Image generation corresponding to user's message

### 2. Model
### 2.1. Text Generation: OpenAI GPT (Chat) API
- Making a chatting agent with user's pet information (user giving when joining the app).
  
### 2.2. Image Generation: [Dreambooth Fast Stable Diffusion](https://github.com/TheLastBen/fast-stable-diffusion)
- Using pre-training checkpoint: [runwayml/stable-diffusion-v1-5](https://huggingface.co/runwayml/stable-diffusion-v1-5)
- Finetuning a model with user's 5 pet photos (user giving when joining the app).

### 3. Dataset (Demo Examples)
**Dreambooth**(*kind of sd finetuning method*) makes it possible to finetune the model with only a few images. Therefore, we do not use a large dataset. We only use data of 5 images for finetuning. Finetuning takes about 30 minutes. The finetuning outputs(ckpts) are as follows.

<details>
<summary><strong>강아지 양파</strong></summary>
<div markdown="1">
1. <strong>Checkpoint:</strong> <a href="https://huggingface.co/dhdbsrlw/pet-onion">dhdbsrlw/pet-onion</a> <br>
2. Finetuning Images <br> (*src: Instagram <em>@pom_onion</em>)
  <div align="center">
  <img src="./fastapi/resources/assets/images/onion (1).jpg" alt="onion_1" width="15%" />
  <img src="./fastapi/resources/assets/images/onion (2).jpg" alt="onion_2" width="15%" />
  <img src="./fastapi/resources/assets/images/onion (3).jpg" alt="onion_3" width="15%" />
  <img src="./fastapi/resources/assets/images/onion (4).jpg" alt="onion_4" width="15%" />
  <img src="./fastapi/resources/assets/images/onion (5).jpg" alt="onion_5" width="15%" />
  </div>
</div>
</details>

<details>
<summary><strong>강아지 제로</strong></summary>
<div markdown="1">
1. <strong>Checkpoint:</strong> <a href="https://huggingface.co/dhdbsrlw/pet-zero">dhdbsrlw/pet-zero</a> <br>
2. Finetuning Images <br> (*src: Google)
  <div align="center">
  <img src="./fastapi/resources/assets/images/zero (1).jpg" alt="zero_1" width="15%" />
  <img src="./fastapi/resources/assets/images/zero (2).jpg" alt="zero_2" width="15%" />
  <img src="./fastapi/resources/assets/images/zero (3).jpg" alt="zero_3" width="15%" />
  <img src="./fastapi/resources/assets/images/zero (4).jpg" alt="zero_4" width="15%" />
  <img src="./fastapi/resources/assets/images/zero (5).jpg" alt="zero_5" width="15%" />
  </div>
</div>
</details>

<details>
<summary><strong>강아지 몽자</strong></summary>
<div markdown="1">
1. <strong>Checkpoint:</strong> <a href="https://huggingface.co/dhdbsrlw/pet-monga">dhdbsrlw/pet-monga</a> <br>
2. Finetuning Images <br> (*src: Instagram <em>@mongja0408</em>)
  <div align="center">
  <img src="./fastapi/resources/assets/images/monga (1).jpg" alt="monga_1" width="15%" />
  <img src="./fastapi/resources/assets/images/monga (2).jpg" alt="monga_2" width="15%" />
  <img src="./fastapi/resources/assets/images/monga (3).jpg" alt="monga_3" width="15%" />
  <img src="./fastapi/resources/assets/images/monga (4).jpg" alt="monga_4" width="15%" />
  <img src="./fastapi/resources/assets/images/monga (5).jpg" alt="monga_5" width="15%" />
  </div>
</div>
</details>


## 4. Generation Output
<div align="center">
  <img src="./images/app/join_app.jpg" alt="Join" width="45%" />
  <img src="./images/app/chat_app.jpg" alt="Chat" width="45%" />
</div>

### More generation outputs can be accessed in [here](https://github.com/eternal-tales/AI/tree/main/images/inference) !
<br>

---
(Last Update: 2024/02/10) <br>
Contact: dhdbsrlw@korea.ac.kr
