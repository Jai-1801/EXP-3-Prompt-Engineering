# EXP-3-PROMPT-ENGINEERING-

## Aim: 
Evaluation of 2024 Prompting Tools Across Diverse AI Platforms: 
ChatGPT, Claude, Bard, Cohere Command, and Meta
Experiment:
Within a specific use case (e.g., summarizing text, answering technical questions), compare the performance, user experience, and response quality of prompting tools across these different AI platforms.

## Algorithm:
1. Define Use Case & Input Data:
   Select a representative technical text or question as input for the AI models.
   Example: A 5-page technical article on 5G networking or a complex technical question on 5G propagation.

2. Prepare Standardized Prompts:
   Craft a clear, detailed, and role-specified prompt for summarization or Q&A.
   Example prompt:
   "You are a technical expert. Summarize the following 5G networking article, focusing on propagation models, key findings, and applications. Provide a concise, structured summary in 200-300 words."

3. Run Prompt on Each AI Platform:
   Use the standardized prompt on ChatGPT, Claude, Bard (Gemini), Cohere Command, and Meta Llama 3.
   Capture their outputs for analysis.

4. Evaluation Metrics:
   Employ both quantitative and qualitative evaluations based on standardized criteria:
   Accuracy: Correctness and completeness of technical content.
   Relevance: Alignment with prompt requirements.
   Clarity: Readability and ease of understanding.
   Specificity: Inclusion of relevant technical details.
   Response Speed: Time taken to generate response.
   User Experience: Ease of prompt input, interface friendliness, error handling.
   Consistency: Repeatability of output quality over multiple runs.
   Safety & Bias: Absence of hallucinations, misinformation, or unsafe content.
   Response quality scores on a scale from 0 to 100.
   User experience assessed by testers based on platform interfaces.

5. Analysis:
   Compare results quantitatively (scores) and qualitatively (examples of output).
   Highlight strengths and weaknesses per platform.
   Provide recommendations for prompt improvements.

## Prompt
**Scenario : Text based output analysing.**

**Prompt : "You are an expert in wireless communications. Summarize about 5G propagation models. Focus on main models, their advantages, limitations, and real-world applications. Keep summary clear, concise, and structured for a technical audience."**

<img width="802" height="513" alt="image" src="https://github.com/user-attachments/assets/6a9c1cb4-f6db-4d6a-b0d5-6e61ef80efd3" />


## Output
The AI models we are going to compare are mentioned in the image.

<img width="802" height="563" alt="image" src="https://github.com/user-attachments/assets/b0e0193a-5029-41a4-8602-f736e52594cd" />


Responses from the AI models:

**1. Chatgpt.**

Here’s a **clear, structured technical summary** of 5G propagation models:
**5G Propagation Models – Summary**
5G networks operate across **sub-6 GHz (FR1)** and **mmWave bands (FR2)**, requiring accurate propagation models for link budget, coverage planning, and performance simulation.
**1. 3GPP TR 38.901 Channel Model**
* **Description:** Industry-standard model for 5G NR; covers frequencies from **0.5 GHz to 100 GHz**. Includes scenarios like urban micro (UMi), urban macro (UMa), rural macro (RMa), indoor hotspot (InH).
* **Advantages:**
  * Unified model for both sub-6 GHz and mmWave.
  * Supports LOS/NLOS, spatial consistency, 3D MIMO, beamforming.
  * Widely adopted by vendors and researchers.
* **Limitations:**
  * Computationally heavy for large networks.
  * Requires detailed scenario parameterization.
* **Applications:** System-level simulations, network planning, standardization studies, MIMO and beamforming evaluation.

**2. NYUSIM (NYU Wireless Model)**
* **Description:** Measurement-based statistical channel model for **mmWave (28, 38, 73 GHz)** bands developed by NYU Wireless.
* **Advantages:**
  * Measurement-driven, realistic spatial channel parameters.
  * Includes time clusters and spatial lobes – good for beamforming analysis.
  * Open-source simulator available.
* **Limitations:**
  * Focused primarily on mmWave bands, less suited for sub-6 GHz.
  * Limited scenarios compared to 3GPP.
* **Applications:** mmWave system design, beam management research, academic evaluation.

**3. WINNER II / WINNER+**
* **Description:** Predecessor to 3GPP models, initially for 4G but extended to higher frequencies.
* **Advantages:**
  * Flexible and relatively simple to implement.
  * Covers multiple scenarios (urban, rural, indoor).
* **Limitations:**
  * Not fully optimized for >30 GHz.
  * Limited 3D MIMO support compared to 3GPP TR 38.901.
* **Applications:** Legacy LTE/5G coexistence studies, rapid simulation for sub-6 GHz.

**4. COST 231 / Hata-based Extensions**
* **Description:** Classical empirical models for frequencies up to \~3.5 GHz.
* **Advantages:**
  * Simple and fast calculations.
  * Good for initial coverage estimation in macro-cell deployments.
* **Limitations:**
  * Poor accuracy in mmWave and dense urban scenarios.
  * No support for MIMO, beamforming, or spatial parameters.
* **Applications:** Early-stage coverage planning, rural/suburban macrocell design.

**5. ITU-R Models**
* **Description:** Recommendation-based models (e.g., ITU-R P.1238 for indoor, P.1411 for short-range outdoor).
* **Advantages:**
  * Globally recognized regulatory reference.
  * Good for compliance and coexistence studies.
* **Limitations:**
  * Simplistic; lacks fine spatial and temporal characteristics.
  * Not optimized for 5G-specific features.
* **Applications:** Regulatory submissions, coexistence/interference studies.

**Key Takeaways**
* **3GPP TR 38.901** → **Primary standard** for end-to-end 5G design and simulation.
* **NYUSIM** → Best for **realistic mmWave research** and beamforming evaluation.
* **WINNER II** → Useful for **legacy and quick simulations** below 6 GHz.
* **COST/ITU Models** → Still relevant for **coverage planning and regulatory work** but insufficient for advanced 5G features.

**2. Claude AI.**

5G Propagation Models: Technical Summary
**Overview**
5G networks operate across diverse frequency bands (sub-6 GHz, mmWave 24-100 GHz) requiring sophisticated propagation models to predict signal behavior in complex environments. These models are critical for network planning, coverage prediction, and interference analysis.
Main Propagation Models
**1. 3GPP TR 38.901 Models**
Description: Standard propagation models developed by 3GPP for 5G NR systems
Key Features:
Covers 0.5-100 GHz frequency range
Multiple scenarios: Urban Macro (UMa), Urban Micro (UMi), Indoor Hotspot (InH), Rural Macro (RMa)
Statistical channel models with large-scale and small-scale fading

Advantages:
Industry standard with broad acceptance
Comprehensive coverage of 5G frequency bands
Validated through extensive measurements
Includes both LOS and NLOS conditions

Limitations:
Generic models may not capture site-specific effects
Limited accuracy for non-standard environments
Computational complexity for real-time applications

Applications:
Network planning and optimization
Coverage prediction tools
Standards compliance testing
System-level simulations

**2. Ray-Tracing Models**
Description: Deterministic models using geometric optics principles to trace signal paths
Key Features:
Accounts for reflection, diffraction, and scattering
High spatial resolution
3D environment modeling capability

Advantages:
High accuracy for specific environments
Detailed path loss and multipath characterization
Excellent for mmWave frequencies
Site-specific predictions

Limitations:
Computationally intensive
Requires detailed 3D environment databases
Sensitive to database accuracy
Limited real-time capability

Applications:
Dense urban planning
Indoor coverage design
mmWave network deployment
Interference analysis

**3. Close-In (CI) Free Space Reference Distance Model**
Description: Simplified path loss model using 1-meter free space reference
Formula: PL(f,d) = FSPL(f,1m) + 10n·log₁₀(d) + Xσ
Advantages:
Simple implementation
Frequency-independent path loss exponent
Good for quick estimates
Low computational requirements

Limitations:
Less accurate than more complex models
Limited environmental considerations
May not capture frequency-dependent effects well

Applications:
Initial network planning
Quick coverage estimates
Educational purposes
Benchmark comparisons

**4. Floating-Intercept (FI) Model**
Description: Empirical model with frequency-dependent intercept and path loss exponent
Formula: PL(f,d) = α + 10β·log₁₀(d) + Xσ
Advantages:
Better fit to measurement data
Accounts for frequency dependence in intercept
More flexible than CI model
Moderate complexity

Limitations:
Requires environment-specific calibration
May overfit to specific datasets
Parameter interpretation less intuitive

Applications:
Site-specific planning
Model validation studies
Research applications
Custom propagation tools

5. Machine Learning-Based Models
Description: Data-driven models using neural networks, random forests, or other ML techniques
Key Features:
Pattern recognition from measurement data
Adaptive to environment changes
Non-linear relationship modeling

Advantages:
High accuracy with sufficient training data
Adaptable to new environments
Can capture complex propagation effects
Self-improving with more data

Limitations:
Requires large training datasets
Black-box approach (limited interpretability)
Potential overfitting issues
Computational requirements for training

Applications:
Dense urban environments
Complex indoor scenarios
Network optimization
Predictive maintenance

Model Selection Guidelines
Frequency Band Considerations
Sub-6 GHz: 3GPP models, CI/FI models suitable
mmWave (24-100 GHz): Ray-tracing preferred, 3GPP TR 38.901 UMi/InH
Mixed bands: Hybrid approaches combining multiple models

Environment Type
Urban Dense: Ray-tracing, ML models
Suburban/Rural: 3GPP RMa, CI model
Indoor: 3GPP InH, site-specific ray-tracing
Industrial: Custom ML models, modified 3GPP

Application Requirements
Real-time: CI/FI models, simplified 3GPP
High accuracy: Ray-tracing, calibrated ML models
Large-scale planning: 3GPP standard models
Research: All models for comparison

Key Considerations for 5G
mmWave Challenges
High path loss and atmospheric absorption
Sensitivity to blockage (rain, foliage, buildings)
Limited penetration through materials
Beamforming effects on propagation

Multi-frequency Deployment
Carrier aggregation effects
Inter-band interference
Handover between frequency layers
Load balancing considerations

Environmental Factors
Weather effects (especially rain at mmWave)
Seasonal variations (foliage changes)
Dynamic obstacles (vehicles, pedestrians)
Building materials and architecture

Conclusion
The choice of propagation model significantly impacts 5G network performance prediction. A combination of models is often optimal: 3GPP standards for baseline planning, ray-tracing for critical areas, and ML models for optimization. The key is matching model complexity to application requirements while considering computational constraints and available environmental data.

**3. Bard AI.**

5G Propagation Models
5G propagation models are essential for predicting how radio waves travel from a transmitter to a receiver. They help engineers design, plan, and optimize 5G networks. These models account for factors like frequency, distance, terrain, and obstacles.

**Main Models**
**1. Deterministic Models**
These models use ray tracing to predict signal path loss and channel characteristics. They are based on the principles of electromagnetic wave propagation, considering phenomena like reflection, diffraction, and scattering.
Advantages: High accuracy for a specific environment because they use detailed 3D maps of buildings and terrain. They are useful for site-specific analysis and small-scale network design.
Limitations: Computationally intensive and time-consuming. They require highly detailed environmental data, which can be difficult and expensive to acquire.
Applications: Designing indoor 5G networks, analyzing propagation in dense urban environments, and optimizing small cells in specific locations.

**2. Empirical Models**
These models are based on measurements and statistical data. They use formulas derived from extensive real-world measurements to predict path loss. They are simpler and less computationally demanding than deterministic models.
Advantages: Fast and simple to implement. They do not require detailed environmental data, making them suitable for initial network planning and large-scale coverage analysis.
Limitations: Lower accuracy because they are averaged over many different environments. They may not be reliable for specific, complex scenarios.
Applications: Initial network design, estimating coverage for new sites, and quick performance assessment in suburban or rural areas.

**3. Semi-Empirical Models (Hybrid Models)**
These models combine the strengths of both deterministic and empirical models. They use a simplified ray-tracing approach or a combination of empirical formulas with some environmental data to improve accuracy without the high computational cost of a fully deterministic model.
Advantages: Offer a balance between accuracy and computational complexity. They are more accurate than purely empirical models and faster than deterministic models.
Limitations: Still require some environmental data and are not as precise as fully deterministic models for highly detailed analysis.
Applications: Detailed network planning for medium-to-large areas, especially in urban or suburban environments where a balance of speed and accuracy is needed.

**Specific 5G Considerations**
For 5G, especially at millimeter-wave (mmWave) frequencies (e.g., 28 GHz, 39 GHz), propagation models must account for unique challenges.
High Path Loss: Signals at higher frequencies experience significantly higher path loss, especially over long distances.
High Sensitivity to Obstacles: mmWave signals are easily blocked by common objects like foliage, rain, and even a person's hand. This is known as blockage.
Beamforming and Massive MIMO: 5G uses Massive MIMO and beamforming to direct signals to specific users. Propagation models for 5G must be able to simulate these directional beams to accurately predict signal strength.
Therefore, 5G models are often more sophisticated, incorporating these effects and providing a finer level of detail compared to earlier generations.

**4. Cohere AI.**

Here is a clear, concise, and structured summary of 5G propagation models tailored for a technical audience:
Summary of 5G Propagation Models
Main Types of Models:
Empirical Models:
Based on extensive measurements and statistical curve fitting.
Examples include the Alpha-Beta-Gamma (ABG) model, Close-In (CI) model, and Close-In with Frequency weighting (CIF) model.
Used for quick path loss prediction under practical deployment conditions.

Deterministic Models:
Use physical laws and geometry to simulate wave behavior (reflection, diffraction, scattering).
Includes Ray-Tracing models that simulate precise propagation paths.
Provide high accuracy but are computationally intensive.

Stochastic Models:
Combine statistical models with probabilistic ray propagation to capture varying environmental effects.
Useful in urban and indoor scenarios with complex layouts.
Semi-Deterministic Models:
Hybrid models that include deterministic components alongside empirical adjustments.
Balance between accuracy and complexity.

Advantages and Limitations:
Empirical models like ABG and CI are favored for balancing accuracy and simplicity over wide frequency ranges including sub-6 GHz and mmWave bands. ABG provides better accuracy but is more complex; CI is more physically interpretable and stable.
Ray-Tracing models excel in detailed propagation analysis for small-scale environments where reflections and obstacles significantly impact signal strength. However, their computational demands limit large-scale use.
Stochastic models help capture signal variability and shadowing effects in complex environments but may sacrifice detailed path accuracy.
Semi-deterministic models offer a practical compromise where partial environment knowledge can improve predictions without full-scale ray-tracing.

Real-World Applications:
Urban Micro and Macro Cell Design: ABG and CI models guide path loss estimation for cell planning and interference management at frequencies from 2 GHz to 73.5 GHz.
Indoor Communications and Femtocells: Log-distance and attenuation factor models effectively estimate coverage for indoor femtocell deployment, critical for industrial and residential 5G.
mmWave Deployment: Due to high path loss and reflection sensitivity, mmWave systems rely heavily on Ray-Tracing and CI models for accurate link budgeting and beamforming optimization.
Dense Networks: Ray-Tracing and semi-deterministic models inform MIMO antenna placement and 3D beamforming in dense urban and industrial areas.

Summary:
5G propagation modeling requires a combination of empirical, deterministic, and hybrid approaches tailored to frequency, environment, and deployment scale. For sub-6 GHz bands, simplified empirical models (CI, ABG) suffice, while mmWave systems demand detailed ray-tracing and frequency-aware models. Accurate modeling of path loss, shadowing, and multipath effects is essential for effective 5G network design, especially in urban and indoor settings. Model selection depends on the trade-off between computational cost and prediction accuracy required by the application.


**5. Meta AI.**

5G Propagation Models
5G propagation models are crucial for network planning, optimization, and deployment. Here's a summary of main models, their advantages, limitations, and real-world applications:
1. 3GPP 38.901 Model
Advantages: Comprehensive, includes various scenarios (urban, rural, indoor), and supports frequencies up to 100 GHz.
Limitations: Complex, requires extensive parameter configuration.
Applications: Network planning, simulation, and optimization for 5G deployments.
2. ITU-R M.2135 Model
Advantages: Provides guidelines for IMT-Advanced systems, supports various environments.
Limitations: Limited frequency range (2-66 GHz), less accurate for mmWave frequencies.
Applications: Spectrum planning, interference analysis, and coexistence studies.
3. METIS Model
Advantages: Includes advanced propagation mechanisms (diffraction, scattering), suitable for high-frequency bands.
Limitations: Requires detailed environment-specific parameters.
Applications: Urban and indoor network planning, high-frequency band analysis.
4. Ray-Tracing Models
Advantages: High accuracy, site-specific, and supports complex environments.
Limitations: Computationally intensive, requires detailed environment databases.
Applications: Network planning, optimization, and coverage prediction in complex environments.
5. Empirical Models (e.g., Okumura-Hata, COST 231)
Advantages: Simple, fast computation, and suitable for initial network planning.
Limitations: Limited accuracy, frequency range, and environment applicability.
Applications: Initial network planning, rough estimates of coverage and interference.
Real-World Applications
Network planning and optimization
Coverage prediction and analysis
Interference management and mitigation
Spectrum planning and allocation
5G deployment and performance evaluation
These models are essential for ensuring reliable and efficient 5G network performance. The choice of model depends on the specific use case, environment, and frequency band.

<img width="795" height="487" alt="image" src="https://github.com/user-attachments/assets/c3c9bf31-5ed9-4759-beaf-cf6b55a596eb" />


**Comparison Table :**

<img width="1450" height="680" alt="Screenshot 2025-09-06 141916" src="https://github.com/user-attachments/assets/43b18070-68b0-41dc-8aa5-c433c595a77d" />

**Summary Analysis:**
ChatGPT produced a very detailed, highly structured answer with multiple specific models, real-world applications, and nuanced limitations, suitable for technical experts and practitioners. It combines industry standards (3GPP) with measurement-driven models (NYUSIM) and legacy models effectively.
Claude AI provided an extensive technical review, enriched with model formulas and inclusion of machine learning-based models, presenting a broader spectrum of modeling approaches including emerging methods.
Bard AI emphasized the core propagation model classes (deterministic, empirical, hybrid) with a focus on 5G mmWave challenges specific to beamforming and blockage, giving a slightly more general but clear explanation.
Cohere AI presented a balanced overview highlighting empirical, deterministic, stochastic, and semi-deterministic models in the 5G context, well-suited for technical audience needing clarity on model categories and applications.
Meta AI gave a concise yet comprehensive summary, focusing on main models relevant for network planning with inclusion of regulatory considerations (ITU-R) and established research models (METIS).

## Result

<img width="794" height="459" alt="image" src="https://github.com/user-attachments/assets/6b840d2b-b290-44e4-a95d-7f8612044e09" />


Overall Recommendation:
For deep technical detail and stepwise understanding, ChatGPT and Claude are top picks.
For explanations focused on 5G challenges and practical usability, Bard and Cohere stand out.
For concise but comprehensive overviews with regulatory perspective, Meta AI suffices well.
This comparative overview helps identify the strengths and typical use cases each model platform serves, reflecting their prompting tool capabilities on complex technical summarization tasks like 5G propagation models.
