<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Women Safety Website</title>
<style>
  * { box-sizing: border-box; }
  body {
    margin: 0;
    font-family: Candara, Arial, sans-serif;
    background-color: #f0f6fb;
    color: #222;
  }
  header {
    background: linear-gradient(90deg, #b8e8fc 0%, #e8f0fc 100%);
    color: #156087;
    padding: 30px 15px;
    text-align: center;
    font-weight: 700;
    font-size: 3.2rem;
    letter-spacing: 1.3px;
    box-shadow: 0 3px 10px rgba(18, 87, 130, 0.12);
  }
  #side-nav {
    position: fixed;
    top: 105px;
    left: 0;
    width: 200px;
    height: calc(100% - 105px);
    background-color: #e9f0fa;
    border-right: 1px solid #d3e0ef;
    padding: 20px 0;
    overflow-y: auto;
    box-shadow: 2px 0 6px rgba(24,95,174,0.04);
  }
  #side-nav ul { list-style: none; padding-left: 0; margin: 0; }
  #side-nav ul li { margin: 13px 0; text-align: center; }
  #side-nav ul li a {
    color: #156087;
    text-decoration: none;
    font-weight: 700;
    font-size: 16px;
    display: block;
    padding: 9px 0;
    border-radius: 6px;
    transition: background .3s, color .3s;
  }
  #side-nav ul li a:hover, #side-nav ul li a.active {
    background-color: #156087;
    color: #fff;
  }
  main {
    margin-left: 200px;
    padding: 32px 55px;
    max-width: 1200px;
    background-color: #fff;
    min-height: calc(100vh - 105px);
    margin-top: 105px;
  }
  main section {
    margin-bottom: 80px;
    border-bottom: 1px solid #dde6f4;
  }
  main section h1,
  main section h2,
  main section h3 {
    color: #156087;
    margin-bottom: 18px;
  }
  button {
    background-color: #156087;
    color: white;
    border: none;
    padding: 15px 34px;
    border-radius: 8px;
    font-size: 18px;
    cursor: pointer;
    font-weight: 600;
    transition: background .3s;
  }
  button:hover { background-color: #0f4260; }
  form {
    max-width: 490px;
  }
  form label {
    display: block;
    margin-bottom: 10px;
    font-weight: 700;
    font-size: 16px;
  }
  form input[type="text"],
  form input[type="email"],
  form input[type="password"],
  form textarea {
    width: 100%;
    padding: 13px;
    margin-bottom: 21px;
    border: 1px solid #b8c6db;
    border-radius: 8px;
    font-size: 15px;
    resize: vertical;
  }
  form textarea { height: 135px; }
  #route-map-img {
    display: block;
    margin: 18px auto 15px auto;
    width: 350px;
    max-width: 85%;
    height: auto;
    border-radius: 12px;
    box-shadow: 0 2px 8px rgba(24, 95, 174, 0.12);
    border: 2px solid #156087;
  }
  .feedback-container {
    display: flex;
    flex-wrap: wrap;
    gap: 22px;
  }
  .feedback-card {
    flex: 1 1 300px;
    border: 1px solid #dde6f4;
    border-radius: 10px;
    padding: 18px 25px;
    background-color: #fafbfc;
    box-shadow: 0 2px 6px rgba(24, 95, 174, 0.06);
  }
  .user-name { font-weight: 700; margin-bottom: 7px; font-size: 17px; }
  .user-email { font-size: 14px; color: #4580bc; margin-bottom: 14px; font-style: italic; }
  .stars { color: #facc15; font-size: 20px; }
  ul li { margin: 8px 0; }
  p { font-size: 16px; line-height: 1.5; }
</style>
</head>
<body>

<header>
  Women Safety
</header>

<aside id="side-nav">
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#about">About Us</a></li>
    <li><a href="#sos">SOS Alert</a></li>
    <li><a href="#voice">Voice Alert</a></li>
    <li><a href="#map">Safe Route Map</a></li>
    <li><a href="#community">Community</a></li>
    <li><a href="#tips">Safety Tips</a></li>
    <li><a href="#profile">User Profile</a></li>
    <li><a href="#register">Register</a></li>
    <li><a href="#login">Login</a></li>
    <li><a href="#faq">FAQ</a></li>
    <li><a href="#contact">Contact Us</a></li>
  </ul>
</aside>

<main>
  <section id="home">
    <h1>Welcome to Women Safety Portal</h1>
    <p>
      Women Safety Portal is an initiative dedicated to empowering women by providing them with easy access to safety tools, emergency alerts, and community support. We envision a world where every woman feels safe and confident, whether she is at home, at work, or traveling.
    </p>
    <p>
      Our platform offers cutting-edge technology powered by real-time location tracking, voice alerts, and community connectivity to create a safety net that women can rely on in moments of distress.
    </p>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p>
      Our mission is to create a safer environment for women everywhere by leveraging advanced technologies and fostering a supportive community. We believe that awareness, preparedness, and quick response can save lives.
    </p>
    <p>
      Women Safety Portal provides tools and information to increase women’s confidence and independence, while connecting them to emergency services and support networks immediately.
    </p>
    <p>
      We collaborate with local authorities, volunteers, and NGOs to ensure real help is available when needed.
    </p>
  </section>

  <section id="sos">
    <h2>SOS Alert</h2>
    <button onclick="sendSOS()">Send Emergency SOS Alert</button>
    <p>
      The SOS button allows you to send an immediate distress signal to your trusted contacts with your exact location. This feature is designed to alert your family, friends, or emergency services at the click of a button.
    </p>
    <p>
      When you press SOS in distress, your location is continuously shared and tracked until help arrives or the alert is cancelled.
    </p>
  </section>

  <section id="voice">
    <h2>Voice Alert</h2>
    <button onclick="recordAudio()">Record and Send Voice Alert</button>
    <p>
      Sometimes, speaking out can be hard. This voice alert feature lets you record an audio message clearly communicating your situation to your emergency contacts.
    </p>
    <p>
      Once recorded and sent, your contacts receive your message with your location for faster and better assistance.
    </p>
    <p id="audio-status"></p>
  </section>

  <section id="map">
    <h2>Safe Route Map</h2>
    <p>
      This map can be used as a reference for planning your travel routes through major cities. Always choose well-lit, populated roads and share your live location with trusted contacts while traveling. Our portal recommends sticking to main public routes and using community-verified safe zones especially during night hours.
    </p>
    <img src="https://upload.wikimedia.org/wikipedia/commons/8/83/National_Highway_3_%28India%29.png" alt="Route Map Reference" id="route-map-img">
  </section>

  <section id="community">
    <h2>Community Support</h2>
    <p>
      Our active community connects women with local volunteers, police stations, and NGOs for real-time aid and information.
    </p>
    <ul>
      <li>Volunteer contact networks available 24/7</li>
      <li>Alerts from local police and emergency units</li>
      <li>Access to women’s help centers and counseling services</li>
      <li>Community forums for sharing experiences and tips</li>
    </ul>
  </section>

  <section id="tips">
    <h2>Safety Tips</h2>
    <ul>
      <li>Always inform a trusted person about your whereabouts.</li>
      <li>Avoid isolated or poorly-lit places, especially at night.</li>
      <li>Keep whistle or pepper spray handy for self-defense.</li>
      <li>Stay alert and trust your instincts about suspicious behavior.</li>
      <li>Keep your cellphone charged and emergency numbers saved.</li>
      <li>Learn basic self-defense moves as precaution.</li>
    </ul>
  </section>

  <section id="profile">
    <h2>User Profile</h2>
    <p>Name: <span id="user-name-display">Anita Singh</span></p>
    <p>Email: <span id="user-email-display">anita.singh@example.com</span></p>
    <button onclick="updateProfile()">Update Profile</button>
    <h3>What Our Users Say</h3>
    <div class="feedback-container">
      <div class="feedback-card">
        <p class="user-name">Seema Patel</p>
        <p class="user-email">seema.patel@email.com</p>
        <p>The SOS alert feature saved my life once. I felt truly safe using this app.</p>
        <p class="stars">★★★★★</p>
      </div>
      <div class="feedback-card">
        <p class="user-name">Ritika Sharma</p>
        <p class="user-email">ritika.sharma@email.com</p>
        <p>The community support helped me network with brave volunteers and get assistance when needed.</p>
        <p class="stars">★★★★☆</p>
      </div>
      <div class="feedback-card">
        <p class="user-name">Meera Joshi</p>
        <p class="user-email">meera.joshi@email.com</p>
        <p>The safety tips really help me stay aware and careful during my travels.</p>
        <p class="stars">★★★★★</p>
      </div>
    </div>
  </section>

  <section id="register">
    <h2>Register</h2>
    <form id="register-form" onsubmit="return registerUser()">
      <label for="reg-name">Name:</label>
      <input type="text" id="reg-name" name="reg-name" required />
      <label for="reg-email">Email:</label>
      <input type="email" id="reg-email" name="reg-email" required />
      <label for="reg-password">Password:</label>
      <input type="password" id="reg-password" name="reg-password" required />
      <button type="submit">Register</button>
    </form>
    <p id="register-msg"></p>
  </section>

  <section id="login">
    <h2>Login</h2>
    <form id="login-form" onsubmit="return loginUser()">
      <label for="login-email">Email:</label>
      <input type="email" id="login-email" name="login-email" required />
      <label for="login-password">Password:</label>
      <input type="password" id="login-password" name="login-password" required />
      <button type="submit">Login</button>
    </form>
    <p id="login-msg"></p>
  </section>

  <section id="faq">
    <h2>Frequently Asked Questions</h2>
    <ul>
      <li><strong>What if I accidentally press the SOS button?</strong>
        <p>You can cancel the alert within 10 seconds to avoid false alarms.</p></li>
      <li><strong>How is my voice alert sent?</strong>
        <p>The voice recording is securely transmitted alongside your location to your emergency contacts.</p></li>
      <li><strong>Is my location shared all the time?</strong>
        <p>Location sharing only happens during active emergencies or when you choose to share it.</p></li>
    </ul>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <form id="contact-form" onsubmit="return sendContactForm()">
      <label for="contact-name">Name:</label>
      <input type="text" id="contact-name" required />
      <label for="contact-email">Email:</label>
      <input type="email" id="contact-email" required />
      <label for="contact-message">Message:</label>
      <textarea id="contact-message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
    <p id="contact-msg"></p>
  </section>
</main>

<script>
  document.addEventListener("DOMContentLoaded", () => {
    const navLinks = document.querySelectorAll('#side-nav a');
    function clearActive() { navLinks.forEach(link => link.classList.remove('active')); }
    function onScroll() {
      let current = '';
      document.querySelectorAll('main section').forEach(section => {
        const sectionTop = section.offsetTop - 80;
        if (window.scrollY >= sectionTop) current = section.getAttribute('id');
      });
      if(current) {
        clearActive();
        navLinks.forEach(link => {
          if(link.getAttribute('href') === `#${current}`) link.classList.add('active');
        });
      }
    }
    window.addEventListener('scroll', onScroll);
    navLinks.forEach(link => {
      link.addEventListener('click', e => {
        e.preventDefault();
        let targetId = link.getAttribute('href').slice(1);
        document.getElementById(targetId).scrollIntoView({behavior: 'smooth'});
      });
    });
  });

  function sendSOS() { alert('Emergency SOS alert sent to contacts!'); }
  function recordAudio() { document.getElementById('audio-status').textContent = 'Audio alert recorded and sent successfully!'; }
  function updateProfile() { alert('Profile update feature coming soon!'); }
  function registerUser() {
    document.getElementById('register-msg').textContent = "Registration successful! You can now log in.";
    return false;
  }
  function loginUser() {
    document.getElementById('login-msg').textContent = "Login successful! Welcome back.";
    return false;
  }
  function sendContactForm() {
    document.getElementById('contact-msg').textContent = "Thank you for contacting us. We will get back to you shortly.";
    return false;
  }
</script>
</body>
</html>
