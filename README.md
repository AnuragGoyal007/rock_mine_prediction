<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rock vs Mine Prediction - README</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom styles for better readability and aesthetics */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f2f5; /* Light gray background */
            color: #333;
            line-height: 1.6;
        }
        .container {
            max-width: 800px;
            margin: 2rem auto;
            padding: 2rem;
            background-color: #ffffff;
            border-radius: 0.75rem; /* Rounded corners */
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }
        h1, h2, h3 {
            color: #2c3e50; /* Darker heading color */
            font-weight: 700;
            margin-bottom: 1rem;
        }
        h1 {
            font-size: 2.5rem;
            text-align: center;
            border-bottom: 2px solid #e0e0e0;
            padding-bottom: 1rem;
            margin-bottom: 2rem;
        }
        h2 {
            font-size: 2rem;
            border-bottom: 1px solid #e0e0e0;
            padding-bottom: 0.5rem;
            margin-top: 2rem;
        }
        h3 {
            font-size: 1.5rem;
            margin-top: 1.5rem;
        }
        a {
            color: #3498db; /* Blue links */
            text-decoration: none;
            transition: color 0.3s ease;
        }
        a:hover {
            color: #2980b9;
        }
        ul {
            list-style-type: disc;
            margin-left: 1.5rem;
            margin-bottom: 1rem;
        }
        ol {
            list-style-type: decimal;
            margin-left: 1.5rem;
            margin-bottom: 1rem;
        }
        code {
            background-color: #e9ecef;
            padding: 0.2em 0.4em;
            border-radius: 0.25rem;
            font-family: 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, Courier, monospace;
        }
        pre {
            background-color: #2d2d2d; /* Dark background for code blocks */
            color: #f8f8f2; /* Light text for code blocks */
            padding: 1rem;
            border-radius: 0.5rem;
            overflow-x: auto;
            margin-bottom: 1.5rem;
        }
        pre code {
            background-color: transparent;
            padding: 0;
            color: inherit;
        }
    </style>
</head>
<body class="p-4">
    <div class="container">
        <h1 class="text-gray-800">Rock vs Mine Prediction using Logistic Regression</h1>

        <p class="mb-4">This project demonstrates a machine learning model built using Logistic Regression to classify sonar signals as either a "Rock" or a "Mine". The dataset used contains 60 features representing the sonar signal and a target variable indicating whether the object is a rock or a mine.</p>

        <h2 class="text-gray-700">Table of Contents</h2>
        <ul class="list-none pl-0">
            <li><a href="#project-overview" class="text-blue-600 hover:underline">Project Overview</a></li>
            <li><a href="#dataset" class="text-blue-600 hover:underline">Dataset</a></li>
            <li><a href="#dependencies" class="text-blue-600 hover:underline">Dependencies</a></li>
            <li><a href="#project-structure" class="text-blue-600 hover:underline">Project Structure</a></li>
            <li><a href="#how-to-run" class="text-blue-600 hover:underline">How to Run</a></li>
            <li><a href="#model-performance" class="text-blue-600 hover:underline">Model Performance</a></li>
            <li><a href="#contributing" class="text-blue-600 hover:underline">Contributing</a></li>
        </ul>

        <h2 id="project-overview" class="text-gray-700">Project Overview</h2>
        <p class="mb-4">The goal of this project is to accurately distinguish between rocks and mines based on sonar data. A Logistic Regression model is trained on a pre-processed dataset, and its performance is evaluated using accuracy scores on both training and test sets. The project also includes a simple predictive system to demonstrate how the trained model can be used to classify new, unseen data.</p>

        <h2 id="dataset" class="text-gray-700">Dataset</h2>
        <p class="mb-4">The dataset, <code>sonar.csv</code>, consists of 208 entries, each with 60 numerical features and a target label.</p>
        <ul class="mb-4">
            <li><strong>Features (Columns 0-59):</strong> These represent various characteristics extracted from the sonar signals.</li>
            <li><strong>Target (Column 60):</strong> This column contains the labels 'R' (Rock) or 'M' (Mine).</li>
        </ul>

        <h3 class="text-gray-700">Data Distribution</h3>
        <ul class="mb-4">
            <li>Mines (M): 111 instances</li>
            <li>Rocks (R): 97 instances</li>
        </ul>

        <h2 id="dependencies" class="text-gray-700">Dependencies</h2>
        <p class="mb-4">To run this notebook, you will need the following Python libraries:</p>
        <ul class="mb-4">
            <li><code>numpy</code></li>
            <li><code>pandas</code></li>
            <li><code>scikit-learn</code></li>
        </ul>
        <p class="mb-4">You can install them using pip:</p>
        <pre><code>pip install numpy pandas scikit-learn</code></pre>

        <h2 id="project-structure" class="text-gray-700">Project Structure</h2>
        <ul class="mb-4">
            <li><code>Rock vs Mine Prediction.ipynb</code>: The main Jupyter Notebook containing the data loading, preprocessing, model training, evaluation, and prediction logic.</li>
            <li><code>sonar.csv</code>: The dataset used for training and testing the model.</li>
        </ul>

        <h2 id="how-to-run" class="text-gray-700">How to Run</h2>
        <ol class="mb-4">
            <li><strong>Clone the repository:</strong>
                <pre><code>git clone https://github.com/AnuragGoyal007/rock_mine_prediction
            cd rock_mine_prediction</code></pre>
            </li>
            <li><strong>Install dependencies:</strong>
                <pre><code>pip install -r requirements.txt</code></pre>
                <p class="mt-2">Alternatively, install them manually as listed in the <a href="#dependencies" class="text-blue-600 hover:underline">Dependencies</a> section.</p>
            </li>
            <li><strong>Open the Jupyter Notebook:</strong>
                <pre><code>jupyter notebook "Rock vs Mine Prediction.ipynb"</code></pre>
            </li>
            <li><strong>Run all cells</strong> in the notebook to see the data processing, model training, and evaluation results.</li>
        </ol>

        <h2 id="model-performance" class="text-gray-700">Model Performance</h2>
        <p class="mb-4">The Logistic Regression model achieved the following accuracy scores:</p>
        <ul class="mb-4">
            <li><strong>Accuracy on Training Data:</strong> ~83.42%</li>
            <li><strong>Accuracy on Test Data:</strong> ~76.19%</li>
        </ul>

        <h2 id="contributing" class="text-gray-700">Contributing</h2>
        <p class="mb-4">Feel free to fork this repository, make improvements, and submit pull requests. Any contributions are welcome!</p>
    </div>
</body>
</html>
