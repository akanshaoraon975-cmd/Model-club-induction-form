i# Model-club-induction-form
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Model Club BIT Sindri - Induction Form</title>
  <style>
    :root {
      --bg-color: #0d1117;
      --card-bg: #161b22;
      --accent-color: #00e5ff;
      --accent-hover: #00b3cc;
      --text-color: #f0f6fc;
      --text-muted: #8b949e;
      --border-color: #30363d;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background-color: var(--bg-color);
      color: var(--text-color);
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      padding: 20px;
    }

    .form-container {
      background-color: var(--card-bg);
      border: 1px solid var(--border-color);
      border-radius: 12px;
      padding: 30px;
      width: 100%;
      max-width: 500px;
      box-shadow: 0 8px 24px rgba(0, 0, 0, 0.5);
    }

    .header {
      text-align: center;
      margin-bottom: 25px;
    }

    .header h1 {
      font-size: 1.6rem;
      color: var(--accent-color);
      letter-spacing: 1px;
      text-transform: uppercase;
    }

    .header p {
      color: var(--text-muted);
      font-size: 0.9rem;
      margin-top: 5px;
    }

    .form-group {
      margin-bottom: 18px;
    }

    .form-group label {
      display: block;
      margin-bottom: 6px;
      font-size: 0.85rem;
      color: var(--text-color);
      font-weight: 600;
    }

    .form-group input, 
    .form-group select, 
    .form-group textarea {
      width: 100%;
      padding: 12px;
      background-color: var(--bg-color);
      border: 1px solid var(--border-color);
      border-radius: 6px;
      color: var(--text-color);
      font-size: 0.95rem;
      outline: none;
      transition: border-color 0.2s ease;
    }

    .form-group input:focus, 
    .form-group select:focus, 
    .form-group textarea:focus {
      border-color: var(--accent-color);
    }

    .form-row {
      display: flex;
      gap: 12px;
    }

    .form-row .form-group {
      flex: 1;
    }

    .submit-btn {
      width: 100%;
      padding: 12px;
      background-color: var(--accent-color);
      color: #000;
      font-weight: bold;
      font-size: 1rem;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      transition: background-color 0.2s ease;
      margin-top: 10px;
    }

    .submit-btn:hover {
      background-color: var(--accent-hover);
    }

    /* Footer styling added */
    .form-footer {
      margin-top: 25px;
      padding-top: 15px;
      border-top: 1px solid var(--border-color);
      text-align: center;
      font-size: 0.85rem;
      color: #ffffff;
    }

    .form-footer p {
      margin-bottom: 6px;
    }

    .form-footer a {
      color: #ffffff;
      text-decoration: underline;
    }

    .form-footer a:hover {
      color: var(--accent-color);
    }

    @media (max-width: 480px) {
      .form-row {
        flex-direction: column;
        gap: 0;
      }
    }
  </style>
</head>
<body>

  <div class="form-container">
    <div class="header">
      <h1>Model Club</h1>
      <p>B.I.T. Sindri — Induction Registration</p>
    </div>

    <form action="#" method="POST">
      <div class="form-group">
        <label for="fullname">Full Name *</label>
        <input type="text" id="fullname" name="fullname" placeholder="Enter your full name" required>
      </div>

      <div class="form-row">
        <div class="form-group">
          <label for="roll">Roll No. *</label>
          <input type="text" id="roll" name="roll" placeholder="e.g. 2301045" required>
        </div>
        <div class="form-group">
          <label for="batch">Batch *</label>
          <select id="batch" name="batch" required>
            <option value="" disabled selected>Select Batch</option>
            <option value="2k26">2k26</option>
            <option value="2k25">2k25</option>
          </select>
        </div>
      </div>

      <div class="form-group">
        <label for="branch">Branch *</label>
        <select id="branch" name="branch" required>
          <option value="" disabled selected>Select Branch</option>
          <option value="CSE">Computer Science & Engg.</option>
          <option value="CSE CYBER">Computer Science Cyber Security</option>
          <option value="IT">Information Technology</option>
          <option value="ECE">Electronics & Comm. Engg.</option>
          <option value="EE">Electrical Engg.</option>
          <option value="ME">Mechanical Engg.</option>
          <option value="CE">Civil Engg.</option>
          <option value="CHE">Chemical Engg.</option>
          <option value="MME">Metallurgical Engg.</option>
          <option value="MIN">Mining Engg.</option>
          <option value="PE">Production Engg.</option>
        </select>
      </div>

      <div class="form-group">
        <label for="email">Email Address *</label>
        <input type="email" id="email" name="email" placeholder="student@bitsindri.ac.in" required>
      </div>

      <div class="form-group">
        <label for="phone">WhatsApp Number *</label>
        <input type="tel" id="phone" name="phone" placeholder="10-digit phone number" pattern="[0-9]{10}" required>
      </div>

      <div class="form-group">
        <label for="domain">Preferred Domain *</label>
        <select id="domain" name="domain" required>
          <option value="" disabled selected>Choose domain of interest</option>
          <option value="web-dev">Web Development</option>
          <option value="robotics">Robotics & UAV (Unmanned aerial vehicle)</option>
          <option value="visual eff">Visual Effect</option>
          <option value="competitive prog">Competitive Programming</option>
          <option value="IOT">Internet of things</option>     
          <option value="design">Graphic Design (GFX)</option>
          <option value="AI/ML">AI/ML</option>
          <option value="ethical hack">Ethical Hacking</option>
        </select>
      </div>
      
      <div class="form-group">
        <label for="strength">What is your strength?</label>
        <textarea id="strength" name="strength" rows="3" placeholder="Briefly state your strength.."></textarea>
      </div>
      
      <div class="form-group">
        <label for="weakness">What is your weakness?</label>
        <textarea id="weakness" name="weakness" rows="3" placeholder="Briefly state your weakness.."></textarea>
      </div>
      
      <div class="form-group">
        <label for="hobbies">What is your hobby?</label>
        <textarea id="hobbies" name="hobbies" rows="3" placeholder="Briefly state your hobby.."></textarea>
      </div>
      
      <div class="form-group">
        <label for="queries">Do you have any query about model club?</label>
        <textarea id="queries" name="queries" rows="3" placeholder="Briefly state your query.."></textarea>
      </div>

      <div class="form-group">
        <label for="reason">Why do you want to join Model Club?</label>
        <textarea id="reason" name="reason" rows="3" placeholder="Briefly state your motivation..."></textarea>
      </div>

      <button type="submit" class="submit-btn">Submit Application</button>
    </form>

    <div class="form-footer">
      <p>Email: modelclub.bitsindri@gmail.com</p>
      <p>Contact: +91 98765 43210</p>
      <p>Website: <a href="https://modelclubbit.in" target="_blank" rel="noopener noreferrer">modelclubbit.in</a></p>
    </div>
  </div>

</body>
</html>
