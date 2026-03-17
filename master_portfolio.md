# MASTER PORTFOLIO SOURCE FILE

## /summary

I am an AI Research Engineer specializing in image-based scientific data, with a strong focus on computer vision, signal processing, and representation learning.

My work sits at the intersection of **research and real-world applications**: I design models, build pipelines, and evaluate them rigorously, while ensuring they solve concrete problems for end users.

I am particularly interested in problems where:
- data is complex, noisy, or high-dimensional  
- understanding the structure of the signal matters as much as the model itself  
- solutions must be both **technically sound and operationally useful**

I enjoy working on challenging problems that require deep thinking and have a tangible, positive impact.

---

## /what_i_do

- Design and implement machine learning and deep learning models for image and signal data  
- Conduct literature reviews and identify gaps in existing approaches  
- Build end-to-end research pipelines (data → model → evaluation → interpretation)  
- Work with domain experts to translate real-world needs into technical solutions  
- Develop tools that bridge the gap between raw data and actionable insights  

---

## /core_expertise

### AI & Machine Learning
- Deep learning (CNNs, Transformers, generative models)  
- Representation learning for complex data  
- Optimization and probabilistic modeling  
- Experiment design, benchmarking, and evaluation  

### Computer Vision & Image Processing
- Segmentation, detection, feature extraction  
- Spectral analysis and multispectral data processing  
- Denoising, super-resolution, registration  
- Document image analysis and OCR pipelines  

### Geospatial & Scientific Data
- Remote sensing and Earth Observation  
- Raster/vector data processing  
- Multisensor data fusion  
- Coordinate systems and geospatial pipelines  

---

## /technical_skills

### Programming
- Python, C++, Matlab  

### ML Frameworks
- PyTorch, TensorFlow, Keras, Scikit-learn  
- Optuna (hyperparameter optimization)  

### Python Ecosystem
- numpy, pandas, scipy  
- matplotlib  
- opencv, scikit-image  
- rasterio, geopandas, shapely  
- xarray  

### MLOps & Tools
- Git  
- Docker (working knowledge)  
- ONNX, TensorRT  
- Gradio, Hugging Face  
- LangChain  
- Linux  

### Data & Infrastructure
- API integration  
- CUDA  

---

## /scientific_background

- Linear algebra, matrix calculus  
- Signal processing (Fourier, Laplace transforms)  
- Partial differential equations  
- Control theory, Kalman filters  
- State-space representations  
- Inverse problems  
- Optimization  
- Probabilistic modeling  
- Geometry  

---

## /engineering_practices

- Reproducible experimentation  
- Modular and maintainable code  
- Dataset curation and pipeline design  
- Training and evaluation infrastructure  
- Systematic benchmarking (baselines, ablations, metrics)  

---

## /domains

- Earth Observation & geospatial intelligence  
- Environmental monitoring  
- Document intelligence  
- Medical imaging (exploration)  
- Robotics & automation  
- Scientific data processing  

---

## /how_i_work

When approaching a new problem, I start by building a **deep understanding of the context**:
- What problem are we solving, and for whom?
- What are the constraints, objectives, and available resources?
- What makes the problem difficult?

I then focus on the data:
- understanding its structure, limitations, and signal content  
- identifying what information is already available and what is missing  

From there:
- I explore relevant literature and methods  
- identify what can transfer to the problem  
- implement and iterate through rigorous experimentation  

My workflow is fundamentally:
**understanding → modeling → experimentation → evaluation → iteration**

I naturally lean toward **theory → implementation**, but always with a focus on usefulness and real-world impact.

---

## /projects

### Attention-NMF — Multispectral Image Decomposition

**Context**: Research internship (Synchromedia Lab)  

**Problem**  
Blind spectral unmixing of multispectral images of ancient documents, aiming to decompose complex data into interpretable components.

**Approach**  
- Hybrid model combining autoencoder architecture and Non-negative Matrix Factorization  
- Attention mechanisms to focus on relevant spatial regions  
- Orthogonality constraints to improve decomposition quality  

**Technologies**  
CNNs, attention mechanisms, NMF  

**Contributions**  
- Proposed a novel hybrid AE + NMF architecture  
- Addressed an underexplored research problem  
- Reduced model parameters while improving performance  
- Designed and validated experiments on real degraded data  

**Results**  
- Outperformed state-of-the-art baselines  
- Improved handling of nonlinear multispectral data  
- Enhanced interpretability and efficiency  

**Research Output**  
- Paper: *Attention-based AE Orthogonal NMF for Blind Image Decomposition*  
- Submitted to ICASSP 2025 (2 marginal accepts, 1 marginal reject)  
- Code available  

**What I learned**  
End-to-end research ownership: from literature review and problem framing to implementation, evaluation, and scientific communication.

---

### SENWISE — Thermal Earth Observation Fusion (ESA)

**Context**: Research project (Diginove, ESA collaboration)  

**Problem**  
Simulate future satellite capabilities (LSTM mission) by fusing multisensor EO data to produce high-resolution thermal imagery.

**Approach**  
- GAN-based spatio-temporal fusion of Sentinel-3 and Landsat data  
- Time-series analysis for environmental monitoring (e.g., fire conditions)  
- Large-scale dataset curation (hundreds of GB)  

**Technologies**  
Python, geospatial libraries, deep learning, APIs  

**Contributions**  
- Led the project on Diginove’s side (sole contributor / point of contact)  
- Built datasets and fusion models  
- Integrated model into internal tools for operational use  
- Collaborated with domain experts and end-users (firefighters)  

**Results**  
- Improved performance over existing STF methods  
- Validated against in-situ measurements  
- Poster presented at AI4EO 2025  
- Paper in progress  

**Evaluation**  
- MAE, SSIM  
- Benchmarking against high-resolution references  

**What I learned**  
- Leading a research project in a multi-partner environment  
- Bridging research and operational needs  
- Designing solutions with end-users in mind  

---

### Agent4EO — Agentic Earth Observation Interface

**Context**: Personal project  

**Problem**  
Bridging the gap between geospatial data and decision-makers by transforming raw imagery into actionable insights.

**Approach**  
- LLM-based routing agent selecting appropriate EO analysis  
- Metrics: NDVI, LST, dNBR  
- Integration with OpenStreetMap context  
- Second-pass LLM to generate operational narratives  

**Technologies**  
Ministral-3B, LangChain, Rasterio, Gradio, Hugging Face  

**Results**  
- Public demo available  
- Clear outputs combining visuals, metrics, and explanations  
- Reusable architecture for EO workflows  

**What I learned**  
- LLM orchestration and prompt design  
- Human-centered interfaces for technical data  
- Bridging AI outputs with non-expert usability  

---

### Document AI — AI Integration in Production Software

**Context**: Internal R&D (Diginove)  

**Problem**  
Modernizing a document management system with AI capabilities beyond traditional deterministic methods.

**Approach**  
- Integration of deep learning into existing pipelines  
- Collaboration with developers and customers to identify needs  

**Technologies**  
Python, C++, ONNX, TensorRT, BERT, OCR  

**Contributions**  
- Handwritten digit and character recognition  
- OCR integration  
- Named Entity Recognition (BERT-based)  
- Pipeline design, training, benchmarking, and deployment  

**Constraints**  
- CPU-based deployment  
- Integration into legacy systems  

**Results**  
- Features deployed and used in production  
- Example: extraction of structured information from forms (health records)  

**What I learned**  
- Integrating AI into existing industrial systems  
- Designing under deployment constraints  
- Working closely with real users and business needs  

---

### Medical VLM Exploration — Multimodal AI for Healthcare

**Context**: Personal project  

**Problem**  
Understanding how vision-language models can be applied to medical imaging.

**Approach**  
- Literature review on VLMs and medical AI  
- Reproduction of CT-CLIP model (chest CT modality)  
- Exploration of inference constraints and deployment implications  

**What I learned**  
- Multimodal architectures and self-supervised learning  
- Practical constraints in medical AI systems  
- Importance of interpretability and bias awareness  

---

### Robotics Automation — Industrial Internship (Bioderma)

**Context**: 4-month internship  

**Problem**  
Ensure traceability and synchronization across production and palletizing systems.

**Approach**  
- Monitoring product flow across the production line  
- Communication between PLCs via OPC server  
- Python-based supervision tools  

**Results**  
- Automated synchronization between systems  
- Reduced manual intervention  
- Saved several dozen minutes per day  

**What I learned**  
- Industrial constraints and reliability  
- Real-time system monitoring  
- Automation and system integration  

---

### ITER Robot Competition — Cooperative Robotics

**Context**: Student competition  

**Problem**  
Design a robot to collect and sort simulated nuclear waste.

**Approach**  
- State-machine (Grafcet-style) control logic  
- Sensor-driven navigation and manipulation  

**Technologies**  
Raspberry Pi, sensors, DC motors  

**Contributions**  
- Electrical design  
- Full control algorithm implementation  

**Results**  
- Team won the competition  

**What I learned**  
- Team collaboration  
- Robustness in robotics systems  

---

## /research

- Paper submitted to ICASSP 2025  
- Experience writing scientific papers and reports  
- Collaboration with researchers, professors, and domain experts  
- Daily use of rigorous experimental methodology  

---

## /evidence

- GitHub repositories (Attention-NMF, Agent4EO, CT-CLIP exploration)  
- Live demo (Agent4EO)  
- Research paper (Attention-NMF)  
- Conference poster (AI4EO 2025, not public)  
- Recommendation letters (research and industry)  

---

## /personal_traits

- People who work with me would say I am reliable and easy to collaborate with. I enjoy helping others, sharing knowledge, and I can be counted on to deliver while communicating clearly about constraints.  
- I approach problems by understanding them deeply before acting.  
- What distinguishes me is my curiosity and my willingness to explore new domains and methods to find the right solution.  

---

## /what_i_am_looking_for

I am looking for roles such as:
- AI / ML Engineer  
- Research Engineer  
- Applied Scientist  
- Image Processing Engineer  

I am particularly interested in:
- scientific AI  
- medical imaging  
- robotics AI  
- multimodal and foundation models  

I am drawn to environments such as:
- deep tech startups  
- research labs  
- climate tech  
- healthcare and tech-for-good applications  

---

## /short_bio

AI Research Engineer specializing in computer vision and scientific data, with experience in Earth Observation, document AI, and research-driven model design. I build end-to-end solutions from data understanding to deployment, with a strong focus on rigor and real-world impact.

---

## /long_bio

I am an AI Research Engineer with a background in image processing and scientific data analysis. My work focuses on extracting meaningful information from complex, high-dimensional data such as satellite imagery, documents, and medical images.

I have experience both in research environments and applied industrial settings, where I design models, build pipelines, and ensure their usability in real-world contexts. I am particularly interested in problems that require combining theoretical understanding, data analysis, and practical constraints.

I enjoy working at the intersection of disciplines, where solving a problem requires not only choosing the right model, but also understanding the data, the domain, and the end user.
