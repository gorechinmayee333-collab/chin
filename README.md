<!DOCTYPE html>
<html lang="en" class="m-0 p-0 overflow-x-hidden">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
    <title>Chinmayee Gore | Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        
        :root {
            --netflix-red: #E50914;
            --dark-bg: #141414;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--dark-bg);
            color: white;
            scroll-behavior: smooth;
            width: 100%;
            overflow-x: hidden;
        }

        /* Forced Edge-to-Edge Layout */
        .edge-to-edge {
            width: 100vw;
            max-width: 100%;
            position: relative;
            left: 50%;
            right: 50%;
            margin-left: -50vw;
            margin-right: -50vw;
            padding-left: 5%;
            padding-right: 5%;
        }

        .scroll-row::-webkit-scrollbar { display: none; }
        .scroll-row { 
            -ms-overflow-style: none; 
            scrollbar-width: none; 
            display: flex;
            overflow-x: auto;
            gap: 1rem;
            padding: 20px 0 40px 0;
            width: 100%;
        }

        .featured-banner {
            background-image: linear-gradient(to right, rgba(20,20,20,1) 0%, rgba(20,20,20,0.2) 60%, rgba(20,20,20,1) 100%), url('https://iili.io/fR2Ym92.jpg');
            background-size: cover;
            background-position: center;
            height: 90vh;
            width: 100vw;
            display: flex;
            align-items: center;
            padding-left: 5%;
        }

        /* Card Styles */
        .card-item-container {
            transition: transform .3s ease;
            cursor: pointer;
            width: 260px;
            height: 340px;
            flex-shrink: 0;
            position: relative;
            perspective: 1000px;
        }

        .card-item-container:hover { transform: scale(1.05); z-index: 50; }
        
        .flip-inner {
            position: relative;
            width: 100%;
            height: 100%;
            transition: transform 0.6s;
            transform-style: preserve-3d;
            border-radius: 4px;
        }

        .card-item-container:hover .flip-inner { transform: rotateY(180deg); }
        
        .flip-front, .flip-back {
            position: absolute;
            width: 100%;
            height: 100%;
            backface-visibility: hidden;
            border-radius: 4px;
            overflow: hidden;
        }

        .flip-back {
            background: #1a1a1a;
            transform: rotateY(180deg);
            display: flex;
            flex-direction: column;
            padding: 20px;
            border: 2px solid var(--netflix-red);
        }

        .mini-skill-btn { 
            padding: 10px 18px; 
            margin: 5px; 
            border-radius: 2px; 
            font-size: 12px; 
            background: #262626; 
            color: #fff; 
            border: 1px solid #444; 
            cursor: pointer; 
            transition: 0.2s; 
            text-transform: uppercase;
            font-weight: 700;
        }
        .mini-skill-btn.active { background: var(--netflix-red); border-color: white; }

        .utility-card {
            background-color: #222;
            border: 1px solid #333;
        }

        /* Full Width Utility for Section Headers */
        .section-header {
            padding-left: 5%;
            width: 100%;
            margin-bottom: 1.5rem;
        }
    </style>
</head>
<body class="antialiased">
    <header class="fixed top-0 w-full z-50 bg-black/90 border-b border-white/5">
        <nav class="flex items-center justify-between px-[5%] py-4">
            <h1 class="text-2xl font-black text-red-600 tracking-tighter">CHINMAYEE</h1>
            <div class="flex items-center space-x-6">
                <ul class="hidden lg:flex space-x-6 text-[10px] font-bold uppercase tracking-widest text-gray-400">
                    <li><a href="#experience" class="hover:text-white transition">Experience</a></li>
                    <li><a href="#internship" class="hover:text-white transition">Internships</a></li>
                    <li><a href="#academics" class="hover:text-white transition">Academics</a></li>
                    <li><a href="#recognitions" class="hover:text-white transition">Honors</a></li>
                </ul>
            </div>
        </nav>
    </header>

    <main class="w-full">
        <!-- Banner -->
        <section id="featured" class="featured-banner">
            <div class="max-w-4xl">
                <h1 class="text-6xl md:text-9xl font-black mb-2 tracking-tighter uppercase leading-[0.85]">Chinmayee Gore</h1>
                <p class="text-xl md:text-3xl font-light text-gray-300 mt-6 tracking-wide max-w-2xl">
                    SaaS Customer Success | Analytics | Marketing Strategy
                </p>
                <div class="flex flex-wrap gap-4 mt-12">
                    <button onclick="document.getElementById('footer-contact').scrollIntoView()" class="px-12 py-4 bg-white text-black font-black uppercase text-xs tracking-widest hover:bg-red-600 hover:text-white transition-all">Get In Touch</button>
                    <button onclick="window.open('https://calendly.com/chinmayee-gore-zqneqt')" class="px-12 py-4 bg-transparent border-2 border-white text-white font-black uppercase text-xs tracking-widest hover:bg-white hover:text-black transition-all">Schedule Meet</button>
                </div>
            </div>
        </section>

        <!-- Compatibility Engine (Edge to Edge) -->
        <section class="w-full bg-[#111] border-y border-white/5">
            <div class="px-[5%] py-4 text-[10px] font-black text-red-600 uppercase tracking-[0.4em] bg-black/50">Skill Matrix Alignment</div>
            <div class="flex flex-wrap lg:flex-nowrap w-full">
                <div id="skill-btn-container" class="w-full lg:w-2/3 p-[5%] bg-zinc-900/30">
                    <!-- Skills injected here -->
                </div>
                <div class="w-full lg:w-1/3 bg-black flex flex-col items-center justify-center p-12 border-l border-white/5">
                    <span class="text-[10px] text-gray-500 uppercase font-black mb-4 tracking-[0.2em]">Match Percentage</span>
                    <div id="match-score" class="text-9xl font-black italic text-white transition-all duration-500">0%</div>
                </div>
            </div>
        </section>

        <!-- Experience Row -->
        <section id="experience" class="py-20 w-full overflow-hidden">
            <div class="section-header">
                <h2 class="text-xs font-black text-red-600 uppercase tracking-[0.3em] mb-2">Portfolio</h2>
                <h3 class="text-4xl font-black uppercase tracking-tighter">Work Experience</h3>
            </div>
            <div class="px-[5%] w-full">
                <div class="scroll-row">
                    <!-- MoEngage -->
                    <div class="card-item-container">
                        <div class="flip-inner">
                            <div class="flip-front utility-card">
                                <img src="https://iili.io/fRKkvYx.png" class="w-full h-40 object-cover grayscale hover:grayscale-0 transition-all" />
                                <div class="p-6">
                                    <h4 class="font-black text-lg uppercase leading-tight">Assoc. CSM</h4>
                                    <p class="text-xs text-red-600 font-bold mt-1">MoEngage</p>
                                </div>
                            </div>
                            <div class="flip-back">
                                <h5 class="text-[10px] font-black text-red-600 uppercase mb-4 tracking-widest">Key Impact</h5>
                                <ul class="text-xs text-gray-400 space-y-3 font-medium">
                                    <li>● KPI Alignment via AI</li>
                                    <li>● Churn Reduction Strategy</li>
                                    <li>● Product Roadmap Influence</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <!-- IMS -->
                    <div class="card-item-container">
                        <div class="flip-inner">
                            <div class="flip-front utility-card">
                                <img src="https://iili.io/fRK8jUb.png" class="w-full h-40 object-cover grayscale hover:grayscale-0 transition-all" />
                                <div class="p-6">
                                    <h4 class="font-black text-lg uppercase leading-tight">Ed. Consultant</h4>
                                    <p class="text-xs text-red-600 font-bold mt-1">IMS International</p>
                                </div>
                            </div>
                            <div class="flip-back">
                                <h5 class="text-[10px] font-black text-red-600 uppercase mb-4 tracking-widest">Key Impact</h5>
                                <ul class="text-xs text-gray-400 space-y-3 font-medium">
                                    <li>● Global Admissions Strategy</li>
                                    <li>● 100% Documentation Success</li>
                                    <li>● GRE/GMAT Planning</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Internship Row -->
        <section id="internship" class="py-20 bg-zinc-900/20 w-full overflow-hidden">
            <div class="section-header">
                <h3 class="text-4xl font-black uppercase tracking-tighter">Internships</h3>
            </div>
            <div class="px-[5%] w-full">
                <div class="scroll-row">
                    <div class="card-item-container">
                        <div class="flip-inner">
                            <div class="flip-front utility-card">
                                <img src="https://iili.io/fRDDXXj.png" class="w-full h-40 object-cover grayscale" />
                                <div class="p-6"><h4 class="font-black text-sm uppercase">Growth Hackers</h4></div>
                            </div>
                            <div class="flip-back flex items-center justify-center p-6"><p class="text-xs text-center text-gray-400 font-bold">Product Mgmt Trainee & GTM Strategy Design</p></div>
                        </div>
                    </div>
                    <div class="card-item-container">
                        <div class="flip-inner">
                            <div class="flip-front utility-card">
                                <img src="https://iili.io/fRDDwqQ.png" class="w-full h-40 object-cover grayscale" />
                                <div class="p-6"><h4 class="font-black text-sm uppercase">PTE University</h4></div>
                            </div>
                            <div class="flip-back flex items-center justify-center p-6"><p class="text-xs text-center text-gray-400 font-bold">Social Media Branding & Growth Assoc.</p></div>
                        </div>
                    </div>
                    <div class="card-item-container">
                        <div class="flip-inner">
                            <div class="flip-front utility-card">
                                <img src="https://iili.io/fRDDMmu.png" class="w-full h-40 object-cover grayscale" />
                                <div class="p-6"><h4 class="font-black text-sm uppercase">Unschool</h4></div>
                            </div>
                            <div class="flip-back flex items-center justify-center p-6"><p class="text-xs text-center text-gray-400 font-bold">Growth Manager & Community Outreach</p></div>
                        </div>
                    </div>
                    <div class="card-item-container">
                        <div class="flip-inner">
                            <div class="flip-front utility-card">
                                <img src="https://iili.io/fRDDE79.jpg" class="w-full h-40 object-cover grayscale" />
                                <div class="p-6"><h4 class="font-black text-sm uppercase">Safecity</h4></div>
                            </div>
                            <div class="flip-back flex items-center justify-center p-6"><p class="text-xs text-center text-gray-400 font-bold">Stakeholder Liaison & Safety Analytics</p></div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Certifications Row -->
        <section id="certifications" class="py-20 w-full overflow-hidden">
            <div class="section-header">
                <h3 class="text-4xl font-black uppercase tracking-tighter">Certifications</h3>
            </div>
            <div class="px-[5%] w-full">
                <div class="scroll-row">
                    <div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fEHgRGj.png" class="w-full h-full object-cover grayscale opacity-50 hover:opacity-100 transition-all" /></div><div class="flip-back p-6 flex items-center justify-center text-center text-xs font-black uppercase tracking-widest">Six Sigma Green Belt</div></div></div>
                    <div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fEHgoy7.png" class="w-full h-full object-cover grayscale opacity-50 hover:opacity-100 transition-all" /></div><div class="flip-back p-6 flex items-center justify-center text-center text-xs font-black uppercase tracking-widest">Neuromarketing</div></div></div>
                    <div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fEHgIje.png" class="w-full h-full object-cover grayscale opacity-50 hover:opacity-100 transition-all" /></div><div class="flip-back p-6 flex items-center justify-center text-center text-xs font-black uppercase tracking-widest">Bloomberg Market Concepts</div></div></div>
                    <div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fEHgzu9.png" class="w-full h-full object-cover grayscale opacity-50 hover:opacity-100 transition-all" /></div><div class="flip-back p-6 flex items-center justify-center text-center text-xs font-black uppercase tracking-widest">Data Analytics</div></div></div>
                </div>
            </div>
        </section>
    </main>

    <!-- Edge to Edge Footer -->
    <footer id="footer-contact" class="bg-black border-t border-white/5 py-24 w-full">
        <div class="px-[5%] grid grid-cols-1 lg:grid-cols-3 gap-16">
            <div>
                <h4 class="text-4xl font-black text-red-600 mb-6 tracking-tighter uppercase">CHINMAYEE GORE</h4>
                <p class="text-gray-500 font-bold text-sm tracking-widest uppercase mb-1">+91 8291109930</p>
                <p class="text-gray-500 font-bold text-sm tracking-widest uppercase">Mumbai, India</p>
            </div>
            <div class="space-y-6">
                <h4 class="text-[10px] font-black uppercase tracking-[0.4em] text-white">Navigation</h4>
                <ul class="space-y-4 text-xs font-bold uppercase tracking-widest text-gray-500">
                    <li><a href="mailto:gorechinmayee333@gmail.com" class="hover:text-red-600 transition">Email Direct</a></li>
                    <li><a href="https://linkedin.com/in/gorechinmayee" target="_blank" class="hover:text-red-600 transition">LinkedIn</a></li>
                </ul>
            </div>
            <div class="bg-zinc-900/50 p-8 border border-white/5">
                <h4 class="text-[10px] font-black uppercase tracking-[0.4em] text-red-600 mb-6">Send a Quick Ping</h4>
                <textarea id="email-draft-input" rows="3" class="w-full bg-black border border-white/10 p-4 text-white text-xs font-bold uppercase tracking-widest outline-none focus:border-red-600 transition-all mb-4" placeholder="Type message..."></textarea>
                <button onclick="sendEmail(document.getElementById('email-draft-input').value)" class="w-full py-4 bg-red-600 text-white font-black text-[10px] uppercase tracking-[0.3em] hover:bg-white hover:text-black transition-all">Submit</button>
            </div>
        </div>
        <div class="mt-24 text-center text-[10px] text-zinc-800 font-black uppercase tracking-[1em] border-t border-white/5 pt-12">&copy; 2025 ALL RIGHTS RESERVED</div>
    </footer>

    <script>
        const compSkills = ["Customer Success", "Retention Strategy", "Churn Reduction", "SaaS Onboarding", "NPS/CSAT", "Agile Roadmap", "GTM Strategy", "SEO/SEM", "Data Visualization", "CRM Workflow", "Marketing Analytics", "Market Research"];
        
        function initComp() {
            const list = document.getElementById('skill-btn-container');
            compSkills.forEach(s => {
                const b = document.createElement('button');
                b.className = "mini-skill-btn";
                b.innerText = s;
                b.onclick = () => { b.classList.toggle('active'); updateScore(); };
                list.appendChild(b);
            });
        }

        function updateScore() {
            const active = document.querySelectorAll('.mini-skill-btn.active').length;
            const scoreDisplay = document.getElementById('match-score');
            const score = Math.min(active * 12, 100);
            scoreDisplay.innerText = score + "%";
            scoreDisplay.style.color = score > 70 ? '#E50914' : 'white';
        }

        function sendEmail(message) {
            const body = encodeURIComponent(message || "Hello Chinmayee, I'm reaching out from your portfolio.");
            window.location.href = `mailto:gorechinmayee333@gmail.com?subject=Portfolio Inquiry&body=${body}`;
        }

        window.onload = () => {
            initComp();
            lucide.createIcons();
        };
    </script>
</body>
</html>
