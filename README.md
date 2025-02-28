<h1> Analyzing Vocal Features for Improved Machine Learning-Based Gender Identification </h1>
<p>
Brad Buckland<br>
Talia Frendl<br>
Triet Huynh<br>
</p>

<h2>Introduction</h2>
<p>
With the increasing reliance on speech recognition technologies in applications such as virtual assistants, security authentication, and accessibility tools, accurately classifying a speaker’s gender based on vocal characteristics has become an important area of research. However, gender classification in speech presents challenges due to natural variations in pitch, tone, and articulation among individuals.
</p>
<p>
This project seeks to address this challenge by analyzing the Vocal Gender Features dataset, which includes a comprehensive set of spectral, pitch, energy, and cepstral features extracted from speech recordings. Spectral features, such as spectral centroid, bandwidth, and contrast, provide insights into the frequency composition of a speaker’s voice, helping to differentiate between male and female speech patterns. Pitch-related features, including mean, minimum, and maximum pitch frequencies, capture variations in fundamental frequency, a key distinguishing factor in vocal gender classification. Energy-based features, such as root mean square (RMS) energy, log energy, and zero-crossing rate, offer information about the loudness and variability of the signal. Additionally, Mel-Frequency Cepstral Coefficients (MFCCs), which are widely used in speech processing, characterize the timbre of a speaker’s voice and play a crucial role in voice identification.
</p>
<p>
The hypothesis of this study posits that a machine learning model trained on these vocal features can effectively classify speaker gender, with particular emphasis on the role of pitch and MFCCs in distinguishing between male and female voices. This hypothesis is grounded in prior research, which has demonstrated that spectral and pitch-based features are especially effective for gender classification tasks. By analyzing the relationship between these features and speaker gender, this project seeks to evaluate the accuracy and reliability of gender classification in speech.
</p>
<h2>Dataset</h2>
<p>
The dataset selected for this project is the Vocal Gender Features dataset, available on Kaggle: https://www.kaggle.com/datasets/murtadhanajim/vocal-gender-features
This dataset contains a collection of extracted audio features from speech recordings, to classify the speaker's gender as either male (1) or female (0).
</p>

<h2>Goal</h2>
<p>
This study seeks to determine which combination of spectral, pitch, energy, and cepstral features is most effective in classifying a speaker's gender using machine learning models. Additionally, it aims to identify which model will perform the best on these features. By employing data preprocessing, feature engineering, and a variety of machine learning algorithms, this study will evaluate the relative importance of these feature groups in gender classification. The findings from this research may contribute to advancements in speech-processing applications by improving the accuracy and reliability of automated gender recognition systems and providing insights into which models are most suitable for this task.
</p>

<h2>Features</h2>
<p>
The dataset includes various spectral, pitch, energy, and cepstral features that characterize the acoustic properties of speech. Spectral features such as spectral centroid, bandwidth, and contrast provide insights into the distribution of frequencies in the signal, which can help differentiate between male and female voices. Pitch-related features, including mean, minimum, and maximum pitch, capture variations in fundamental frequency, a key factor in gender classification. Energy-based features like root mean square (RMS) energy and zero-crossing rate measure the overall loudness and signal variability, while Mel-Frequency Cepstral Coefficients (MFCCs) represent the timbral characteristics of the voice, commonly used in speech recognition tasks.
</p>

<h2>Methods</h2>
<h3>Tools</h3>
<ul>
  <li>Numpy</li>
  <li>Pandas</li>
  <li>Seaborn</li>
  <li>os</li>
  <li>matplotlib.pyplot</li>
  
</ul>
From sklearn, unless otherwise noted:

<ul>
  <li>Models: KNeighborsClassifier, KNeighborsRegressor, LinearRegression, DecisionTreeClassifier, </li>
  <li>Data Preprocessing: StandardScaler, SMOTE (imblearn), RandomOverSampler (imblearn)</li>
  <li>Evaluation: cross_val_score, GridSearchCV, learning_curve, mean_squared_error, accuracy_score, r2_score, confusion_matrix, classification_report</li>
  <li>Other: train_test_split</li>
</ul>

<h3>APIs</h3>
<ul>
  <li>KaggleHub</li>
</ul>

<h2>Results</h2>
<p>
The goal of this study was to determine whether machine learning models trained on spectral, pitch, energy, and cepstral features could effectively classify a speaker’s gender. The results demonstrated that the models performed well across the different features, with the Linear Regression model yielding the highest performance in terms of accuracy, achieving a 99.98% accuracy rate. This was followed by the K-Nearest Neighbors (KNN) model, which attained an accuracy of 91.21%, and the Decision Tree classifier, which reached 90% accuracy. The hypothesis, which posited that pitch and MFCCs would be key features in distinguishing between male and female voices, was supported by the results. Linear Regression, in particular, showed that pitch and spectral features played significant roles in gender classification, with minimal misclassifications. Visualizations such as confusion matrices and classification reports helped to further analyze the models' performance, revealing that the Linear Regression model had very few false positives or false negatives, indicating highly accurate gender classification.
</p>

<h2>Discussion</h2>
<p>
The results suggest that the Linear Regression model, with its near-perfect accuracy, is highly effective for gender classification tasks. The significant role of pitch-related features and MFCCs aligns with previous research in speech processing, where these features have been proven to be crucial for distinguishing between male and female voices. The KNN model also performed well, demonstrating its robustness and minimal overfitting, which is particularly useful in real-world applications where robustness is a priority. While the Decision Tree classifier showed solid performance, its accuracy was lower compared to the other models, though it still holds value in applications where model interpretability is important. 
</p>
<p>
The implications of these findings extend beyond just gender classification; they suggest that speech-based features, particularly spectral and pitch-related characteristics, can be reliably used to infer gender with high accuracy. This can have practical applications in fields such as virtual assistants, where gender identification can help tailor user interactions. Future research could explore further improvements in model performance by experimenting with other advanced machine learning techniques or by incorporating additional features related to voice modulation and speaker age. Additionally, expanding the dataset to include more diverse speech samples could improve the model's generalizability and fairness.
</p>
<p>
The tools employed for this assignment, including scikit-learn’s models, evaluation metrics, and cross-validation techniques, proved to be valuable in obtaining and validating the results. While these tools provided useful insights, further exploration of more sophisticated machine learning algorithms and feature engineering techniques could yield even better results.  
</p>

<h2>Summary</h2>
<p>
This study successfully demonstrated that machine learning models could be used to classify a speaker’s gender based on vocal features. The Linear Regression model was the most accurate, achieving nearly perfect classification results. The KNN model also performed well, exhibiting robustness with minimal overfitting, while the Decision Tree classifier, although slightly less accurate, still performed solidly. Overall, the findings support the hypothesis that pitch and MFCCs are crucial features for gender classification and highlight the potential for improving speech-based applications through better gender identification models.
</p>

<h2>References</h2>
Najim, M. (2023). Vocal gender features [Data set]. Kaggle. https://www.kaggle.com/datasets/murtadhanajim/vocal-gender-features

<h2>Date Dataset was Last Downloaded</h2>
February 27, 2025
