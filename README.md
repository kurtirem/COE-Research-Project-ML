# Machine Learning for Crystal Plasticity Parameter Calibration

Author: Youngbin Pyo, Irem Kurt

## Project Overview
Automated calibration of Crystal Plasticity Finite Element Method (CPFEM) parameters using machine learning to replace manual curve-fitting. Integrates nanoindentation data, simulations, and ML to predict:
- Initial resolved shear stress (τ₀)
- Hardening exponent (a)
- Hardening rate (h₀) 
- Critical shear stress (τ_cs)

## Key ML Contributions
- Developed an automated ML pipeline for CPFEM parameter calibration, reducing manual effort and improving reproducibility.
- Trained and evaluated multiple ML models (ANN, LSTM, CNN, Random Forest) to identify the best-performing approach for force-displacement (FD) curve prediction.
- Implemented feature engineering and data preprocessing to enhance model performance, including normalization, outlier removal, and percentile-based feature extraction.
- Achieved high accuracy with Artificial Neural Networks (ANNs), yielding an R² score of up to 0.995 and low RMSE (2.228e-05) for material-specific predictions.
- Designed an iterative optimization workflow to refine parameters and align simulated FD curves with experimental data.

## My Role (ML Lead)
As the primary contributor to the ML component of this project, I was responsible for:
- Designing the ML pipeline: From data preprocessing to model deployment.
- Developing and training ANN models: Achieved state-of-the-art accuracy for CPFEM parameter prediction.
- Iterative optimization: Implemented a feedback loop to refine parameters using percentile-based error metrics.
- Cross-disciplinary collaboration: Worked with material scientists to validate ML outputs against experimental data.

## Model Performance
| Material          | RMSE       | R² Score | Best Model |
|-------------------|------------|----------|------------|
| DP1000            | 1.331e-05  | 0.975    | ANN        |
| QP1200 (Ferrite)  | 3.128e-05  | 0.983    | ANN        |
| QP1200 (Martensite)| 2.228e-05 | 0.995    | ANN        |

## Future Improvements
- Expand datasets: Incorporate more materials and microstructural variants.
- Enhance feature engineering: Add strain-rate sensitivity and unloading slope metrics.
- Deploy lightweight models: Optimize ANNs for real-time industrial applications.

# Acknowledgments
Special acknowledgments to Rongfei Juan for her invaluable support throughout the entire process. Her continuous feedback, guidance, and provision of essential simulation templates have significantly contributed to the success of this project. We extend our sincere gratitude for their collaborative spirit and assistance.

Special thanks to Binh for providing invaluable assistance in resolving the challenges associated with pushing large data files to GitHub.

Gratitude to Professor Junhe Lian for their outstanding efforts in organizing and facilitating the course.
