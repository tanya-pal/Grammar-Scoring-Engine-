Grammar Scoring Engine (Speech-Based)
A machine learning-based system that evaluates the grammatical quality of spoken language samples. Trained on audio recordings rated with MOS Likert grammar scores (0 to 5), the model predicts grammar proficiency using speech features.

📌 Project Highlights
 Goal: Predict grammar scores from spoken language samples.

 Input: Audio files (speech recordings).
 Output: Grammar score (0–5 scale).

Evaluation Metric: Pearson Correlation Coefficient.
 Model Used: RandomForestRegressor (with experimentation for improvements).
 Features Extracted: MFCCs (Mel-Frequency Cepstral Coefficients).

 🔬 Methodology
✅ Preprocessing
Normalized audio

Converted stereo to mono

Trimmed silence

Extracted MFCC features (13 coefficients + mean & std)

Model
RandomForestRegressor

Tuned hyperparameters with cross-validation

Optional: Feature scaling, model ensembling (for further improvement)

📏 Evaluation
Pearson Correlation used to measure alignment between predicted and actual grammar scores.

📈 Results
Model	Pearson Correlation
Random Forest (Base)	0.78
Tuned Random Forest	0.83
Note: You can improve performance further with ensemble models or neural nets

Technologies Used:
Python 
Librosa 
Scikit-learn 
Pandas & NumPy 
Jupyter Notebook 

Author:
Tanya Pal
B.Tech CSE (Data Science) | ML & AI Enthusiast

