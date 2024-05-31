<h2>Problem Statement</h2>
  <p>Despite advancements in IoT security, botnets continue to pose significant threats to IoT networks, compromising data integrity and system performance. This study aims to comprehensively analyze botnet behavior in IoT networks, including attack patterns, impacts, and detection mechanisms using machine learning.</p>

  <h2>Analytic problem type</h2>
  <p>Classification problem: Identifying the type of botnet attacks within IoT network traffic data.</p>

  <h2>Objectives</h2>
  <p>Gain insights into botnet behavior and characteristics within IoT networks through an in-depth analysis of attack patterns, features, and impacts. Develop accurate detection mechanisms using machine learning to identify various types of botnet attacks in IoT networks. Ensuring that machine learning models generalize well to new and unseen botnet attack instances.</p>

  <h2>Success Criteria</h2>
  <p>Limited understanding of IoT network architecture, protocols, and security vulnerabilities Successfully identify and analyze botnet attack patterns in IoT network traffic data. Limited availability of comprehensive and diverse datasets for training machine learning models Develop machine learning models with high detection accuracy for different types of botnet attacks. Demonstrate the effectiveness of the detection mechanisms by reducing the false positive rate and response time</p>

  <h2>Hypothesis 1</h2>
  <p>Botnet attacks in IoT networks exhibit distinct patterns in network traffic data, including abnormal packet and byte counts, unusual traffic rates, and atypical protocol usage.</p>

  <h2>Hypothesis 2</h2>
  <p>Machine learning models trained on diverse datasets containing features indicative of botnet activities can accurately detect and classify different types of botnet attacks in IoT networks.</p>

  <h2>Use of the 3 V’s</h2>
  <p><strong>Volume:</strong> Analyzing large volumes of IoT network traffic data to identify patterns and anomalies indicative of botnet attacks.<br>
    <strong>Variety:</strong> Handling diverse types of network traffic features, including source and destination IP addresses, ports, protocols, packet counts, and traffic rates.<br>
    <strong>Velocity:</strong> Detecting botnet attacks in real-time or near real-time to enable proactive defense measures and minimize the impact on IoT network infrastructure.</p>

  <h2>Dataset Description</h2>
  <p>We selected the Dataset from kaggle name - BoT-IoT - All Features - 5% sample The dataset comprises of 46 columns and around 1 million rows and after preprocessing we were left with 40 columns. The main columns are Category, Subcategory, State, flags, proto</p>

  <h2> Models used </h2>
  <ul>
    <li>Naive Bayes</li>
    <li>Logistic Regression</li>
    <li>XGBoost</li>
    <li>Decision Tree(Information Gain)</li>
    <li>Decision Tree (Gini)</li>
    <li>Random Forest</li>
    <li>CNN</li>
  </ul>

  <h2>Evaluation</h2>
  <ul>
    <li>Precision: The XGBoost model has the highest precision (~0.1), indicating potential overfitting. The CNN model follows with a precision of 0.97.</li>
    <li>Recall: All models show high recall (0.65 to 0.9), indicating a strong ability to capture true positives. CNN has the highest recall after XGBoost.</li>
    <li>F1-score: XGBoost has the highest F1-score, followed by CNN and Random Forest, with scores ranging from 0.6 to 0.9.</li>
    <li>Accuracy: All models have high accuracy (0.7 to 0.9), with less variation compared to F1-scores. XGBoost has the highest accuracy (~1), suggesting overfitting, followed by CNN and Random Forest.</li>
  </ul>

  <h2>HyperParameter Tuning</h2>
  <p>We conducted hyperparameter tuning for Logistic Regression, Decision Trees, Random Forest, and Convolutional Neural Networks (CNNs) to optimize their performance. This process involved adjusting parameters to improve each model's accuracy and effectiveness in detecting botnet activities. After thorough evaluation, the CNN model consistently achieved the highest scores, demonstrating superior capability in capturing intricate patterns in the network traffic data compared to the other models.</p>

  <h2>Deployment</h2>
  <p>Utilizing the CNN model, we developed a Streamlit application for attack detection. Users input values for various fields, and the application swiftly identifies whether the activity corresponds to a Denial of Service (DoS) or Distributed Denial of Service (DDoS) attack.</p>
  <h2>Conclusion</h2>
  <p>Analysis of the botnet behavior in IoT networks and designing a machine learning based detection system has been successfully completed which will go a long way in improving the security of IoT networks. With an accuracy of 97% using CNN, the project has shown some very promising results using the latest technology to fight against the dynamic threats in the cyber world.
</p>

<h2>Future Work</h2>
<p>For future extensions, we would be using much larger datasets to train and test the detection system. A large dataset containing various types of attacks, both known and unknown, can be used to train the model so that it can detect a variety of attacks and also it will make the detection system more robust and resilient enabling it to detect unknown attacks thereby taking a proactive measure to stop its proliferation. Also, a combination of multiple machine learning algorithms can be used as an ensemble technique, for example, decision trees, random forest, gradient boosting etc., all these algorithms can be trained with the dataset and the output of each algorithm can be taken as the input for the next one. </p>

<h2>Team Members</h2>
<p>Dyuti Dasmahapatra</p>
<p> Ankur Kaushal</p>
