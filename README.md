<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Chinmayee Gore | Portfolio</title>
<script src="https://cdn.tailwindcss.com"></script>
<script src="https://unpkg.com/lucide@latest"></script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
:root {
--netflix-red: #E50914;
--dark-bg: #141414;
--light-text: #E5E7EB;
}
body {
font-family: 'Inter', sans-serif;
background-color: var(--dark-bg);
color: white;
scroll-behavior: smooth;
overflow-x: hidden;
}
.scroll-row::-webkit-scrollbar { display: none; }
.scroll-row { -ms-overflow-style: none; scrollbar-width: none; }
.featured-banner {
background-image: linear-gradient(to right, rgba(20,20,20,1) 10%, rgba(20,20,20,0.2) 60%, rgba(20,20,20,1) 100%), url('https://iili.io/fR2Ym92.jpg');
background-size: cover;
background-position: left;
}

/* Card Styles */
.card-item-container {
transition: transform .3s ease;
cursor: pointer;
width: 280px;
height: 320px;
flex-shrink: 0;
position: relative;
perspective: 1000px;
}
.card-item-container:hover { transform: scale(1.08); z-index: 50; }
.card-item-container:hover .flip-inner { box-shadow: 0 0 25px rgba(229,9,20,.9); }

.flip-inner {
position: relative;
width: 100%;
height: 100%;
transition: transform 0.6s;
transform-style: preserve-3d;
border-radius: 12px;
}
.card-item-container:hover .flip-inner { transform: rotateY(180deg); }
.flip-front, .flip-back {
position: absolute;
width: 100%;
height: 100%;
backface-visibility: hidden;
border-radius: 12px;
overflow: hidden;
}
.flip-back {
background: #1a1a1a;
transform: rotateY(180deg);
display: flex;
flex-direction: column;
justify-content: flex-start;
padding: 20px;
text-align: left;
border: 2px solid var(--netflix-red);
}

/* Compatibility Box */
.comp-box-full {
width: 100vw;
position: relative;
left: 50%;
right: 50%;
margin-left: -50vw;
margin-right: -50vw;
background: #1a1a1a;
border-top: 1px solid rgba(255,255,255,0.1);
border-bottom: 1px solid rgba(255,255,255,0.1);
margin-top: 2rem;
margin-bottom: 2rem;
}
.comp-split { display: flex; height: 240px; width: 100%; }
.comp-left { width: 60%; padding: 25px; overflow-y: auto; background: #111; border-right: 1px solid #333; }
.comp-right { width: 40%; display: flex; flex-direction: column; align-items: center; justify-content: center; background: #000; }
.mini-skill-btn { width: 100%; text-align: left; padding: 10px 15px; margin-bottom: 6px; border-radius: 6px; font-size: 13px; background: #262626; color: #888; border: 1px solid transparent; cursor: pointer; transition: 0.2s; }
.mini-skill-btn.active { background: var(--netflix-red); color: white; border-color: white; font-weight: bold; }

.utility-card {
background-color: #2A2A2A;
background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='80' height='80' viewBox='0 0 80 80'%3E%3Cg fill='%23333333' fill-opacity='0.1'%3E%3Cpath fill-rule='evenodd' d='M0 0h40v40H0V0zm40 40h40v40H40V40zm-40 80h40v40H0V80zm40-40h40v40H40V40z'/%3E%3C/g%3E%3C/svg%3E");
background-size: 40px 40px;
}
</style>
</head>
<body class="antialiased">

<header class="fixed top-0 w-full z-50 bg-black/60 backdrop-blur-md border-b border-white/10">
<nav class="flex items-center justify-between px-6 py-4">
<h1 class="text-2xl font-bold text-red-600 tracking-tight">PORTFOLIO</h1>
<ul class="hidden md:flex space-x-6 text-sm font-medium">
<li><a href="#experience" class="hover:text-red-500 transition">Experience</a></li>
<li><a href="#internship" class="hover:text-red-500 transition">Internship</a></li>
<li><a href="#academics" class="hover:text-red-500 transition">Academics</a></li>
<li><a href="#recognitions" class="hover:text-red-500 transition">Recognitions</a></li>
<li><a href="#certifications" class="hover:text-red-500 transition">Certifications</a></li>
</ul>
</nav>
</header>

<section id="featured" class="featured-banner pt-40 md:pt-48 h-[75vh] flex items-center">
<div class="w-full px-6 md:px-12 text-left">
<h1 class="text-5xl md:text-7xl font-extrabold mb-4 drop-shadow-lg leading-tight">Chinmayee Gore</h1>
<ul class="space-y-1 mt-4 text-xl font-medium max-w-xl text-gray-200">
<li>👋 Skilled at keeping SaaS customers happy.</li>
<li>🧑‍🏫 Can explain complex ideas clearly.</li>
<li>🎯 Leadership experience across education.</li>
</ul>
</div>
</section>

<div class="flex flex-wrap items-center justify-center gap-4 w-full py-10 px-6">
<a href="#footer-contact" class="flex items-center justify-center px-8 py-3 bg-white text-black border border-gray-300 rounded-full hover:bg-gray-100 transition-all shadow-sm font-bold">
<i data-lucide="sparkles" class="w-5 h-5 mr-2"></i><span>Contact Me</span>
</a>
<button onclick="window.open('https://calendly.com/chinmayee-gore-zqneqt')" class="flex items-center justify-center px-8 py-3 bg-red-600 text-white rounded-full hover:bg-red-700 hover:shadow-[0_0_20px_rgba(229,9,20,0.5)] transition-all font-bold">
<i data-lucide="calendar" class="w-5 h-5 mr-2"></i><span>Lets connect [Virtual]</span>
</button>
</div>

<div class="comp-box-full">
<div class="px-12 py-3 border-b border-white/10 text-[11px] font-black text-red-600 uppercase tracking-[0.3em] bg-zinc-900">Compatibility Engine</div>
<div class="comp-split">
<div id="skill-btn-container" class="comp-left"></div>
<div class="comp-right">
<span class="text-[10px] text-gray-500 uppercase font-black mb-2 tracking-widest">Candidate Fit</span>
<div id="match-score" class="text-7xl font-black italic text-white">0%</div>
</div>
</div>
</div>

<!-- WORK EXPERIENCE -->
<section id="experience" class="py-16 container mx-auto px-6">
<p class="text-red-600 text-3xl font-bold mb-2">Professional Journey</p>
<h3 class="text-2xl font-bold mb-8 text-white/90">Work Experience</h3>
<div class="flex space-x-8 overflow-x-auto pb-10 scroll-row">
<!-- MoEngage -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRKkvYx.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Assoc. CSM</h4><p class="text-sm text-gray-400">MoEngage</p><p class="text-[10px] text-gray-500">Aug 2024 – Oct 2025</p></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Aligning AI tools with client KPIs.</li>
<li>Guiding onboarding & use cases.</li>
<li>Managing QBRs & reducing churn.</li>
<li>Influencing product roadmap.</li>
</ul>
</div></div></div>
<!-- IMS -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRK8jUb.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Education Consultant</h4><p class="text-sm text-gray-400">IMS International</p><p class="text-[10px] text-gray-500">May 2024 – Jul 2024</p></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>End-to-end global university guidance.</li>
<li>Course shortlisting & SOP/LOR editing.</li>
<li>Expert documentation for 100% success rate.</li>
<li>Strategic planning for GRE, GMAT & IELTS.</li>
</ul>
</div></div></div>
</div>
</section>

<!-- INTERNSHIPS - 7 TOTAL -->
<section id="internship" class="py-12 container mx-auto px-6 md:px-12">
<h3 class="text-3xl font-bold mb-8 text-white/90">Internships & Live Projects</h3>
<div class="scroll-row flex overflow-x-scroll space-x-6 pb-4">
<!-- 1. Growth Hackers -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRDDXXj.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Product Mgmt Trainee</h4><p class="text-xs text-gray-400 mt-2">Growth Hackers</p></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Designed GTM strategy for digital products.</li>
<li>Improved UI/UX for landing pages.</li>
<li>Initiated affiliate partnerships & pipelines.</li>
<li>Awarded Letter of Appreciation.</li>
</ul>
</div></div></div>
<!-- 2. PTE University -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRDDwqQ.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Social Media Assoc.</h4><p class="text-xs text-gray-400 mt-2">PTE University</p></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Delivered lectures with innovative methods.</li>
<li>Improved student learning outcomes.</li>
<li>Managed strategic social media content.</li>
<li>Promoted university programs and branding.</li>
</ul>
</div></div></div>
<!-- 3. Geeta Group -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRDDhLx.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Digital Mkt Intern</h4><p class="text-xs text-gray-400 mt-2">Geeta Group</p></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Created articles and solved social media queries.</li>
<li>Improved institute's online presence.</li>
<li>Implemented content strategies for lead gen.</li>
<li>Boosted overall online engagement.</li>
</ul>
</div></div></div>
<!-- 4. Unschool -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRDDMmu.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Growth Manager</h4><p class="text-xs text-gray-400 mt-2">Unschool</p></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Tailored lectures for student body.</li>
<li>Implemented innovative teaching methods.</li>
<li>Managed social media for education.</li>
<li>Enhanced student enrollment via outreach.</li>
</ul>
</div></div></div>
<!-- 5. Safecity -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRDDE79.jpg" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Volunteer (Safe City)</h4><p class="text-xs text-gray-400 mt-2">Safe city</p></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Cataloged women's safety reports.</li>
<li>Identified critical cases for stakeholders.</li>
<li>Collaborated with law enforcement.</li>
<li>Generated 50+ reports in a single month.</li>
</ul>
</div></div></div>
<!-- 6. Piramal -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRDDc12.jpg" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Volunteer & Coach</h4><p class="text-xs text-gray-400 mt-2">Piramal Foundation</p></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Administered surveys for aid implementation.</li>
<li>Improved lives of people in need.</li>
<li>Coached students in modern science.</li>
<li>Leveraged tech with limited resources.</li>
</ul>
</div></div></div>
<!-- 7. Cur8 -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRDD1d7.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Community Influencer</h4><p class="text-xs text-gray-400 mt-2">Cur8</p></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Analyzed education marketing trends.</li>
<li>Strategized social media content.</li>
<li>Optimized SEO for community growth.</li>
<li>Contributed as a Growth Analyst.</li>
</ul>
</div></div></div>
</div>
</section>

<!-- ACADEMICS - Letter Style -->
<section id="academics" class="py-12 container mx-auto px-6 md:px-12">
<h3 class="text-3xl font-bold mb-8 text-white/90">Academic Credentials</h3>
<div class="scroll-row flex overflow-x-scroll space-x-6 pb-4">
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRbfHCP.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">MBA (Analytics)</h4><p class="text-xs text-gray-400 mt-2">NMIMS Hyderabad</p></div></div><div class="flip-back">
<div class="text-[10px] leading-tight text-gray-300 italic">
<p>Dear Reader,</p>
<p class="mt-2">My MBA in Marketing and Analytics equipped me with a powerful blend of marketing expertise and data-driven decision-making, allowing me to connect creativity with analytical insights.</p>
<p class="mt-2">Warm regards,<br>Chinmayee</p>
</div>
</div></div></div>
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRbhnDb.jpg" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">M.Com</h4><p class="text-xs text-gray-400 mt-2">Mumbai University</p></div></div><div class="flip-back">
<div class="text-[10px] leading-tight text-gray-300 italic">
<p>Dear Reader,</p>
<p class="mt-2">From my MCom in General Management, I gained enhanced strategic thinking and a broader perspective on management that helped me see the bigger picture in business operations.</p>
<p class="mt-2">Warm regards,<br>Chinmayee</p>
</div>
</div></div></div>
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRbecMb.jpg" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">BMS</h4><p class="text-xs text-gray-400 mt-2">Saraf College</p></div></div><div class="flip-back">
<div class="text-[10px] leading-tight text-gray-300 italic">
<p>Dear Reader,</p>
<p class="mt-2">The takeaway from my Bachelor of Management Studies was a solid foundation in business fundamentals and a clear understanding of how organizations operate and thrive.</p>
<p class="mt-2">Warm regards,<br>Chinmayee</p>
</div>
</div></div></div>
</div>
</section>

<!-- RECOGNITIONS - 7 TOTAL -->
<section id="recognitions" class="py-12 container mx-auto px-6 md:px-12">
<h3 class="text-3xl font-bold mb-8 text-white/90">Recognition</h3>
<div class="scroll-row flex overflow-x-scroll space-x-6 pb-4">
<!-- 1. Operencia -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRDDlgS.jpg" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Co-Head</h4><p class="text-xs text-gray-400">Operencia</p></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Oversaw Event Planning & Management.</li>
<li>Organized high-impact guest lectures (KPMG).</li>
<li>Led a club of over 50 members.</li>
<li>Enhanced student engagement & growth.</li>
</ul>
</div></div></div>
<!-- 2. Student Council -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRbfHCP.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Student Council</h4></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Represented student concerns to administration.</li>
<li>Coordinated supportive campus environment.</li>
<li>Liaison for effective communication.</li>
<li>Promoted welfare and enriching experiences.</li>
</ul>
</div></div></div>
<!-- 3. Hostel Committee -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRbfHCP.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Hostel Committee</h4></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Managed overall accommodation structure.</li>
<li>Ensured facility standards & maintenance.</li>
<li>Addressed infrastructure issues promptly.</li>
<li>Contributed to welcoming atmosphere.</li>
</ul>
</div></div></div>
<!-- 4. Growth Hackers Appreciation -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRDDXXj.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Appreciation - Growth Hackers</h4></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Excellence in market research tasks.</li>
<li>Contributed significantly to sales goals.</li>
<li>Enhanced product feature usability.</li>
<li>Improved website UI/UX design.</li>
</ul>
</div></div></div>
<!-- 5. PTE Recommendation -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRDDwqQ.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Recommendation - PTE university</h4></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Developed strategic content calendars.</li>
<li>Recognized for marketing creativity.</li>
<li>Reliable support for university branding.</li>
<li>Earned strong letter of recommendation.</li>
</ul>
</div></div></div>
<!-- 6. DLLE -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRbAo4R.jpg" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">DLLE Council</h4></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Organized social awareness programs.</li>
<li>Executed community outreach in Mumbai.</li>
<li>Promoted lifelong learning initiatives.</li>
<li>Focused on social responsibility programs.</li>
</ul>
</div></div></div>
<!-- 7. UNICEF -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fRbAIYN.jpg" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">UNICEF</h4></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Driven COVID-19 awareness campaigns.</li>
<li>Spreading crucial health information.</li>
<li>Supported public community safety.</li>
<li>Impactful efforts during global pandemic.</li>
</ul>
</div></div></div>
</div>
</section>

<!-- CERTIFICATIONS - 4 TOTAL -->
<section id="certifications" class="py-12 container mx-auto px-6 md:px-12">
<h3 class="text-3xl font-bold mb-8 text-white/90">Certifications</h3>
<div class="scroll-row flex overflow-x-scroll space-x-6 pb-4">
<!-- Six Sigma -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fEHgRGj.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Six Sigma</h4></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Process Improvement Mastery & Lean tools.</li>
<li>Data-Driven Decision Making techniques.</li>
<li>Reducing Waste & Operational Cost strategies.</li>
<li>Leadership in Quality Management (Green Belt).</li>
</ul>
</div></div></div>
<!-- Neuromarketing -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fEHgoy7.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Neuromarketing</h4></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Understanding neural Consumer Behavior.</li>
<li>Applying Neuroscience to Persuasive Marketing.</li>
<li>Enhancing Customer Experience cues.</li>
<li>Analyzing neural data for marketing.</li>
</ul>
</div></div></div>
<!-- Marketing - Bloomberg Market Concepts -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fEHgIje.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Marketing</h4></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Mastered Bloomberg analytical tools.</li>
<li>Market research and competitive positioning.</li>
<li>Strategic Marketing Planning for growth.</li>
<li>Analytical understanding of global markets.</li>
</ul>
</div></div></div>
<!-- Data Analytics -->
<div class="card-item-container"><div class="flip-inner"><div class="flip-front utility-card"><img src="https://iili.io/fEHgzu9.png" class="w-full h-32 object-cover" /><div class="p-4"><h4 class="font-bold">Data Analytics</h4></div></div><div class="flip-back">
<h5 class="text-[11px] font-bold text-red-600 uppercase mb-2">To summon up</h5>
<ul class="text-[10px] text-gray-300 space-y-1 list-disc ml-4">
<li>Data Interpretation from large datasets.</li>
<li>Hands-on Excel, SQL, and Visualization tools.</li>
<li>Turning data into strategic recommendations.</li>
<li>Structured data-led problem solving.</li>
</ul>
</div></div></div>
</div>
</section>

<!-- FOOTER / CONTACT -->
<footer id="footer-contact" class="py-10 border-t border-gray-800 bg-gray-900 mt-16">
<div class="container mx-auto px-6 md:px-12 grid md:grid-cols-3 gap-8 text-left">
<div>
<h4 class="text-lg font-semibold mb-3 text-white">About</h4>
<p class="text-sm text-gray-400">Chinmayee Gore: +918291109930</p>
</div>
<div>
<h4 class="text-lg font-semibold mb-3 text-white">Links</h4>
<ul class="space-y-2 text-sm text-gray-400">
<li><a href="mailto:gorechinmayee333@gmail.com" class="hover:text-red-500">Email Me Directly</a></li>
<li><a href="https://linkedin.com/in/gorechinmayee" target="_blank" class="hover:text-red-500">LinkedIn</a></li>
</ul>
</div>
<div>
<h4 class="text-lg font-semibold mb-3 text-white flex items-center">
<i data-lucide="mail-open" class="w-5 h-5 mr-2 text-red-500"></i>Direct Contact
</h4>
<textarea id="email-draft-input" rows="2" class="w-full p-2 bg-gray-800 border border-gray-700 text-white rounded-lg" placeholder="Type your message..."></textarea>
<button onclick="sendEmail(document.getElementById('email-draft-input').value)" class="w-full mt-2 px-4 py-2 bg-red-600 text-white font-bold rounded-lg hover:bg-red-700 transition-colors">Open My Mailer</button>
</div>
</div>
<div class="text-center text-sm text-gray-600 pt-8 mt-8 border-t border-gray-800">&copy; 2025 CG Portfolio. All Rights Reserved.</div>
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
document.getElementById('match-score').innerText = Math.min(active * 12, 100) + "%";
}
function sendEmail(message) {
const body = encodeURIComponent(message || "Hello Chinmayee, I'm interested in your profile.");
window.location.href = `mailto:gorechinmayee333@gmail.com?subject=Portfolio Inquiry&body=${body}`;
}
window.onload = () => {
initComp();
lucide.createIcons();
};
</script>
</body>
</html>
