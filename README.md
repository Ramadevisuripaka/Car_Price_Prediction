# Car_Price_Prediction
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Car Price Prediction - README</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background-color: #f6f8fa;
            color: #24292e;
            line-height: 1.7;
        }

        .page {
            max-width: 900px;
            margin: 40px auto;
            background: white;
            border-radius: 12px;
            box-shadow: 0 2px 15px rgba(0,0,0,0.1);
            padding: 50px;
        }

        /* HEADER */
        .header {
            text-align: center;
            border-bottom: 3px solid darkblue;
            padding-bottom: 25px;
            margin-bottom: 30px;
        }

        .header h1 {
            font-size: 36px;
            color: darkblue;
            margin-bottom: 15px;
        }

        .badges {
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
            margin-top: 10px;
        }

        .badge {
            padding: 5px 14px;
            border-radius: 20px;
            font-size: 13px;
            font-weight: bold;
            color: white;
        }

        .badge-blue    { background: #007ec6; }
        .badge-grey    { background: #808080; }
        .badge-green   { background: #28a745; }
        .badge-bright  { background: #44cc11; }

        /* LIVE DEMO BOX */
        .live-demo {
            background: linear-gradient(135deg, #e3f2fd, #bbdefb);
            border: 2px solid #90caf9;
            border-radius: 10px;
            padding: 20px 30px;
            text-align: center;
            margin: 25px 0;
        }

        .live-demo p {
            font-size: 18px;
            font-weight: bold;
            color: darkblue;
            margin-bottom: 10px;
        }

        .live-demo a {
            display: inline-block;
            background: darkblue;
            color: white;
            padding: 12px 30px;
            border-radius: 8px;
            text-decoration: none;
            font-size: 16px;
            font-weight: bold;
        }

        .live-demo a:hover {
            background: green;
        }

        /* SECTIONS */
        h2 {
            font-size: 24px;
            color: darkblue;
            border-bottom: 2px solid #e1e4e8;
            padding-bottom: 8px;
            margin: 35px 0 15px 0;
        }

        h3 {
            font-size: 18px;
            color: crimson;
            margin: 20px 0 10px 0;
        }

        p {
            margin-bottom: 12px;
            font-size: 16px;
        }

        ul {
            margin-left: 25px;
            margin-bottom: 15px;
        }

        ul li {
            margin-bottom: 7px;
            font-size: 16px;
        }

        /* TABLES */
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 15px 0 25px 0;
            font-size: 15px;
        }

        th {
            background: darkblue;
            color: white;
            padding: 12px 15px;
            text-align: left;
        }

        td {
            padding: 10px 15px;
            border: 1px solid #e1e4e8;
        }

        tr:nth-child(even) {
            background: #f6f8fa;
        }

        /* CODE BLOCKS */
        pre {
            background: #1e1e1e;
            color: #d4d4d4;
            padding: 20px;
            border-radius: 8px;
            overflow-x: auto;
            margin: 15px 0;
            font-size: 14px;
            font-family: "Courier New", monospace;
            line-height: 1.6;
        }

        code {
            background: #f0f0f0;
            color: crimson;
            padding: 2px 6px;
            border-radius: 4px;
            font-family: "Courier New", monospace;
            font-size: 14px;
        }

        pre code {
            background: none;
            color: #d4d4d4;
            padding: 0;
        }

        /* NOTE BOX */
        .note {
            background: #e8f5e9;
            border-left: 5px solid green;
            padding: 12px 18px;
            border-radius: 5px;
            margin: 15px 0;
            font-size: 15px;
        }

        /* STEP BOXES */
        .step {
            background: #f0f8ff;
            border: 1px solid #90caf9;
            border-radius: 8px;
            padding: 15px 20px;
            margin: 12px 0;
        }

        .step-number {
            background: darkblue;
            color: white;
            border-radius: 50%;
            width: 28px;
            height: 28px;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 14px;
            margin-right: 10px;
        }

        .step h3 {
            display: inline;
            color: darkblue;
            font-size: 16px;
        }

        /* VISUALIZATION CARDS */
        .viz-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            margin: 15px 0;
        }

        .viz-card {
            background: #fff3e0;
            border: 1px solid #ffb74d;
            border-radius: 8px;
            padding: 15px;
        }

        .viz-card h4 {
            color: darkblue;
            margin-bottom: 8px;
            font-size: 15px;
        }

        .viz-card p {
            font-size: 14px;
            color: #555;
            margin: 0;
        }

        /* FOLDER STRUCTURE */
        .folder {
            background: #1e1e1e;
            color: #d4d4d4;
            padding: 20px;
            border-radius: 8px;
            font-family: "Courier New", monospace;
            font-size: 14px;
            line-height: 1.8;
        }

        /* DIVIDER */
        hr {
            border: none;
            border-top: 2px solid #e1e4e8;
            margin: 30px 0;
        }

        /* CONTACT SECTION */
        .contact {
            background: linear-gradient(135deg, #e8f5e9, #c8e6c9);
            border: 2px solid #81c784;
            border-radius: 12px;
            padding: 30px;
            text-align: center;
            margin-top: 30px;
        }

        .contact h2 {
            border: none;
            color: darkblue;
            font-size: 26px;
            margin-bottom: 10px;
        }

        .contact h3 {
            font-size: 28px;
            color: darkblue;
            margin: 10px 0;
        }

        .contact p {
            font-size: 17px;
            margin: 8px 0;
        }

        .contact a {
            color: darkblue;
            font-weight: bold;
        }

        /* STAR NOTE */
        .star-note {
            background: #fffde7;
            border: 2px solid #fff176;
            border-radius: 10px;
            padding: 18px;
            text-align: center;
            font-size: 17px;
            font-weight: bold;
            color: #333;
            margin-top: 25px;
        }
    </style>
</head>
<body>

<div class="page">

    <!-- HEADER -->
    <div class="header">
        <h1>🚗 Car Price Prediction System</h1>
        <div class="badges">
            <span class="badge badge-blue">Python 3.10</span>
            <span class="badge badge-grey">Flask Web App</span>
            <span class="badge badge-green">Machine Learning</span>
            <span class="badge badge-bright">Status: Completed</span>
        </div>
    </div>

    <!-- LIVE DEMO -->
    <div class="live-demo">
        <p>🌐 Live Demo — Try the Application Now!</p>
        <a href="https://car-price-prediction-eyp4.onrender.com" target="_blank">
            👉 Click Here to View Live Application
        </a>
    </div>

    <hr>

    <!-- ABOUT -->
    <h2>📌 About This Project</h2>
    <p>The <strong>Car Price Prediction System</strong> is a Machine Learning web application that predicts the price of a car based on user inputs such as Brand, Year, Engine Size, Fuel Type, Transmission, Mileage, Condition, and Model.</p>
    <p>This project was built to help <strong>buyers and sellers estimate the fair market price of a car</strong> without visiting multiple dealerships. It uses a trained ML model integrated into a Flask web application with a clean and colorful UI.</p>

    <hr>

    <!-- WHY -->
    <h2>🎯 Why I Built This Project</h2>
    <ul>
        <li>To apply real-world Machine Learning on a practical dataset</li>
        <li>To learn how to integrate an ML model with a Flask web application</li>
        <li>To understand how multiple features (brand, year, mileage, etc.) affect car price</li>
        <li>To build a complete end-to-end Data Science project from data to deployment</li>
        <li>To strengthen my portfolio as a Data Analyst and ML Engineer</li>
    </ul>

    <hr>

    <!-- TOOLS -->
    <h2>🛠️ Tools and Technologies Used</h2>
    <table>
        <tr><th>Tool / Technology</th><th>Purpose</th></tr>
        <tr><td><strong>Python</strong></td><td>Core programming language</td></tr>
        <tr><td><strong>Pandas</strong></td><td>Data loading and manipulation</td></tr>
        <tr><td><strong>NumPy</strong></td><td>Numerical calculations</td></tr>
        <tr><td><strong>Scikit-learn</strong></td><td>Machine Learning model training</td></tr>
        <tr><td><strong>Matplotlib &amp; Seaborn</strong></td><td>Data visualization and graphs</td></tr>
        <tr><td><strong>Flask</strong></td><td>Web application framework</td></tr>
        <tr><td><strong>HTML &amp; CSS</strong></td><td>Frontend UI design</td></tr>
        <tr><td><strong>Jinja2</strong></td><td>Template rendering in Flask</td></tr>
        <tr><td><strong>Joblib</strong></td><td>Saving and loading the trained model</td></tr>
        <tr><td><strong>GitHub</strong></td><td>Version control and project hosting</td></tr>
        <tr><td><strong>VS Code</strong></td><td>Code editor</td></tr>
    </table>

    <hr>

    <!-- DATASET -->
    <h2>📊 Dataset Overview</h2>
    <p><strong>Features Used:</strong></p>
    <ul>
        <li>Brand (Tesla, BMW, Audi, Ford, Honda, Mercedes, Toyota)</li>
        <li>Year of Manufacture</li>
        <li>Engine Size (in litres)</li>
        <li>Fuel Type (Petrol / Diesel)</li>
        <li>Transmission (Manual / Automatic)</li>
        <li>Mileage (in km)</li>
        <li>Condition (New / Used / Like New)</li>
        <li>Model (Model X, 5 Series, A4, Mustang, City, C Class, Innova)</li>
    </ul>
    <p><strong>Target Variable:</strong> Car Price (in currency units)</p>

    <hr>

    <!-- MANUAL CALCULATIONS -->
    <h2>🧮 Manual Calculations (Step by Step)</h2>

    <h3>Step 1 — Label Encoding</h3>
    <p>Categorical values are converted to numbers before training:</p>

    <table>
        <tr><th>Brand</th><th>Encoded Value</th></tr>
        <tr><td>Tesla</td><td>0</td></tr>
        <tr><td>BMW</td><td>1</td></tr>
        <tr><td>Audi</td><td>2</td></tr>
        <tr><td>Ford</td><td>3</td></tr>
        <tr><td>Honda</td><td>4</td></tr>
        <tr><td>Mercedes</td><td>5</td></tr>
        <tr><td>Toyota</td><td>6</td></tr>
    </table>

    <table>
        <tr><th>Fuel Type</th><th>Encoded Value</th></tr>
        <tr><td>Petrol</td><td>0</td></tr>
        <tr><td>Diesel</td><td>1</td></tr>
    </table>

    <table>
        <tr><th>Transmission</th><th>Encoded Value</th></tr>
        <tr><td>Manual</td><td>0</td></tr>
        <tr><td>Automatic</td><td>1</td></tr>
    </table>

    <table>
        <tr><th>Condition</th><th>Encoded Value</th></tr>
        <tr><td>New</td><td>0</td></tr>
        <tr><td>Used</td><td>1</td></tr>
        <tr><td>Like New</td><td>2</td></tr>
    </table>

    <h3>Step 2 — Linear Regression Formula</h3>
    <p>The model uses <strong>Multiple Linear Regression</strong>:</p>
    <pre><code>Price = b0 + b1(Brand) + b2(Year) + b3(Engine) + b4(Fuel) + b5(Transmission) + b6(Mileage) + b7(Condition) + b8(Model)</code></pre>
    <ul>
        <li><code>b0</code> = Intercept (base price)</li>
        <li><code>b1 to b8</code> = Coefficients (weight of each feature)</li>
    </ul>

    <h3>Step 3 — Manual Example Calculation</h3>
    <p><strong>Input Values:</strong></p>
    <pre><code>Brand        = BMW        → encoded = 1
Year         = 2020
Engine Size  = 2.0
Fuel Type    = Diesel     → encoded = 1
Transmission = Automatic  → encoded = 1
Mileage      = 30000
Condition    = Used       → encoded = 1
Model        = 5 Series   → encoded = 1</code></pre>

    <p><strong>Assume model coefficients (example):</strong></p>
    <pre><code>b0  = 5000
b1  = 3000   (Brand)
b2  = 200    (Year)
b3  = 1500   (Engine)
b4  = 500    (Fuel)
b5  = 1000   (Transmission)
b6  = -0.05  (Mileage — negative: higher mileage = lower price)
b7  = -2000  (Condition — used = lower price)
b8  = 1200   (Model)</code></pre>

    <p><strong>Manual Calculation:</strong></p>
    <pre><code>Price = 5000
      + (3000 × 1)       → Brand BMW
      + (200  × 2020)    → Year
      + (1500 × 2.0)     → Engine
      + (500  × 1)       → Diesel
      + (1000 × 1)       → Automatic
      + (-0.05 × 30000)  → Mileage
      + (-2000 × 1)      → Used condition
      + (1200 × 1)       → 5 Series model

Price = 5000 + 3000 + 404000 + 3000 + 500 + 1000 - 1500 - 2000 + 1200

Price = ₹ 4,15,200 (approximately)</code></pre>

    <div class="note">✅ The actual model uses scikit-learn to calculate exact coefficients from the training data automatically.</div>

    <h3>Step 4 — Train-Test Split</h3>
    <pre><code>Total Dataset  → 100%
Training Data  → 80%  (model learns from this)
Testing Data   → 20%  (model is evaluated on this)</code></pre>

    <h3>Step 5 — Model Accuracy</h3>
    <pre><code>R² Score  = 1 - (SS_residual / SS_total)

Mean Absolute Error (MAE)  = Average of |Actual - Predicted|

Mean Squared Error  (MSE)  = Average of (Actual - Predicted)²

Root Mean Squared Error (RMSE) = √MSE</code></pre>

    <hr>

    <!-- VISUALIZATIONS -->
    <h2>📈 Visualizations</h2>
    <p>The following graphs were plotted during the analysis:</p>

    <div class="viz-grid">
        <div class="viz-card">
            <h4>1. Brand vs Average Price</h4>
            <p>Bar chart showing which brand has highest average price. Tesla and Mercedes were highest.</p>
        </div>
        <div class="viz-card">
            <h4>2. Mileage vs Price (Scatter)</h4>
            <p>As mileage increases, price decreases — showing a negative correlation.</p>
        </div>
        <div class="viz-card">
            <h4>3. Year vs Price</h4>
            <p>Newer cars have higher prices — showing a positive correlation.</p>
        </div>
        <div class="viz-card">
            <h4>4. Fuel Type Distribution (Pie)</h4>
            <p>Distribution of Petrol vs Diesel cars in the dataset.</p>
        </div>
        <div class="viz-card">
            <h4>5. Correlation Heatmap</h4>
            <p>Year and Engine Size had the highest positive correlation with price.</p>
        </div>
        <div class="viz-card">
            <h4>6. Actual vs Predicted Price</h4>
            <p>Compares model predictions against real values. Points near diagonal = good predictions.</p>
        </div>
    </div>

    <hr>

    <!-- HOW TO RUN -->
    <h2>🚀 How to Run This Project</h2>

    <div class="step">
        <span class="step-number">1</span>
        <h3>Clone the Repository</h3>
        <pre><code>git clone https://github.com/yourusername/car-price-prediction.git
cd car-price-prediction</code></pre>
    </div>

    <div class="step">
        <span class="step-number">2</span>
        <h3>Install Required Libraries</h3>
        <pre><code>pip install -r requirements.txt</code></pre>
    </div>

    <div class="step">
        <span class="step-number">3</span>
        <h3>Train the Model</h3>
        <pre><code>python model.py</code></pre>
    </div>

    <div class="step">
        <span class="step-number">4</span>
        <h3>Run the Flask App</h3>
        <pre><code>python app.py</code></pre>
    </div>

    <div class="step">
        <span class="step-number">5</span>
        <h3>Open in Browser</h3>
        <pre><code>http://127.0.0.1:5000</code></pre>
    </div>

    <hr>

    <!-- PROJECT STRUCTURE -->
    <h2>📁 Project Structure</h2>
    <div class="folder">
car-price-prediction/<br>
│<br>
├── static/<br>
│&nbsp;&nbsp;&nbsp;├── vt image.jpeg<br>
│&nbsp;&nbsp;&nbsp;├── Tesla-Motors-Model-S.jpg<br>
│&nbsp;&nbsp;&nbsp;├── bmw-7-series-1.webp<br>
│&nbsp;&nbsp;&nbsp;├── audi-a4-1.webp<br>
│&nbsp;&nbsp;&nbsp;├── ford.avif<br>
│&nbsp;&nbsp;&nbsp;├── honda.webp<br>
│&nbsp;&nbsp;&nbsp;├── benz.avif<br>
│&nbsp;&nbsp;&nbsp;└── toyota.jpg<br>
│<br>
├── templates/<br>
│&nbsp;&nbsp;&nbsp;└── index.html<br>
│<br>
├── app.py<br>
├── model.py<br>
├── car_model.pkl<br>
├── requirements.txt<br>
├── Procfile<br>
└── README.md
    </div>

    <hr>

    <!-- REQUIREMENTS -->
    <h2>📦 Requirements</h2>
    <pre><code>flask
scikit-learn
pandas
numpy
matplotlib
seaborn
joblib
gunicorn</code></pre>

    <hr>

    <!-- DEPLOYMENT -->
    <h2>🌐 Deployment</h2>
    <p>This project is deployed on <strong>Render</strong>:</p>
    <ul>
        <li>Live Link → <a href="https://car-price-prediction-eyp4.onrender.com" target="_blank">https://car-price-prediction-eyp4.onrender.com</a></li>
        <li><code>Procfile</code> → <code>web: gunicorn app:app</code></li>
        <li><code>requirements.txt</code> → all dependencies</li>
        <li><code>runtime.txt</code> → Python version</li>
    </ul>

    <hr>

    <!-- CONTACT -->
    <div class="contact">
        <h2>🤝 Support &amp; Contact</h2>
        <p>If you found this project helpful or want to collaborate, feel free to reach out:</p>
        <br>
        <p><strong>Developed By</strong></p>
        <h3>Suripaka Ramadevi</h3>
        <p>💼 Role — Data Analyst and ML Engineer</p>
        <p>🏢 Training — Vihara Tech Private Limited</p>
        <p>📧 Email — <a href="mailto:ramdevisuripaka6@gmail.com">ramdevisuripaka6@gmail.com</a></p>
    </div>

    <!-- STAR NOTE -->
    <div class="star-note">
        ⭐ If you like this project, please give it a <strong>star</strong> on GitHub — it really helps!
    </div>

</div>

</body>
</html>
