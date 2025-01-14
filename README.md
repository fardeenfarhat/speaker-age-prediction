# Speaker Age Prediction Model

## Introduction
This project focuses on predicting speakers' ages from audio recordings using advanced signal processing and machine learning techniques. By extracting acoustic features such as pitch, formant frequencies, intensity, duration, and spectral characteristics, we aim to develop a robust regression model capable of estimating speaker age. The results have applications in voice-based personalization, targeted advertising, and forensic analysis.

---

## Features Extracted
Key acoustic features derived from the speech signals include:
1. **Pitch**: Perceived tone or frequency of the voice.
2. **Formant Frequencies**: Resonant frequencies of the vocal tract.
3. **Intensity**: Energy or loudness of the voice.
4. **Duration**: Length of speech segments.
5. **Spectral Features**: Frequency content derived from Fourier transform or spectrograms.

These features are crucial for capturing the variations in vocal characteristics associated with age.

---

## Data Preprocessing
Due to the size of the original dataset, it is not included in the repository. However, the extracted features are stored in a CSV file, which is provided for convenience. This CSV file contains all the necessary data to train and evaluate the model.

To handle missing data, four datasets were created using the following techniques:
1. **Dataset 1**: Rows with missing values were removed.
2. **Dataset 2**: Missing values were imputed with the mean.
3. **Dataset 3**: Missing values were imputed with the mode.
4. **Dataset 4**: Missing values were imputed with the median.

Additionally, all features were normalized and scaled to ensure uniformity, improving the performance and convergence of machine learning algorithms.

--- 

## Model Training
A regression-based approach was adopted for this task:
1. **Algorithm Selection**: 
   - Linear Regression
2. **Training**: The model was trained on the preprocessed datasets, utilizing extracted features as inputs and speaker ages as target variables.

The choice of the regression model depends on dataset complexity, size, and the desired interpretability.

---

## Model Evaluation
The trained model was evaluated using:
- **Mean Squared Error (MSE)**
- **Mean Absolute Error (MAE)**

---

### Performance Assessment
Evaluation focused on the model's ability to predict ages across different groups, emphasizing metrics that reflect predictive accuracy and model generalizability.

---

## Results
- Insights into how different preprocessing strategies affected model performance.
- Impact of acoustic features on speaker age prediction.

---

## Applications
- **Voice Personalization**: Tailoring user experiences based on predicted age.
- **Forensics**: Age estimation for legal and investigative purposes.
- **Targeted Advertising**: Age-specific content delivery.

---

## Technology Stack
- **Programming Language**: Python
- **Core Libraries**:
  - `numpy` for numerical operations.
  - `pandas` for data handling.
  - `scikit-learn` for machine learning.
  - `matplotlib` for visualizations.

---

## How to Run the Code
1. Clone the repository:
   ```bash
   git clone https://github.com/fardeenfarhat/speaker-age-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd speaker-age-prediction
   ```
3. Enjoy the code

---

## Example
### Input:
  - **CSV File**: Contains acoustic features such as pitch, formants, and spectral characteristics.

### Output:
  - **Predictions**: Age estimates for speakers based on audio features.
  - **Metrics**: MSE, MAE, and R² values indicating model performance.

---

## Contributing
1. Fork the repository.
2. Create a new branch for your feature or bugfix:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Submit a pull request.

---

## License
This project is licensed under the [MIT License](LICENSE).

---

## Contact
- **Author**: Fardeen Farhat
- **Email**: fardeenfarhat@gmail.com
- **GitHub**: [fardeenfarhat](https://github.com/fardeenfarhat)

