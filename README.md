## Hi, I'm Zichun Ai

I'm an MSc student in **Internet of Things with AI** at the **University of Bristol**. I enjoy taking computer-vision models out of the notebook and making them run fast and reliably on real camera streams.

> **Looking for PhD positions (2027 entry)** in efficient on-device AI, computer vision and multimodal learning, and for research-related roles.

<!-- Add links here when ready, for example:
[Email](mailto:your-address) · [CV](link-to-pdf) · [LinkedIn](link-to-profile)
-->

### Research interests, and what I've done so far

- **Efficient model deployment, towards edge AI.** In [car_detect](https://github.com/guagua-paopao/car_detect), moving image handling onto the GPU cut full-pipeline processing time per frame from 43.8 ms to 17.9 ms (−59%) with no change in output on the frames checked, measured on an RTX 4080 laptop GPU. I haven't deployed on dedicated edge hardware yet, and that is where I'd like to go next.
- **Computer vision on live video.** [vision_project](https://github.com/guagua-paopao/vision_project) detects and tracks people on a live RTSP stream, counts line crossings and applies pose rules, with one decoded stream shared by several tasks.
- **Multimodal learning.** An audio-visual lip-reading project (20 spoken names, code not public) reached 91% accuracy by combining lip video and audio, compared with 79% for video alone and about 90% for audio alone.
- **Data quality and knowing when a model is unsure.** Early in car_detect, a manual review found 379 of the first 600 priority samples unusable and 3,254 automatically generated labels too unreliable to train on, and the system answers "unknown" when it isn't confident. [chat_model_service](https://github.com/guagua-paopao/chat_model_service) takes the same approach with language models: it cites its sources and declines to answer when the documents don't cover a question.

### Selected projects

| Project | What it is | Built with |
|---|---|---|
| [vision_project](https://github.com/guagua-paopao/vision_project) | Real-time people-flow analytics: tracking, line counting, electronic fence, pose rules | C++, CUDA, TensorRT, YOLO11-pose, FFmpeg, Redis |
| [car_detect](https://github.com/guagua-paopao/car_detect) | Two-stage vehicle detection, then body-type and colour recognition | C++, CUDA, TensorRT, ONNX, PostgreSQL |
| [chat_model_service](https://github.com/guagua-paopao/chat_model_service) | Company-document Q&A assistant built on large language models (RAG) | Python, FastAPI, Next.js, PostgreSQL + pgvector |

### Other projects (code not public)

- **Fall detection with smartphone sensors**: compared 7 machine-learning models on accelerometer, gyroscope and barometer data. The best model reached 94.4% accuracy (fall F1 0.916) and runs on Android, sending an SMS with GPS location if the user doesn't respond.
- **Scene classification**: 15 indoor and outdoor scene types. Hand-crafted features (HOG + SVM) reached 48.6%; fine-tuning ResNet-18 reached 93.1%.

### Education

- **MSc Internet of Things with AI**, University of Bristol, 2026 – 2027
- **BSc (Hons) Computing Science**, University of East Anglia, 2026 (First Class)

### Experience

- **Machine-vision intern** (Apr – Jun 2026): people-flow and vehicle analytics on live RTSP camera streams, with TensorRT/CUDA GPU deployment
- **Java development intern** (Jul – Aug 2026): a finance-reporting business system built with Vue 3, Spring Boot, MyBatis-Plus and MySQL

### Tools I use

Python · C++ · Java · CUDA · TensorRT · ONNX · OpenCV · TensorFlow/Keras · scikit-learn · FFmpeg · FastAPI · Spring Boot · Vue 3 · PostgreSQL · MySQL · Redis · Docker · Git
