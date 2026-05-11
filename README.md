<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>OrdosDB - MPP Database with AI Capabilities</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Inter', sans-serif;
}

body {
    background: radial-gradient(circle at top, #06281f, #020c0a);
    color: white;
    overflow-x: hidden;
}

/* Green glow */
.bg-glow {
    position: fixed;
    width: 900px;
    height: 900px;
    background: radial-gradient(circle, rgba(34,197,94,0.25), transparent 60%);
    top: -250px;
    left: -250px;
    filter: blur(70px);
}

/* Header */
header {
    position: fixed;
    top: 0;
    width: 100%;
    padding: 18px 60px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: rgba(2, 10, 8, 0.6);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid rgba(34,197,94,0.15);
    z-index: 1000;
}

.logo {
    display: flex;
    align-items: center;
    gap: 10px;
}

.logo img {
    width: 250px;
    height: 60px;
    border-radius: 8px;
}

.logo span {
    font-weight: 700;
    color: #22c55e;
    letter-spacing: 0.5px;
}

nav a {
    margin-left: 24px;
    text-decoration: none;
    color: #a7f3d0;
    font-size: 14px;
    transition: 0.3s;
}

nav a:hover {
    color: #34d399;
}

/* Hero */
.hero {
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 0 20px;
}

.hero-box {
    max-width: 900px;
}

.badge {
    display: inline-block;
    padding: 6px 12px;
    background: rgba(34,197,94,0.1);
    border: 1px solid rgba(34,197,94,0.3);
    border-radius: 20px;
    font-size: 20px;
    color: #86efac;
    margin-bottom: 20px;
}

.hero h1 {
    font-size: 64px;
    font-weight: 700;
    background: linear-gradient(90deg, #22c55e, #10b981);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.hero p {
    margin-top: 18px;
    font-size: 18px;
    color: #a7f3d0;
    line-height: 1.6;
}

.cta {
    margin-top: 35px;
}

.btn {
    padding: 12px 26px;
    background: linear-gradient(90deg, #22c55e, #16a34a);
    border: none;
    border-radius: 10px;
    color: white;
    cursor: pointer;
    font-weight: 600;
    transition: 0.3s;
}

.btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 30px rgba(34,197,94,0.25);
}

.btn-secondary {
    margin-left: 12px;
    padding: 12px 26px;
    border: 1px solid rgba(34,197,94,0.3);
    background: transparent;
    color: #a7f3d0;
    border-radius: 10px;
}

/* Section */
section {
    padding: 100px 60px;
}

.section-title {
    text-align: center;
    font-size: 34px;
    margin-bottom: 50px;
    color: #dcfce7;
}

/* Grid */
.grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}

.card {
    background: rgba(255,255,255,0.03);
    border: 1px solid rgba(34,197,94,0.15);
    border-radius: 16px;
    padding: 26px;
    backdrop-filter: blur(10px);
    transition: 0.3s;
}

.card:hover {
    transform: translateY(-8px);
    border-color: rgba(34,197,94,0.5);
    box-shadow: 0 20px 40px rgba(0,0,0,0.4);
}

.card h3 {
    color: #22c55e;
    margin-bottom: 10px;
}

.card p {
    color: #a7f3d0;
    font-size: 14px;
}

/* Footer */
footer {
    text-align: center;
    padding: 50px;
    color: #6ee7b7;
    border-top: 1px solid rgba(34,197,94,0.1);
}

/* Responsive */
@media (max-width: 900px) {
    .grid {
        grid-template-columns: 1fr;
    }

    header {
        padding: 15px 20px;
    }

    section {
        padding: 80px 20px;
    }

    .hero h1 {
        font-size: 42px;
    }
}

#bgCanvas {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 0;
    pointer-events: none;
    opacity: 0.85;
}
</style>
</head>

<body>

<canvas id="bgCanvas"></canvas>


<div class="bg-glow"></div>

<header>
    <div class="logo">
        <img src="./ordosdb_logo_h.png" />
        <span></span>
    </div>

    <nav>
        <a href="#">Product</a>
        <a href="#">Architecture</a>
        <a href="#">Docs</a>
        <a href="#">About OrdosDB</a>
    </nav>
</header>

<section class="hero">
    <div class="hero-box">
        <div class="badge">AI-Empowered Massive Parallel Processing(MPP) Database</div>

        <h1>OrdosDB</h1>

        <p>
            Hybrid MPP Database with AI Capabilities.
        </p>

        <div class="cta">
            <button class="btn">Start OrdosDB</button>
            <button class="btn">View Docs</button>
        </div>
    </div>
</section>

<section>
    <h2 class="section-title">OrdosDB Core Capabilities</h2>

    <div class="grid">
	
		<div class="card">
            <h3>LLM as First Class Citizen as Relation</h3>
            <p>You can Build LLM Relation on Top of LLMs.</p>
        </div>
		
        <div class="card">
            <h3>SQL Extensions for LLM</h3>
            <p>LLM related Operations now Embedded into SQL Language.</p>
        </div>
		
		 <div class="card">
            <h3>LLM Analytics inside MPP Database</h3>
            <p>AI-Native Analytics Functions in Database.</p>
        </div>
		
		<div class="card">
            <h3>Developer Friendly</h3>
            <p>SQL + Open API.</p>
        </div>

        <div class="card">
            <h3>On-Premise LLM</h3>
            <p>Enterprise Data Assets for Local LLM.</p>
        </div>

      
        <div class="card">
            <h3>OrdosDB Super Appliance</h3>
            <p>MPP and LLM Integrated Release and Installation.</p>
        </div>


    </div>
</section>

<!-- Footer -->
<footer>

    <div style="display:flex; flex-direction:column; align-items:center; gap:22px;">

        <!-- Copyright -->
        <div style="color:#6ee7b7; font-size:14px;">
            © 2026 OrdosDB. All rights reserved.
        </div>

        <!-- Contact Email -->
        <div style="color:#a7f3d0; font-size:14px;">
            Email: <a href="mailto:ordosdb @ ordosdb.com.cn" style="color:#22c55e; text-decoration:none;">
                ordosdb @ ordosdb.com.cn
            </a>
        </div>

        <!-- Social + QR -->
        <div style="display:flex; gap:40px; flex-wrap:wrap; justify-content:center; align-items:center;">

            <!-- WeChat -->
            <div style="text-align:center;">
                <img src="./ordosdb_qrcode.jpg"
                     style="border-radius:12px; border:1px solid rgba(34,197,94,0.3); width: 100px; height: 100px;">
                <div style="margin-top:6px; font-size:12px; color:#a7f3d0;">
                    WeChat
                </div>
            </div>

            <!-- LinkedIn -->
            <a href="https://www.linkedin.com/groups/20710026/" target="_blank"
               style="color:#a7f3d0; text-decoration:none;">
                LinkedIn
            </a>

            <!-- Twitter -->
            <a href="https://twitter.com" target="_blank"
               style="color:#a7f3d0; text-decoration:none;">
                Twitter (X)
            </a>

        </div>

    </div>

</footer>
<script>
const canvas = document.getElementById("bgCanvas");
const ctx = canvas.getContext("2d");

let w = canvas.width = window.innerWidth;
let h = canvas.height = window.innerHeight;

window.addEventListener("resize", () => {
    w = canvas.width = window.innerWidth;
    h = canvas.height = window.innerHeight;
});

const particles = [];
const count = 85;

// init particles
for (let i = 0; i < count; i++) {
    particles.push({
        x: Math.random() * w,
        y: Math.random() * h,
        vx: (Math.random() - 0.5) * 0.6,
        vy: (Math.random() - 0.5) * 0.6
    });
}

function draw() {
    ctx.clearRect(0, 0, w, h);

    // green AI glow background layer
    const gradient = ctx.createRadialGradient(w/2, h/2, 0, w/2, h/2, w);
    gradient.addColorStop(0, "rgba(34,197,94,0.08)");
    gradient.addColorStop(1, "rgba(0,0,0,0)");

    ctx.fillStyle = gradient;
    ctx.fillRect(0, 0, w, h);

    for (let i = 0; i < particles.length; i++) {
        let p = particles[i];

        p.x += p.vx;
        p.y += p.vy;

        if (p.x < 0 || p.x > w) p.vx *= -1;
        if (p.y < 0 || p.y > h) p.vy *= -1;

        // node
        ctx.beginPath();
        ctx.fillStyle = "rgba(34,197,94,0.75)";
        ctx.arc(p.x, p.y, 2, 0, Math.PI * 2);
        ctx.fill();

        // connections (data flow)
        for (let j = i + 1; j < particles.length; j++) {
            let p2 = particles[j];
            let d = Math.hypot(p.x - p2.x, p.y - p2.y);

            if (d < 130) {
                ctx.strokeStyle = "rgba(34,197,94,0.12)";
                ctx.lineWidth = 1;
                ctx.beginPath();
                ctx.moveTo(p.x, p.y);
                ctx.lineTo(p2.x, p2.y);
                ctx.stroke();
            }
        }
    }

    requestAnimationFrame(draw);
}

draw();
</script>
</body>
</html>
