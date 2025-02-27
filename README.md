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

<h2>Dataset</h2>
<p>
The dataset selected for this project is the Vocal Gender Features dataset, available on Kaggle: https://www.kaggle.com/datasets/murtadhanajim/vocal-gender-features
This dataset contains a collection of extracted audio features from speech recordings, to classify the speaker's gender as either male (1) or female (0).
</p>

<h2>Goal</h2>
<p>
This study seeks to discover which combination of spectral, pitch, energy, and cepstral features is most effective in classifying a speaker's gender using machine learning models. By employing data preprocessing, feature engineering, and machine learning algorithms, this study will evaluate the relative importance of these feature groups in gender classification. The results of this research may contribute to advancements in speech-processing applications by improving the accuracy and reliability of automated gender recognition systems.
</p>

<h2>Features</h2>
<p>
The dataset includes various spectral, pitch, energy, and cepstral features that characterize the acoustic properties of speech. Spectral features such as spectral centroid, bandwidth, and contrast provide insights into the distribution of frequencies in the signal, which can help differentiate between male and female voices. Pitch-related features, including mean, minimum, and maximum pitch, capture variations in fundamental frequency, a key factor in gender classification. Energy-based features like root mean square (RMS) energy and zero-crossing rate measure the overall loudness and signal variability, while Mel-Frequency Cepstral Coefficients (MFCCs) represent the timbral characteristics of the voice, commonly used in speech recognition tasks.
</p>

<h2>Methods</h2>
<h3>Materials</h3>
From sklearn:
<ul>
  <li>KNeighborsClassifier</li>
  <li>KNeighborsRegressor</li>
  <li>LinearRegression</li>
  <li>DecisionTreeClassifier</li>
  <li>StandardScaler</li>
   <li>train_test_split</li>
  <li>cross_val_score</li>
  <li>GridSearchCV</li>
  <li>learning_curve</li>
  <li>mean_squared_error</li>
  <li>accuracy_score</li>
  <li>r2_score</li>
  <li>confusion_matrix</li>
  <li>classification_report</li>
</ul>
From imblearn:
<ul>
  <li>SMOTE</li>
  <li>RandomOverSampler</li>
</ul>
<h3>APIs</h3>
<ul>
  <li>KaggleHub</li>
</ul>
<h3>Tools</h3>
<ul>
  <li>Numpy</li>
  <li>Pandas</li>
  <li>Seaborn</li>
  <li>os</li>
  <li>matplotlib.pyplot</li>
</ul>

<h2>Results</h2>
<i>What answer was found to the research question; what did the study find? Was the tested hypothesis true? Any visualizations?</i>

<h2>Discussion</h2>


<h2>Summary</h2>

