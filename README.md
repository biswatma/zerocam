
# 📸 ZeroCam - Camera Interaction App

A browser-based application that uses the webcam to capture live video, processes frames with a locally run vision-language model (SmolVLM), and returns responses based on user-given instructions. Perfect for experimenting with real-time visual AI interactions!

## [Demo link](https://biswatma.github.io/zerocam/)

---

## 🔍 Features

- 🚀 Uses **WebGPU** for local inference – no server roundtrip required.
- 🤖 Powered by HuggingFace's [SmolVLM-500M-Instruct](https://huggingface.co/HuggingFaceTB/SmolVLM-500M-Instruct) model.
- 📷 Captures frames from your webcam and feeds them into a Vision-to-Text model.
- ⌛ Choose intervals between frame inferences (0ms to 2s).
- 🧠 Real-time interpretation of visual input based on a text instruction.

---

## 📦 Tech Stack

- **HTML/CSS/JavaScript**
- [HuggingFace Transformers.js](https://github.com/huggingface/transformers.js)
- **WebGPU** for on-device model inference
- **SmolVLM-500M-Instruct** model (vision-language model)
- No server needed — everything runs in the browser

---

## 📋 Requirements

- Browser with **WebGPU support** (e.g., recent versions of Chrome/Edge with WebGPU enabled)
- HTTPS or localhost (for webcam access)

---

## 🛠️ Setup & Usage

1. **Clone or open the HTML file locally**  
   You can open the file directly in your browser (Chrome preferred with WebGPU enabled).

2. **Grant Camera Access**  
   When prompted, allow camera permissions.

3. **Enter an Instruction**  
   E.g., _"What is in the frame?"_ or _"Describe the surroundings."_

4. **Choose a Frame Capture Interval**  
   Select from dropdown (e.g., 500ms).

5. **Click Start**  
   The app will begin capturing and interpreting your camera feed in real time.

---

## 📄 Example Use Cases

- Object detection with a natural language query
- Basic scene description
- Real-time captioning of your surroundings
- Building AI-powered smart mirror or surveillance prototypes

---

## ⚠️ Known Limitations

- Requires a browser with **WebGPU** support.
- Inference might be slow or memory-intensive on low-end devices.
- Cannot run on Safari (as of now) or unsecured (`http://`) domains.
- Cannot run on mobile browsers without WebGPU.

---

## 🧪 Advanced

### Supported Instructions:
The model accepts a wide range of natural language instructions, such as:
- "What objects do you see?"
- "Describe the weather in this scene."
- "Is anyone wearing red?"

### Model Info:
- **Model**: `HuggingFaceTB/SmolVLM-500M-Instruct`
- **Backed by**: [transformers.js](https://github.com/huggingface/transformers.js)
- **Inference device**: `webgpu`

---

## 🧹 Cleanup

When you close or refresh the browser, the app will automatically stop the camera.

---

## 📚 References

- [Transformers.js Documentation](https://huggingface.co/docs/transformers.js)
- [SmolVLM Model Card](https://huggingface.co/HuggingFaceTB/SmolVLM-500M-Instruct)
- [WebGPU Support Guide](https://developer.mozilla.org/en-US/docs/Web/API/WebGPU_API)

---

## 🤝 Contributing

Feel free to fork, tweak, and improve this for your own use case. PRs welcome!

---

## 📜 License

MIT License – Use freely, attribute accordingly.
