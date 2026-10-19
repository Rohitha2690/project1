<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TechNova Fest 2026</title>
</head>
<style>
    
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
    scroll-behavior: smooth;
}

body {
    background: #f5f7ff;
    color: #102044;
}

/* Navigation */
header {
    background: #030e2d;
    color: white;
    padding: 15px 6%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
}

.logo h2 {
    color: #ff4bc1;
}

.logo p {
    font-size: 12px;
    margin-top: 5px;
}

nav {
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
}

nav a {
    color: white;
    text-decoration: none;
    font-size: 13px;
}

nav a:hover {
    color: #ff4bc1;
}

.register-btn,
.explore-btn {
    background: linear-gradient(90deg, #e72bb4, #5548ff);
    color: white;
    padding: 12px 20px;
    border-radius: 25px;
    text-decoration: none;
    display: inline-block;
}

/* Hero Section */
.hero {
    min-height: 300px;
    padding: 45px 7%;
    color: white;
    display: flex;
    align-items: center;
    background:
        linear-gradient(90deg, #030b25 10%, #10144799 55%, #050b2999),
        url("https://images.unsplash.com/photo-1459749411175-04bf5292ceea?auto=format&fit=crop&w=1600&q=80");
    background-size: cover;
    background-position: center;
}

.tagline {
    color: #ff58d0;
    font-style: italic;
    margin-bottom: 10px;
}

.hero h1 {
    font-size: clamp(30px, 5vw, 48px);
    margin-bottom: 10px;
}

.hero h1 span {
    color: #e65bdf;
}

.hero h2 {
    color: #55e7f0;
    margin-bottom: 22px;
}

.hero-content > p:not(.tagline) {
    margin-bottom: 22px;
    line-height: 1.8;
    font-size: 14px;
}

/* Common Sections */
.section {
    padding: 30px 7%;
}

.small-title {
    color: #df2cae;
    font-size: 12px;
    font-weight: bold;
    margin-bottom: 5px;
}

.events > h2,
.form-section > h2 {
    font-size: 28px;
    margin-bottom: 8px;
}

.events > p:not(.small-title),
.form-section > p {
    font-size: 13px;
    line-height: 1.6;
}

/* Event Cards */
.event-container {
    display: grid;
    grid-template-columns: repeat(6, minmax(0, 1fr));
    gap: 15px;
    margin-top: 22px;
}

.event-card {
    background: white;
    border-radius: 10px;
    overflow: hidden;
    border: 1px solid #e1e5f0;
    padding-bottom: 14px;
    box-shadow: 0 3px 10px #14224a0b;
    transition: transform 0.3s;
}

.event-card:hover {
    transform: translateY(-5px);
}

.event-image {
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 45px;
}

.code {
    background: linear-gradient(135deg, #061b49, #13b5d9);
}

.art {
    background: linear-gradient(135deg, #ff9cbf, #ffcf63);
}

.singing {
    background: linear-gradient(135deg, #00b5be, #6b3be9);
}

.gaming {
    background: linear-gradient(135deg, #061a40, #008bff);
}

.quiz {
    background: linear-gradient(135deg, #5800ce, #dd43ff);
}

.rangoli {
    background: linear-gradient(135deg, #ff7028, #ffc342);
}

.event-card h3 {
    font-size: 14px;
    margin: 12px 10px 8px;
}

.event-card p {
    font-size: 11px;
    line-height: 1.6;
    margin: 0 10px 12px;
    color: #435575;
}

.technical,
.cultural {
    display: inline-block;
    margin-left: 10px;
    padding: 5px 10px;
    border-radius: 15px;
    font-size: 10px;
    font-weight: bold;
}

.technical {
    color: #1450c9;
    background: #dceaff;
}

.cultural {
    color: #d52283;
    background: #ffe0f0;
}

/* Schedule and About */
.details {
    display: grid;
    grid-template-columns: 1fr 1.1fr;
    gap: 20px;
    padding: 0 7% 30px;
}

.schedule-box,
.about-box {
    border-radius: 10px;
    overflow: hidden;
}

.schedule-box {
    background: #edf0ff;
    padding: 20px;
}

.schedule-box h2,
.about-box h2 {
    font-size: 20px;
    margin-bottom: 10px;
}

.schedule-box > p {
    font-size: 12px;
    margin-bottom: 15px;
}

table {
    width: 100%;
    border-collapse: collapse;
    background: white;
    font-size: 12px;
}

th,
td {
    border: 1px solid #e0e5f0;
    padding: 12px;
    text-align: left;
    line-height: 1.8;
}

th {
    background: #f8f9ff;
}

td:first-child {
    text-align: center;
    color: #e42a9f;
    font-weight: bold;
}

.note {
    color: #60739a;
    font-size: 11px !important;
    margin-top: 12px;
}

/* About */
.about-box {
    background: linear-gradient(135deg, #061334, #102d6c);
    color: white;
    padding: 22px;
}

.about-box > p {
    font-size: 13px;
    line-height: 1.7;
}

.stats {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    text-align: center;
    margin: 20px 0;
    gap: 8px;
}

.stats > div {
    border-right: 1px solid #6a7da5;
}

.stats > div:last-child {
    border-right: none;
}

.stats h2 {
    font-size: 25px;
}

.stats h3 {
    font-size: 17px;
}

.stats p {
    font-size: 11px;
    margin-top: 4px;
}

.memory {
    background:
        linear-gradient(#070d3055, #070d3055),
        url("https://images.unsplash.com/photo-1470229722913-7c0e2dbbafd3?auto=format&fit=crop&w=1000&q=80");
    background-size: cover;
    background-position: center;
    padding: 30px 15px;
    text-align: right;
    font-size: 22px;
    font-style: italic;
    font-weight: bold;
    color: white;
    min-height: 120px;
}

/* Registration */
.registration {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 30px;
    align-items: center;
    background: #f8f8ff;
}

.form-section > p {
    margin-bottom: 15px;
}

.form-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 16px;
}

.form-grid label {
    display: block;
    font-size: 12px;
    font-weight: bold;
    margin-bottom: 7px;
}

input,
select {
    width: 100%;
    padding: 12px;
    border: 1px solid #d5dced;
    border-radius: 6px;
    background: white;
    color: #263858;
    font-size: 12px;
    outline: none;
}

input:focus,
select:focus {
    border-color: #784bff;
}

.form-grid button {
    align-self: end;
    border: none;
    padding: 14px;
    color: white;
    font-size: 13px;
    font-weight: bold;
    border-radius: 7px;
    cursor: pointer;
    background: linear-gradient(90deg, #a522ef, #318bff);
}

.form-grid button:hover {
    opacity: 0.85;
}

.registration-art {
    background: linear-gradient(135deg, #6b35ef, #e942bf);
    padding: 35px 15px;
    border-radius: 50% 40% 45% 35%;
    color: white;
    text-align: center;
    transform: rotate(-3deg);
}

.registration-art h2 {
    font-size: 25px;
    font-style: italic;
    line-height: 1.5;
}

.registration-art p {
    margin-top: 20px;
    font-size: 25px;
}

/* Contact */
.contact {
    display: grid;
    grid-template-columns: 1.5fr 1fr 1fr 1fr;
    align-items: center;
    gap: 20px;
    background: #03132f;
    color: white;
    padding: 30px 7%;
}

.contact h2 {
    margin-bottom: 8px;
}

.contact h3 {
    color: #ff52c8;
    font-size: 13px;
    margin-bottom: 8px;
}

.contact p {
    font-size: 11px;
    line-height: 1.7;
}

/* Footer */
footer {
    background: #020b22;
    color: white;
    padding: 25px 7%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 15px;
    flex-wrap: wrap;
}

footer h3 {
    color: #ff50c8;
    margin-bottom: 5px;
}

footer p {
    font-size: 11px;
    line-height: 1.7;
}

/* Responsive Design */
@media (max-width: 1000px) {
    .event-container {
        grid-template-columns: repeat(3, 1fr);
    }

    header {
        justify-content: center;
    }

    .details {
        grid-template-columns: 1fr 1fr;
    }
}

@media (max-width: 650px) {
    header {
        flex-direction: column;
        text-align: center;
    }

    nav {
        justify-content: center;
        gap: 12px;
    }

    .hero {
        padding: 35px 5%;
    }

    .hero-content > p:not(.tagline) {
        font-size: 12px;
    }

    .event-container {
        grid-template-columns: repeat(2, 1fr);
    }

    .details,
    .registration {
        grid-template-columns: 1fr;
        padding-left: 5%;
        padding-right: 5%;
    }

    .form-grid {
        grid-template-columns: 1fr;
    }

    .registration-art {
        max-width: 300px;
        margin: 10px auto;
    }

    .contact {
        grid-template-columns: 1fr 1fr;
    }

    footer {
        flex-direction: column;
        text-align: center;
    }
}

@media (max-width: 380px) {
    .event-container {
        grid-template-columns: 1fr;
    }

    .stats {
        grid-template-columns: repeat(2, 1fr);
        gap: 15px;
    }

    .stats > div {
        border-right: none;
    }
}

</style>
<body>

    <!-- Navigation -->
    <header>
        <div class="logo">
            <h2>🎉 TechNova Fest</h2>
            <p>Learn | Compete | Celebrate</p>
        </div>

        <nav>
            <a href="#home">Home</a>
            <a href="#events">Events</a>
            <a href="#schedule">Schedule</a>
            <a href="#about">About</a>
            <a href="#registration">Registration</a>
            <a href="#contact">Contact</a>
        </nav>

        <a href="#registration" class="register-btn">Register Now</a>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <p class="tagline">Annual College Fest</p>
            <h1>TechNova Fest <span>2026</span></h1>
            <h2>Learn | Compete | Celebrate</h2>

            <p>📅 15 - 17 March 2026
                &nbsp; 📍 College Campus
                &nbsp; 👥 All Students Welcome
            </p>

            <a href="#events" class="explore-btn">Explore Events →</a>
        </div>
    </section>

    <!-- Featured Events -->
    <section class="events section" id="events">
        <p class="small-title">OUR EVENTS</p>
        <h2>Featured Events</h2>
        <p>Showcase your talent, skills and creativity in exciting events.</p>

        <div class="event-container">

            <div class="event-card">
                <div class="event-image code">💻</div>
                <h3>Code Sprint</h3>
                <p>Test your coding skills and solve real-world problems.</p>
                <span class="technical">Technical</span>
            </div>

            <div class="event-card">
                <div class="event-image art">🎨</div>
                <h3>Art Attack</h3>
                <p>Unleash your creativity with your artistic skills.</p>
                <span class="cultural">Cultural</span>
            </div>

            <div class="event-card">
                <div class="event-image singing">🎤</div>
                <h3>Singing Star</h3>
                <p>Let your voice be heard and mesmerize the audience.</p>
                <span class="cultural">Cultural</span>
            </div>

            <div class="event-card">
                <div class="event-image gaming">🎮</div>
                <h3>Gaming Zone</h3>
                <p>Play, compete and become the ultimate gamer.</p>
                <span class="technical">Technical</span>
            </div>

            <div class="event-card">
                <div class="event-image quiz">💡</div>
                <h3>Business Quiz</h3>
                <p>Think, analyze and win exciting prizes.</p>
                <span class="technical">Technical</span>
            </div>

            <div class="event-card">
                <div class="event-image rangoli">🌸</div>
                <h3>Rangoli</h3>
                <p>Turn colors into art and make your creativity shine.</p>
                <span class="cultural">Cultural</span>
            </div>

        </div>
    </section>

    <!-- Schedule and About -->
    <section class="details">

        <div class="schedule-box" id="schedule">
            <h2>📅 EVENT SCHEDULE</h2>
            <p>Plan your fest experience with our detailed schedule.</p>

            <table>
                <tr>
                    <th>Date</th>
                    <th>Events</th>
                </tr>
                <tr>
                    <td><strong>15</strong><br>Mar 2026</td>
                    <td>
                        • Inauguration<br>
                        • Code Sprint<br>
                        • Singing Star
                    </td>
                </tr>
                <tr>
                    <td><strong>16</strong><br>Mar 2026</td>
                    <td>
                        • Art Attack<br>
                        • Gaming Zone<br>
                        • Business Quiz
                    </td>
                </tr>
                <tr>
                    <td><strong>17</strong><br>Mar 2026</td>
                    <td>
                        • Rangoli<br>
                        • Prize Distribution<br>
                        • Cultural Evening
                    </td>
                </tr>
            </table>

            <p class="note">◷ Full schedule with timings will be available after registration.</p>
        </div>

        <div class="about-box" id="about">
            <h2>🎉 About the Fest</h2>
            <p>
                TechNova Fest is the annual college festival organized
                by students to bring out the best in talent, creativity
                and innovation. It is a platform where you can showcase
                your skills, make new friends and create unforgettable
                memories.
            </p>

            <div class="stats">
                <div><h2>⭐</h2><h3>50+</h3><p>Events</p></div>
                <div><h2>👥</h2><h3>1000+</h3><p>Participants</p></div>
                <div><h2>🏆</h2><h3>Exciting</h3><p>Prizes</p></div>
                <div><h2>💗</h2><h3>Fun</h3><p>Friendship</p></div>
            </div>

            <div class="memory">
                Good Vibes<br>Great Memories!
            </div>
        </div>

    </section>

    <!-- Registration -->
    <section class="registration section" id="registration">
        <div class="form-section">
            <p class="small-title">JOIN THE FEST</p>
            <h2>Register Now</h2>
            <p>Fill in the form to participate in the fest.</p>

            <form>
                <div class="form-grid">
                    <div>
                        <label>Full Name *</label>
                        <input type="text" placeholder="Enter your full name" required>
                    </div>

                    <div>
                        <label>Roll Number *</label>
                        <input type="text" placeholder="Enter your roll number" required>
                    </div>

                    <div>
                        <label>Email Address *</label>
                        <input type="email" placeholder="Enter your email address" required>
                    </div>

                    <div>
                        <label>Department *</label>
                        <select required>
                            <option value="">Select Department</option>
                            <option>CSE</option>
                            <option>ECE</option>
                            <option>EEE</option>
                            <option>Mechanical</option>
                            <option>Civil</option>
                        </select>
                    </div>

                    <div>
                        <label>Choose an Event *</label>
                        <select required>
                            <option value="">Select an Event</option>
                            <option>Code Sprint</option>
                            <option>Art Attack</option>
                            <option>Singing Star</option>
                            <option>Gaming Zone</option>
                            <option>Business Quiz</option>
                            <option>Rangoli</option>
                        </select>
                    </div>

                    <button type="submit">Submit Registration →</button>
                </div>
            </form>

            <p class="note">ℹ Note: This is a front-end demonstration.
                Actual registration requires a backend.
            </p>
        </div>

        <div class="registration-art">
            <h2>Be Part of<br>Something<br>Amazing!</h2>
            <p>🙌 🎉 🙌 🎉 🙌</p>
        </div>
    </section>

    <!-- Contact -->
    <section class="contact" id="contact">
        <div>
            <p class="small-title">GET IN TOUCH</p>
            <h2>Contact Us</h2>
            <p>Have questions? Feel free to reach out to us.</p>
        </div>

        <div>
            <h3>✉ Email</h3>
            <p>technovafest@example.com</p>
        </div>

        <div>
            <h3>📍 Location</h3>
            <p>College Campus</p>
        </div>

        <div>
            <h3>📞 Phone</h3>
            <p>+91 98765 43210</p>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div>
            <h3>🎉 TechNova Fest</h3>
            <p>Learn | Compete | Celebrate</p>
        </div>

        <p>Home &nbsp; | &nbsp; Events &nbsp; | &nbsp;
            Schedule &nbsp; | &nbsp; About &nbsp; | &nbsp; Contact
        </p>

        <p>© 2026 TechNova Fest. All rights reserved.</p>
    </footer>

</body>
</html>

