---
layout: home
title: Phong Le's Website
---

<div style="display: flex; align-items: center; gap: 24px; margin-top: 1.5rem;">
  <img
    src="/assets/images/background_headshot.png"
    alt="Phong Le headshot"
    style="
      width: 150px !important;
      height: 150px !important;
      border-radius: 9999px;
      object-fit: cover;
      display: block;
      flex: 0 0 600px;
    "
  >
  <div style="max-width: 700px;">
    <p>
      Welcome to my personal portfolio! I’m Phong Le, a Biomedical Engineering
      and Computer Science student at Duke University. This site showcases my
      professional journey, skills, and projects. It’s structured like my
      resume for easy navigation, but dives deeper into my work with detailed
      project descriptions.
    </p>
  </div>
</div>


## About Me
I'm a dual-degree candidate pursuing a B.S.E. in Biomedical Engineering and a B.A. in Computer Science at Duke University, with an anticipated graduation in May 2026. My work focuses on the intersection of machine learning, bioinstrumentation, computational drug discovery, and health tech. I'm passionate about leveraging technology for accessible healthcare solutions, from low-cost medical devices to scalable AI for antibiotic screening. Honors include being a Duke QuestBridge Scholar, Florence Family Scholarship Recipient, and Post Grata Award Recipient. In my free time, I enjoy exploring open-source contributions and hardware tinkering.

## Education
- **B.S.E. Biomedical Engineering | B.A. Computer Science** - Duke University, Durham, NC  
  Anticipated Graduation: May 2026  
  Description: Focused on interdisciplinary coursework blending engineering, computer science, and data-driven biology. Key courses include Machine Learning & Imaging, Diagnostic Imaging, Bioinstrumentation, Signals & Systems, and Algorithms in Data Science. Emphasized hands-on projects in ML for healthcare and biosensor modeling.  
  Honors/Awards: Duke QuestBridge Scholar, Florence Family Scholarship Recipient, Post Grata Award Recipient.  
  Links/Files: [LinkedIn Profile](https://www.linkedin.com/in/phong-h-le/) | [Resume PDF (v2.1c)](assets/Resume-SP26-v2.1c.pdf) | [Resume PDF (v2.1b)](assets/Resume-SP26-v2.1b.pdf)

## Professional Experience and Projects
This section combines my experiences and projects, mirroring my resume structure. I've expanded on each with in-depth details based on my involvement, including technical challenges, methodologies, and outcomes.

- **Scalable Machine Learning for Antibiotic Virtual Screening** - Computational Drug Discovery Project, Durham, NC  
  Dates: Aug - December 2025  
  Description: Benchmarked GNEprop (from Nature Biotechnology, 2025) against Chemprop and XGBoost on a dataset of 2,560 antibiotic candidates. Achieved a ROC-AUC of 0.936 through structured batch training and evaluation. Implemented robust ML validation controls like scaffold-based splits and adversarial y-shuffling to detect and prevent data leakage. Quantified trade-offs between model accuracy and computational efficiency to optimize for large-scale screening pipelines. This project addressed the challenge of high-throughput virtual screening in drug discovery, reducing false positives and enabling faster iteration in antibiotic development.  
  Tech Stack: Python, PyTorch, Scikit-Learn, RDKit, Pandas.  
  Challenges & Solutions: Handled large datasets with batch processing; mitigated overfitting via cross-validation techniques.  
  Outcomes: Demonstrated scalable ML for resource-constrained environments; potential for integration into pharmaceutical workflows.

- **Arts North Carolina** - Data Analyst & Policy Advocate, Durham, NC  
  Dates: Jan - May 2025  
  Description: Collaborated with the Arts NC director and NC Department of Public Instruction to lobby for arts education Bill H418. Executed regulatory-compliant data harmonization across 4 state and federal education datasets, involving schema normalization, missing identifier resolution, and adherence to government privacy laws (e.g., FERPA). Applied machine learning to uncover disparities in academic performance correlated with arts education access. Produced a legislative brief that was presented to over 150 legislators during Arts Day NC, influencing policy discussions on equitable education.  
  Tech Stack: Python, Pandas, Scikit-Learn, SQL for data processing.  
  Challenges & Solutions: Ensured data privacy by anonymizing sensitive fields; used clustering algorithms to identify performance gaps.  
  Outcomes: Contributed to advocacy efforts; brief informed statewide policy on arts integration in curricula.

- **Systems Modeling of Gene-Circuit Biosensors** - Gene Circuits Project, Durham, NC  
  Dates: Aug - December 2025  
  Description: Developed ODE-based biosensor models in Python to infer toxin concentrations from bioluminescent whole-cell data. Applied nonlinear optimization and bootstrapping techniques to recover analyte concentrations, quantify sensor sensitivity, detection limits, and dynamic range. This work simulated gene-circuit responses for environmental toxin detection, bridging synthetic biology and computational modeling for real-time biosensing applications.  
  Tech Stack: Python, SciPy for ODE solving, Matplotlib for visualization.  
  Challenges & Solutions: Modeled nonlinear dynamics with numerical integration; used bootstrapping for uncertainty quantification.  
  Outcomes: Enhanced understanding of biosensor performance; models applicable to synthetic biology designs.

- **Electromyography (EMG) Circuit** - Bioinstrumentation Project, Durham, NC  
  Dates: Aug - Dec 2024  
  Description: Designed an analog EMG front-end using instrumentation amplifiers and bandpass filtering for muscle signal acquisition. Optimized gain staging and noise rejection to isolate bicep and tricep activations, enabling downstream signal processing for prosthetic control or rehab tech. Tested for signal fidelity in low-noise environments.  
  Tech Stack: Analog hardware (amplifiers, filters), MATLAB/Python for analysis, oscilloscopes.  
  Challenges & Solutions: Reduced noise with shielding and filtering; calibrated for specific muscle groups.  
  Outcomes: Reliable EMG acquisition prototype; potential for integration into wearable health devices.

- **Analog Hearing Aid for Low-Resource Settings** - Bioinstrumentation Project, Durham, NC  
  Dates: Aug - December 2023  
  Description: Designed and built a low-cost analog hearing aid prototype (under $30 in parts), achieving less than 2% harmonic distortion and up to 55× gain. Engineered a dual-passband filter system to amplify key speech frequencies (500-3000 Hz) while suppressing non-speech noise. Analyzed signal fidelity and gain using MATLAB, Python, and oscilloscope measurements. Validated through user trials with a 4.4/5 speech intelligibility score, compliant with ANSI standards. This project aimed at accessible audiology solutions for underserved communities.  
  Tech Stack: Analog electronics, MATLAB/Python for signal processing, KiCad for design.  
  Challenges & Solutions: Balanced cost and performance; iterated filters for speech clarity.  
  Outcomes: Viable prototype for low-resource deployment; high user satisfaction in trials.

- **Automated Computational Antibiotics Modeling Lab** - Research Project with Dr. Michael Lynch, Durham, NC  
  Dates: Jan - May 2023  
  Description: Built an automated in silico screening pipeline for antibiotic analogues using molecular dynamics simulations. Developed a Python-based workflow integrated with ChimeraX, boosting simulation throughput by ~100×. Applied AlphaFold and RDKit for structure-based and cheminformatics analysis on large-scale datasets, enabling rapid evaluation of drug candidates.  
  Tech Stack: Python, AlphaFold, RDKit, ChimeraX.  
  Challenges & Solutions: Scaled computations with automation; handled big data with efficient parsing.  
  Outcomes: Accelerated antibiotic discovery; pipeline reusable for similar research.

## Leadership and Activities
- **MEDesign** - Co-President, Durham, NC  
  Dates: Jan 2023 - May 2025  
  Description: Led a 30+ member organization focused on medical device and digital health projects. Coordinated mentorship, project planning, and events. Directed the development of an app-linked wearable breathalyzer, handling end-to-end aspects like BLE hardware, mobile app (Flutter), and data transmission. Led a 5-member team to a minimal viable prototype in 4 months.

## Skills
I've categorized my skills for clarity, with proficiency levels and examples.

| Category | Skills | Proficiency | Examples/Tools |
|----------|--------|-------------|----------------|
| Machine Learning | Python, PyTorch, Scikit-Learn, RDKit, Pandas, TensorFlow, Data Processing, Feature Engineering | Advanced | ML for drug screening, adversarial validation |
| Research | Image & Signal Processing, Data Visualization, ODE Modeling, Numerical Simulation, AlphaFold | Advanced | Biosensor modeling, molecular dynamics |
| Embedded & Hardware | PCB Milling, Soldering, Oscilloscopes, BLE (Bluetooth), Arduino, KiCad, 3D Printing | Intermediate | Hearing aid prototype, EMG circuit |
| Software & Tools | Jupyter, GitHub, SQL, Firebase, Flutter, Fusion 360, C/C++, MATLAB | Advanced | Automated pipelines, app development |

## Contact
Feel free to reach out for collaborations, opportunities, or questions!  
- Email: phl6@duke.edu  
- Phone: +1 843-957-2233  
- LinkedIn: [linkedin.com/in/phong-h-le](https://www.linkedin.com/in/phong-h-le/)  
- GitHub: [github.com/yourusername] (Update with your actual GitHub)  
- Location: Murrells Inlet, South Carolina  

Thanks for visiting! This portfolio is hosted on GitHub Pages using the Minima theme and updated as of January 2026.
