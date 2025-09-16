# Project Ideation (Version 0.9)

## 1. Background & Motivation
- As artificial intelligence (AI) workloads have increased recently, the need for resource management and efficiency in cloud/edge/on-device environments has grown.
- Our team is exploring research topics centered on [AI/Operating Systems/Resource Management/Computer Architecture] fields.
---

## 2. Brainstormed Ideas
1. **RISC-V-based On-device AI Lightweight System (Main Candidate)**
  - Custom AI-friendly architecture design using open-source ISA (RISC-V)
  - Achieving performance-power balance in on-device environments
  - Low-level optimization research for efficient execution of lightweight AI models

    
2. **Heterogeneous Resource Operating System Design and Orchestration Techniques for AI Workloads (Main Candidate)**
  - Management of heterogeneous resources including GPU/NPU/CPU/FPGA
  - Kernel-level optimization of scheduling and memory management
  - Performance-power efficiency → AI-friendly operating system direction


3. **Disaggregated Datacenter OS Design and Dynamic Resource Management Techniques (Main Candidate)**
  - Disaggregation of CPU/memory/GPU/storage (Disaggregated Datacenter, DDC)
  - Dynamic allocation and reclamation of resources as needed
  - Research on network latency issues and resource scheduling policies


4. **GPU Workload-based Resource Management and Scheduling Optimization (Reserve Candidate)**
  - Operating system-level resource management research reflecting GPU-centric AI workload characteristics
  - Dynamic scheduling policy design to maximize GPU utilization
  - Optimization techniques considering both performance and power efficiency
  - Goal to mitigate GPU resource bottlenecks during large-scale AI model execution


5. **GPU Memory State-based Real-time LLM Layer Repartitioning Adaptive System (Reserve Candidate)**
  - Real-time relocation/repartitioning of LLM (Large Language Model) layers based on GPU memory occupancy
  - Stable large-scale model inference even in memory shortage situations
  - Maintaining performance-resource balance through adaptive resource management techniques
  - Maximizing GPU memory utilization and improving LLM inference efficiency


6. **[EdgeAI] Neural Network Partitioning for Multi-Access Edge Computing (Dynamically partitioning neural networks based on network latency and device performance for optimal cloud-edge placement)**


7. **[Optimization] System for dynamic resource reallocation based on real-time load when multiple inference tasks share GPU**


8. **[AI(Model Training), System Optimization] Development of 'Anomaly Detection System' using self-generated training data and lightweight AI models**


9. **[AI, OS] AI-based Operating System Anomaly Detection and Autonomous Tuning**


10. **[AI/Optimization/Distributed Scheduling] Research on serverless scheduling techniques specialized for AI inference workloads (or serverless computing optimization research)**
---

## 3. Next Steps
- Finalize main topic through team voting/discussion and professor's advice
- Analyze pros/cons and required resources for each idea
---

## 4. Feedback on the Topics (Version 0.9)
### 1. AI Model Lightweight
- A field where much research has already been conducted → Difficult to secure originality.
- Easy for undergraduates to attempt, but challenging to develop into a good thesis topic.


### 2. OS Design Encompassing GPU/NPU
- The topic is overly broad, and implementation at undergraduate level is virtually impossible.
- Difficult to receive good evaluation in graduation project assessment.


### 3. Disaggregated Datacenter OS Design
- While it's an attracting field, it's not suitable for undergraduates.
- Implementation is difficult, and it's hard to demonstrate results through experiments.


### 4. GPU Memory State-based LLM Layer Repartitioning
- The topic description itself is specific and interesting.
- However, it's unclear how to specifically implement and experiment.


### 5. GPU Workload Resource Management and Scheduling
- Fundamentally an appropriate topic.
- However, since it's a field with much existing research, something is needed to secure originality.

**Refined Direction**  
- Collect CPU/GPU/memory/network resource usage patterns during various AI model training.  
- Design resource usage prediction models based on this data.  
- Consider not only performance metrics but also **energy metrics**.  

**Feedback**  
- Resource usage prediction already has extensive research.  
- Instead, focusing research on **energy consumption prediction** would be more original and strategically appropriate.  
- Sufficiently feasible as an undergraduate graduation project topic, and competitive in papers and final evaluations.

---

### Additional Suggestions
- Cloud servers run multiple VMs executing AI workloads simultaneously.  
- Energy consumption of AI workloads is increasing explosively.  
- Therefore, the most important problem is **how to estimate energy consumption for each VM**.  

**Current Status**  
- CPU/GPU-level energy prediction technologies exist but have low accuracy.  
- Research on accurately dividing individual VM energy from total system power consumption is insufficient.  

**Proposed Idea**  
- Design a model to **predict VM-level energy consumption** based on total system power consumption data.  
- Utilize power measurement equipment → Enable comparison and verification between model predictions and actual measurements.  

**Expansion Possibilities**  
- Beyond simple scheduling, expand to **resource planning/allocation research**.  
  - Example: Reducing performance slightly to save energy.  
  - Or minimizing energy increase while guaranteeing certain performance.