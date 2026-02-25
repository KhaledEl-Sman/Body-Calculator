<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Health Calculator</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --bg: #0d1117;
    --surface: #161b22;
    --card: #1c2333;
    --border: #30363d;
    --accent: #58a6ff;
    --accent2: #3fb950;
    --accent3: #f78166;
    --text: #e6edf3;
    --muted: #8b949e;
    --radius: 16px;
  }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: 'DM Sans', sans-serif;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 24px;
    background-image: radial-gradient(ellipse at 20% 50%, rgba(88,166,255,0.06) 0%, transparent 60%),
                      radial-gradient(ellipse at 80% 20%, rgba(63,185,80,0.05) 0%, transparent 50%);
  }

  .wrapper {
    width: 100%;
    max-width: 560px;
    animation: fadeUp 0.6s ease both;
  }

  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(30px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  header {
    text-align: center;
    margin-bottom: 36px;
  }

  header .pill {
    display: inline-block;
    background: rgba(88,166,255,0.12);
    color: var(--accent);
    font-size: 12px;
    font-weight: 600;
    letter-spacing: 2px;
    text-transform: uppercase;
    padding: 6px 16px;
    border-radius: 50px;
    border: 1px solid rgba(88,166,255,0.2);
    margin-bottom: 14px;
  }

  header h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(2rem, 5vw, 2.8rem);
    line-height: 1.15;
    background: linear-gradient(135deg, #e6edf3 0%, #8b949e 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  header p {
    color: var(--muted);
    margin-top: 10px;
    font-size: 15px;
    font-weight: 300;
  }

  .card {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 32px;
    position: relative;
    overflow: hidden;
  }

  .card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 2px;
    background: linear-gradient(90deg, var(--accent), var(--accent2));
    border-radius: var(--radius) var(--radius) 0 0;
  }

  .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 18px;
  }

  .field {
    display: flex;
    flex-direction: column;
    gap: 8px;
  }

  .field.full { grid-column: 1 / -1; }

  label {
    font-size: 12px;
    font-weight: 600;
    letter-spacing: 1px;
    text-transform: uppercase;
    color: var(--muted);
  }

  input, select {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 10px;
    color: var(--text);
    font-family: 'DM Sans', sans-serif;
    font-size: 15px;
    padding: 12px 16px;
    width: 100%;
    transition: border-color 0.2s, box-shadow 0.2s;
    -webkit-appearance: none;
    appearance: none;
  }

  select {
    cursor: pointer;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='12' viewBox='0 0 12 12'%3E%3Cpath fill='%238b949e' d='M6 8L1 3h10z'/%3E%3C/svg%3E");
    background-repeat: no-repeat;
    background-position: right 14px center;
    padding-right: 36px;
  }

  input:focus, select:focus {
    outline: none;
    border-color: var(--accent);
    box-shadow: 0 0 0 3px rgba(88,166,255,0.12);
  }

  input::placeholder { color: var(--muted); opacity: 0.6; }

  .gender-group {
    display: flex;
    gap: 10px;
  }

  .gender-btn {
    flex: 1;
    padding: 11px;
    border-radius: 10px;
    border: 1px solid var(--border);
    background: var(--surface);
    color: var(--muted);
    font-family: 'DM Sans', sans-serif;
    font-size: 14px;
    font-weight: 500;
    cursor: pointer;
    transition: all 0.2s;
    text-align: center;
  }

  .gender-btn.active {
    border-color: var(--accent);
    background: rgba(88,166,255,0.1);
    color: var(--accent);
  }

  .divider {
    height: 1px;
    background: var(--border);
    margin: 24px 0;
  }

  .btn {
    width: 100%;
    padding: 15px;
    border-radius: 12px;
    border: none;
    background: linear-gradient(135deg, #58a6ff, #3fb950);
    color: #0d1117;
    font-family: 'DM Sans', sans-serif;
    font-size: 16px;
    font-weight: 700;
    cursor: pointer;
    transition: opacity 0.2s, transform 0.15s;
    margin-top: 8px;
    letter-spacing: 0.3px;
  }

  .btn:hover { opacity: 0.92; transform: translateY(-1px); }
  .btn:active { transform: translateY(0); }

  /* POPUP */
  .overlay {
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.75);
    backdrop-filter: blur(6px);
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 24px;
    z-index: 100;
    opacity: 0;
    pointer-events: none;
    transition: opacity 0.3s;
  }

  .overlay.show {
    opacity: 1;
    pointer-events: all;
  }

  .popup {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 20px;
    padding: 36px;
    width: 100%;
    max-width: 480px;
    transform: scale(0.9) translateY(20px);
    transition: transform 0.35s cubic-bezier(0.34,1.56,0.64,1);
    position: relative;
    overflow: hidden;
  }

  .overlay.show .popup {
    transform: scale(1) translateY(0);
  }

  .popup-header {
    text-align: center;
    margin-bottom: 28px;
  }

  .popup-avatar {
    width: 64px;
    height: 64px;
    border-radius: 50%;
    background: linear-gradient(135deg, rgba(88,166,255,0.2), rgba(63,185,80,0.2));
    border: 2px solid var(--border);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 26px;
    margin: 0 auto 14px;
  }

  .popup-name {
    font-family: 'Playfair Display', serif;
    font-size: 1.6rem;
  }

  .popup-subtitle {
    color: var(--muted);
    font-size: 13px;
    margin-top: 4px;
  }

  .bmi-badge {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 8px 20px;
    border-radius: 50px;
    font-weight: 700;
    font-size: 14px;
    margin-top: 14px;
    border: 1.5px solid;
  }

  .stats-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 14px;
    margin: 24px 0;
  }

  .stat-box {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 18px;
    text-align: center;
    position: relative;
    overflow: hidden;
  }

  .stat-box::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 3px;
  }

  .stat-box.bmr::before { background: var(--accent); }
  .stat-box.tdee::before { background: var(--accent2); }
  .stat-box.goal::before { background: var(--accent3); }

  .stat-box.goal { grid-column: 1 / -1; }

  .stat-label {
    font-size: 11px;
    font-weight: 700;
    letter-spacing: 1.5px;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 8px;
  }

  .stat-value {
    font-family: 'Playfair Display', serif;
    font-size: 2rem;
    line-height: 1;
  }

  .stat-value.bmr-val { color: var(--accent); }
  .stat-value.tdee-val { color: var(--accent2); }
  .stat-value.goal-val { color: var(--accent3); }

  .stat-unit {
    font-size: 12px;
    color: var(--muted);
    margin-top: 4px;
  }

  .close-btn {
    width: 100%;
    padding: 13px;
    border-radius: 12px;
    border: 1px solid var(--border);
    background: transparent;
    color: var(--muted);
    font-family: 'DM Sans', sans-serif;
    font-size: 15px;
    font-weight: 500;
    cursor: pointer;
    transition: all 0.2s;
  }

  .close-btn:hover {
    background: var(--surface);
    color: var(--text);
    border-color: var(--accent);
  }

  @media (max-width: 480px) {
    .grid-2 { grid-template-columns: 1fr; }
    .card { padding: 24px; }
    .popup { padding: 28px 22px; }
  }
</style>
</head>
<body>

<div class="wrapper">
  <header>
    <div class="pill">Health Metrics</div>
    <h1>Body Calculator</h1>
    <p>BMI · BMR · TDEE — all in one place</p>
  </header>

  <div class="card">
    <div class="grid-2">

      <div class="field full">
        <label>Patient Name</label>
        <input type="text" id="name" placeholder="e.g. Ahmed Hassan">
      </div>

      <div class="field full">
        <label>Gender</label>
        <div class="gender-group">
          <button class="gender-btn active" id="btn-male" onclick="selectGender('male')">♂ Male</button>
          <button class="gender-btn" id="btn-female" onclick="selectGender('female')">♀ Female</button>
        </div>
      </div>

      <div class="field">
        <label>Weight (kg)</label>
        <input type="number" id="weight" placeholder="70" min="1">
      </div>

      <div class="field">
        <label>Height (cm)</label>
        <input type="number" id="height" placeholder="175" min="1">
      </div>

      <div class="field full">
        <label>Age (years)</label>
        <input type="number" id="age" placeholder="30" min="1" max="120">
      </div>

      <div class="divider" style="grid-column:1/-1; margin:8px 0;"></div>

      <div class="field full">
        <label>Activity Level</label>
        <select id="activity">
          <option value="1.2">Sedentary — little or no exercise</option>
          <option value="1.375">Lightly Active — 1–3 days/week</option>
          <option value="1.55" selected>Moderately Active — 3–5 days/week</option>
          <option value="1.725">Very Active — 6–7 days/week</option>
          <option value="1.9">Extra Active — physical job + training</option>
        </select>
      </div>

      <div class="field full">
        <label>Goal Adjustment</label>
        <select id="goal">
          <option value="0">Maintain Weight — eat at TDEE</option>
          <option value="-300">Mild Weight Loss — TDEE − 300 kcal</option>
          <option value="-500">Weight Loss — TDEE − 500 kcal</option>
          <option value="300">Mild Weight Gain — TDEE + 300 kcal</option>
          <option value="500">Weight Gain — TDEE + 500 kcal</option>
        </select>
      </div>

    </div>

    <div style="margin-top:24px;">
      <button class="btn" onclick="calculate()">Calculate Results →</button>
    </div>
  </div>
</div>

<!-- Popup -->
<div class="overlay" id="overlay" onclick="closePopup(event)">
  <div class="popup" id="popup">
    <div class="popup-header">
      <div class="popup-avatar" id="popup-avatar">👤</div>
      <div class="popup-name" id="popup-name"></div>
      <div class="popup-subtitle" id="popup-subtitle"></div>
      <div id="bmi-badge" class="bmi-badge"></div>
    </div>

    <div class="stats-grid">
      <div class="stat-box bmr">
        <div class="stat-label">BMR</div>
        <div class="stat-value bmr-val" id="res-bmr">—</div>
        <div class="stat-unit">kcal/day (at rest)</div>
      </div>
      <div class="stat-box tdee">
        <div class="stat-label">TDEE</div>
        <div class="stat-value tdee-val" id="res-tdee">—</div>
        <div class="stat-unit">kcal/day (active)</div>
      </div>
      <div class="stat-box goal">
        <div class="stat-label">Daily Target</div>
        <div class="stat-value goal-val" id="res-goal">—</div>
        <div class="stat-unit" id="res-goal-label">kcal/day</div>
      </div>
    </div>

    <button class="close-btn" onclick="closePopup()">Close</button>
  </div>
</div>

<script>
  let gender = 'male';

  function selectGender(g) {
    gender = g;
    document.getElementById('btn-male').classList.toggle('active', g === 'male');
    document.getElementById('btn-female').classList.toggle('active', g === 'female');
  }

  function getBMIInfo(bmi) {
    if (bmi < 18.5) return { label: 'Underweight', color: '#79c0ff', bg: 'rgba(121,192,255,0.12)', border: 'rgba(121,192,255,0.3)' };
    if (bmi < 25)   return { label: 'Normal Weight', color: '#3fb950', bg: 'rgba(63,185,80,0.12)', border: 'rgba(63,185,80,0.3)' };
    if (bmi < 30)   return { label: 'Overweight', color: '#e3b341', bg: 'rgba(227,179,65,0.12)', border: 'rgba(227,179,65,0.3)' };
    if (bmi < 35)   return { label: 'Obese I  [30–35)', color: '#f0883e', bg: 'rgba(240,136,62,0.12)', border: 'rgba(240,136,62,0.3)' };
    if (bmi < 40)   return { label: 'Obese II  [35–40)', color: '#f85149', bg: 'rgba(248,81,73,0.12)', border: 'rgba(248,81,73,0.3)' };
    return           { label: 'Obese III  [40+]', color: '#ff7b72', bg: 'rgba(255,123,114,0.18)', border: 'rgba(255,123,114,0.4)' };
  }

  function calculate() {
    const name   = document.getElementById('name').value.trim() || 'Patient';
    const weight = parseFloat(document.getElementById('weight').value);
    const height = parseFloat(document.getElementById('height').value);
    const age    = parseFloat(document.getElementById('age').value);
    const actMul = parseFloat(document.getElementById('activity').value);
    const goalAdj= parseFloat(document.getElementById('goal').value);
    const goalSel= document.getElementById('goal');
    const goalText = goalSel.options[goalSel.selectedIndex].text;

    if (!weight || !height || !age) {
      alert('Please fill in Weight, Height, and Age.');
      return;
    }

    // BMI
    const heightM = height / 100;
    const bmi = weight / (heightM * heightM);

    // BMR — Mifflin-St Jeor
    const bmr = gender === 'male'
      ? (10 * weight) + (6.25 * height) - (5 * age) + 5
      : (10 * weight) + (6.25 * height) - (5 * age) - 161;

    const tdee   = bmr * actMul;
    const target = tdee + goalAdj;

    const bmiInfo = getBMIInfo(bmi);

    // Populate popup
    document.getElementById('popup-avatar').textContent = gender === 'male' ? '👨' : '👩';
    document.getElementById('popup-name').textContent = name;
    document.getElementById('popup-subtitle').textContent =
      `${gender === 'male' ? 'Male' : 'Female'} · ${age} yrs · ${weight} kg · ${height} cm`;

    const badge = document.getElementById('bmi-badge');
    badge.textContent = `BMI ${bmi.toFixed(1)} — ${bmiInfo.label}`;
    badge.style.color = bmiInfo.color;
    badge.style.background = bmiInfo.bg;
    badge.style.borderColor = bmiInfo.border;

    document.getElementById('res-bmr').textContent  = Math.round(bmr).toLocaleString();
    document.getElementById('res-tdee').textContent = Math.round(tdee).toLocaleString();
    document.getElementById('res-goal').textContent = Math.round(target).toLocaleString();
    document.getElementById('res-goal-label').textContent = goalText;

    document.getElementById('overlay').classList.add('show');
  }

  function closePopup(e) {
    if (!e || e.target === document.getElementById('overlay')) {
      document.getElementById('overlay').classList.remove('show');
    }
  }

  document.addEventListener('keydown', e => {
    if (e.key === 'Escape') document.getElementById('overlay').classList.remove('show');
  });
</script>

</body>
</html>
