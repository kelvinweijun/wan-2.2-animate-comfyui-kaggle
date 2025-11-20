# Wan 2.2 Animate 14B ComfyUI on Kaggle
Contains the notebooks and workflows specifically configured to run inference from Wan 2.2 Animate with ComfyUI on Kaggle T4 GPUs smoothly. There are 3 different types of notebooks and 3 different variants of Kijai's modified workflows. 
# Prerequisites
Before running the notebook on Kaggle, there are models and files you may need to install. The notebooks will automatically symlink the model files locations to the ComfyUI kaggle/working/ComfyUI directory, but you'll need to ensure that the models are placed in the correct kaggle input directory with the exact name mentioned here. Below are the specifications and the links to the models:

## Models
### GGUF Model ` /kaggle/input/wan-animate-q3_k_m-gguf `
- **Wan 2.2 Animate 14B Q3_K_M GGUF** — https://huggingface.co/QuantStack/Wan2.2-Animate-14B-GGUF/blob/main/Wan2.2-Animate-14B-Q3_K_M.gguf

### Text Encoder ` /kaggle/input/wan-animate-text-encoder `
- **UMT5 XXL FP16 Safetensor** — https://huggingface.co/Comfy-Org/Wan_2.2_ComfyUI_Repackaged/blob/main/split_files/text_encoders/umt5_xxl_fp16.safetensors

### VAE ` /kaggle/input/wan-animate-vae `
- **Wan 2.1 VAE BF16 Safetensor** — https://huggingface.co/Kijai/WanVideo_comfy/blob/main/Wan2_1_VAE_bf16.safetensors

### LoRAs ` /kaggle/input/wan-animate-loras `
- **Wan Animate Relight LoRA FP16 Safetensor** — https://huggingface.co/Kijai/WanVideo_comfy/blob/main/LoRAs/Wan22_relight/WanAnimate_relight_lora_fp16.safetensors  
- **LightX2V I2V 14B 480p** — https://huggingface.co/Kijai/WanVideo_comfy/blob/main/Lightx2v/lightx2v_I2V_14B_480p_cfg_step_distill_rank64_bf16.safetensors

### Clip Vision ` /kaggle/input/wan-animate-clip-vision `
- **Clip Vision Safetensor** — https://huggingface.co/Comfy-Org/Wan_2.1_ComfyUI_repackaged/tree/main/split_files/clip_vision

## Custom Nodes
### Core Plugins  ` /kaggle/input/wan-animate-custom-nodes/custom_nodes `
- **ComfyUI-Manager** — https://github.com/ltdrdata/ComfyUI-Manager.git  
- **ComfyUI-GGUF** — https://github.com/city96/ComfyUI-GGUF.git  
- **ComfyUI-WanVideoWrapper** — https://github.com/kijai/ComfyUI-WanVideoWrapper.git  

### Kijai Workflow Requirements
- **ComfyUI-KJNodes** — https://github.com/kijai/ComfyUI-KJNodes.git  
- **comfyui_controlnet_aux** — https://github.com/Fannovel16/comfyui_controlnet_aux.git  
- **ComfyUI-VideoHelperSuite** — https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite.git  
- **ComfyUI-segment-anything-2** — https://github.com/kijai/ComfyUI-segment-anything-2.git  
- **ComfyUI-Advanced-ControlNet** — https://github.com/Kosinkadink/ComfyUI-Advanced-ControlNet.git  
- **comfyui-tooling-nodes** — https://github.com/Acly/comfyui-tooling-nodes.git  
- **ComfyUI_essentials** — https://github.com/cubiq/ComfyUI_essentials.git  

### Additional Required Nodes
- **cg-use-everywhere** — https://github.com/chrisgoringe/cg-use-everywhere.git  
- **was-node-suite-comfyui** — https://github.com/WASasquatch/was-node-suite-comfyui.git  
- **ComfyUI-Custom-Scripts** — https://github.com/pythongosssss/ComfyUI-Custom-Scripts.git  
- **ComfyUI-Frame-Interpolation** — https://github.com/Fannovel16/ComfyUI-Frame-Interpolation.git  
- **rgthree-comfy** — https://github.com/rgthree/rgthree-comfy.git  
- **ComfyMath** — https://github.com/evanspearman/ComfyMath.git  
- **ComfyUI-Easy-Use** — https://github.com/yolain/ComfyUI-Easy-Use.git  
- **comfyui-mixlab-nodes** — https://github.com/MixLabPro/comfyui-mixlab-nodes.git  

