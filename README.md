<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Project KALIKASAN</title>
<style>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
  }
  /* Menu Bar */
  .menu {
    background-color: #2e8b57;
    overflow: hidden;
    text-align: center;
  }
  .menu button {
    background-color: #2e8b57;
    color: white;
    border: none;
    padding: 15px 25px;
    cursor: pointer;
    font-size: 16px;
    margin: 0 5px;
    transition: 0.3s;
    border-radius: 5px;
  }
  .menu button:hover {
    background-color: #45a049;
  }
  /* Sections */
  .section {
    display: none; /* Hidden by default */
    padding: 20px;
  }
  .active {
    display: block;
  }
</style>
</head>
<body>

<!-- Menu Bar -->
<div class="menu">
  <button onclick="showSection('description')">Description</button>
  <button onclick="showSection('oop')">OOP Concepts</button>
  <button onclick="showSection('structure')">Program Structure</button>
  <button onclick="showSection('team')">Team</button>
</div>

<!-- Sections -->
<div id="description" class="section">
  <h2>📌 Project Description</h2>
  <p><strong>Project KALIKASAN: Tracing Plastic Waste Reduction</strong> is a Java-based program designed to track and record each user’s plastic waste reduction activities. Users can input daily plastic usage and recycling habits, and the system stores progress securely. Reports show the amount of plastic reduced over time.</p>
</div>

<div id="oop" class="section">
  <h2>🧩 OOP Concepts Applied</h2>
  <ul>
    <li><strong>Encapsulation</strong> – Protects sensitive data via getters/setters.</li>
    <li><strong>Inheritance</strong> – Reusable classes for scalable code.</li>
    <li><strong>Polymorphism</strong> – Methods adapt based on object type.</li>
    <li><strong>Abstraction</strong> – Breaks complex processes into simpler functions.</li>
  </ul>
</div>

<div id="structure" class="section">
  <h2>🛠️ Program Structure</h2>
  <ul>
    <li><strong>User</strong> – Stores user info and progress data.</li>
    <li><strong>PlasticTracker</strong> – Handles calculations and updates.</li>
    <li><strong>FileHandler</strong> – Reads and writes user data securely.</li>
    <li><strong>ReportGenerator</strong> – Generates readable reports.</li>
  </ul>
</div>

<div id="team" class="section">
  <h2>🌿 Team EcoTrio</h2>
  <ul>
    <li>Caringal, Lance Arnie A.</li>
    <li>Quiñones, Ashley D.</li>
    <li>Mendoza, Baby Gwen A.</li>
  </ul>
</div>

<script>
  // Function to show the selected section and hide others
  function showSection(sectionId) {
    const sections = document.querySelectorAll('.section');
    sections.forEach(sec => sec.classList.remove('active'));
    document.getElementById(sectionId).classList.add('active');
  }
</script>

</body>
</html>
