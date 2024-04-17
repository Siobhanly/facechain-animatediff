# facechain-animatediff
  基于AnimateDiff的以人为主体的动态变化
## 概述
本方案充分利用了AnimateDiff在动画生成方面的优势，通过集成新的模块来解决视频生成过程中的一致性和稳定性问题。新模块的设计旨在增强AnimateDiff的能力，使其能够生成与用户输入的描述性Prompt一致的生动有趣的视频内容。此外，方案还包括了对人物动作和表情的连贯性控制，以及对视频风格和情感基调的调整，从而确保生成的视频不仅在视觉上吸引人，而且在叙事上也具有吸引力。通过解析用户的叙事性Prompt，方案能够提取关键信息，并将其转化为详细的分镜脚本，这些脚本随后用于指导AnimateDiff生成连贯且具有叙事性的视频。通过引入叙事性Prompt解析和模块化Prompt生成，方案能够生成更加丰富和多样化的视频内容。
## 模块设计
- 剧本共创
- 分镜生成器
- 视频生成与渲染
- 用户交互界面
## 技术实现
- 通过接入大语言模型LLM，引导用户思考，生成剧本，提取关键信息，并辅助创作更加丰富的剧本内容。
- 对话管理系统设计一个对话流程，通过一系列的提问和回答，引导用户提供剧本所需的详细信息，如人物、场景、动作和情感状态。
- 结合剧本解析结果和预先定义的分镜模板，借助LLM来构建分镜脚本，并预设人物特征，保证人物一致性。
- AnimateDiff采样，根据分镜脚本中的指示创建角色、背景和动作的图像。
- 将生成的帧序列组装成连贯的视频片段。
- 通过ComfyUI实现用户交互，为用户提供一个清晰、易用的操作界面，使动画生成过程变得更加简单和直观。
## 主要特点
- 模块化设计  
- 用户友好性
- 自动化流程
  
## 效果展示

<img width="522" alt="image" src="https://github.com/Siobhanly/facechain-animatediff/assets/79733645/309c078f-4215-419f-a2db-15176af9bf5d">
<img width="640" alt="image" src="https://github.com/Siobhanly/facechain-animatediff/assets/79733645/009dd7a8-3e65-465a-bb6b-49043efcb946">
<img width="640" alt="image" src="https://github.com/Siobhanly/facechain-animatediff/assets/79733645/e17f5946-df89-48a2-b106-4143b17b02b5">
<img width="640" alt="image" src="https://github.com/Siobhanly/facechain-animatediff/assets/79733645/54b23341-b92d-43ad-ab96-3eb8afbbf171">
<img width="438" alt="image" src="https://github.com/Siobhanly/facechain-animatediff/assets/79733645/0f9592ae-fcbc-41ea-a296-aa1f3a5bd13a">
<img width="453" alt="image" src="https://github.com/Siobhanly/facechain-animatediff/assets/79733645/e01256a7-56ee-4f47-9326-525fbd0edcef">
<img width="360" alt="image" src="https://github.com/Siobhanly/facechain-animatediff/assets/79733645/dd9a4c94-d2a4-49ba-a446-c3a34e30fa5f">
<img width="360" alt="image" src="https://github.com/Siobhanly/facechain-animatediff/assets/79733645/0c80eadd-a6ce-465a-ab99-3627f0c8f681">


https://github.com/Siobhanly/facechain-animatediff/assets/79733645/9526d002-2abc-48a6-bf5e-3b3fbae362ec

