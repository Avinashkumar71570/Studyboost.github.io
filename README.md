<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<meta name="description" content="StudyBoost - Free Class 11 Science Notes, Formulas, Important Questions and JEE Preparation Resources.">

<title>StudyBoost | Class 11 Science</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  scroll-behavior:smooth;
}

:root{
  --primary:#2563eb;
  --primary-dark:#1d4ed8;
  --dark:#0f172a;
  --text:#334155;
  --muted:#64748b;
  --bg:#f8fafc;
  --card:#ffffff;
  --border:#e2e8f0;
}

body.dark{
  --dark:#f8fafc;
  --text:#cbd5e1;
  --muted:#94a3b8;
  --bg:#020617;
  --card:#0f172a;
  --border:#1e293b;
}

body{
  font-family:Arial,Helvetica,sans-serif;
  background:var(--bg);
  color:var(--text);
  line-height:1.6;
  transition:.25s;
}

/* HEADER */

header{
  position:sticky;
  top:0;
  z-index:1000;
  background:var(--card);
  border-bottom:1px solid var(--border);
}

.navbar{
  max-width:1200px;
  margin:auto;
  padding:15px 20px;
  display:flex;
  align-items:center;
  justify-content:space-between;
}

.logo{
  text-decoration:none;
  font-size:25px;
  font-weight:800;
  color:var(--primary);
}

.logo span{
  color:var(--dark);
}

nav{
  display:flex;
  align-items:center;
  gap:20px;
}

nav a{
  text-decoration:none;
  color:var(--dark);
  font-size:14px;
  font-weight:600;
}

nav a:hover{
  color:var(--primary);
}

.nav-buttons{
  display:flex;
  gap:8px;
}

.icon-btn{
  border:1px solid var(--border);
  background:var(--card);
  color:var(--dark);
  padding:8px 11px;
  border-radius:8px;
  cursor:pointer;
  font-size:16px;
}

.menu{
  display:none;
}

/* HERO */

.hero{
  padding:90px 20px;
  text-align:center;
  background:linear-gradient(135deg,#eff6ff,var(--bg));
}

.badge{
  display:inline-block;
  background:#dbeafe;
  color:#1d4ed8;
  padding:7px 14px;
  border-radius:30px;
  font-size:13px;
  font-weight:bold;
  margin-bottom:20px;
}

.hero h1{
  color:var(--dark);
  font-size:clamp(40px,7vw,70px);
  line-height:1.05;
}

.hero h1 span{
  color:var(--primary);
}

.hero p{
  max-width:720px;
  margin:20px auto;
  color:var(--muted);
  font-size:18px;
}

.buttons{
  display:flex;
  justify-content:center;
  gap:12px;
  flex-wrap:wrap;
  margin-top:30px;
}

.btn{
  display:inline-block;
  padding:12px 20px;
  border-radius:9px;
  text-decoration:none;
  font-weight:bold;
  cursor:pointer;
  border:0;
}

.primary{
  background:var(--primary);
  color:white;
}

.primary:hover{
  background:var(--primary-dark);
}

.secondary{
  background:var(--card);
  color:var(--dark);
  border:1px solid var(--border);
}

/* GENERAL */

.section{
  max-width:1200px;
  margin:auto;
  padding:70px 20px;
}

.title{
  text-align:center;
  margin-bottom:35px;
}

.title h2{
  color:var(--dark);
  font-size:34px;
}

.title p{
  color:var(--muted);
}

/* SUBJECTS */

.subjects{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:20px;
}

.subject{
  background:var(--card);
  border:1px solid var(--border);
  border-radius:16px;
  padding:28px 20px;
  text-align:center;
  transition:.25s;
}

.subject:hover{
  transform:translateY(-5px);
  box-shadow:0 12px 30px rgba(0,0,0,.08);
}

.subject-icon{
  font-size:42px;
  margin-bottom:12px;
}

.subject h3{
  color:var(--dark);
  margin-bottom:8px;
}

.subject p{
  color:var(--muted);
  font-size:14px;
  margin-bottom:18px;
}

/* SEARCH */

.search-box{
  max-width:750px;
  margin:0 auto 25px;
}

.search-box input{
  width:100%;
  padding:17px 20px;
  border:1px solid var(--border);
  background:var(--card);
  color:var(--dark);
  border-radius:12px;
  font-size:16px;
  outline:none;
}

.search-box input:focus{
  border-color:var(--primary);
}

/* FILTERS */

.filters{
  display:flex;
  justify-content:center;
  flex-wrap:wrap;
  gap:8px;
  margin-bottom:30px;
}

.filter{
  padding:9px 15px;
  border-radius:20px;
  border:1px solid var(--border);
  background:var(--card);
  color:var(--dark);
  cursor:pointer;
  font-weight:600;
}

.filter.active,
.filter:hover{
  background:var(--primary);
  color:white;
  border-color:var(--primary);
}

/* NOTES */

.notes{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
}

.note{
  background:var(--card);
  border:1px solid var(--border);
  border-radius:15px;
  padding:24px;
  transition:.2s;
}

.note:hover{
  transform:translateY(-4px);
  box-shadow:0 10px 25px rgba(0,0,0,.07);
}

.tag{
  display:inline-block;
  background:#eff6ff;
  color:var(--primary);
  padding:5px 9px;
  border-radius:6px;
  font-size:11px;
  font-weight:bold;
  margin-bottom:10px;
}

.note h3{
  color:var(--dark);
  margin-bottom:8px;
}

.note p{
  color:var(--muted);
  font-size:14px;
  margin-bottom:18px;
}

.note-buttons{
  display:flex;
  gap:7px;
  flex-wrap:wrap;
}

.small{
  display:inline-block;
  padding:8px 12px;
  border-radius:7px;
  text-decoration:none;
  font-size:13px;
  font-weight:bold;
}

.read{
  background:var(--primary);
  color:white;
}

.pdf{
  background:#f1f5f9;
  color:#0f172a;
}

/* JEE */

.jee{
  background:#020617;
  color:white;
  border-radius:25px;
  padding:55px 30px;
  text-align:center;
}

.jee h2{
  font-size:38px;
}

.jee>p{
  max-width:700px;
  margin:10px auto;
  color:#cbd5e1;
}

.jee-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:18px;
  margin-top:35px;
}

.jee-card{
  background:rgba(255,255,255,.08);
  border:1px solid rgba(255,255,255,.1);
  border-radius:14px;
  padding:22px;
  text-align:left;
}

.jee-card h3{
  margin-bottom:7px;
}

.jee-card p{
  color:#cbd5e1;
  font-size:14px;
}

/* FORMULAS */

.formulas{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
}

.formula{
  background:var(--card);
  border:1px solid var(--border);
  border-radius:15px;
  padding:25px;
  text-align:center;
}

.formula h3{
  color:var(--dark);
  margin-bottom:12px;
}

.equation{
  background:var(--bg);
  color:var(--primary);
  padding:15px;
  border-radius:10px;
  font-size:19px;
  font-weight:bold;
}

/* FEATURES */

.features{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
}

.feature{
  text-align:center;
  padding:25px;
}

.feature-icon{
  font-size:36px;
}

.feature h3{
  color:var(--dark);
  margin:8px 0;
}

.feature p{
  color:var(--muted);
  font-size:14px;
}

/* CONTACT */

.contact{
  max-width:700px;
  margin:auto;
  background:var(--card);
  border:1px solid var(--border);
  border-radius:16px;
  padding:30px;
}

.contact input,
.contact textarea{
  width:100%;
  padding:13px;
  margin-bottom:15px;
  border:1px solid var(--border);
  border-radius:8px;
  background:var(--bg);
  color:var(--dark);
  font-family:inherit;
}

.contact textarea{
  min-height:130px;
}

/* FOOTER */

footer{
  background:#020617;
  color:white;
  padding:45px 20px 25px;
}

.footer{
  max-width:1200px;
  margin:auto;
  display:grid;
  grid-template-columns:2fr 1fr 1fr;
  gap:40px;
}

.footer h3{
  margin-bottom:12px;
}

.footer p,
.footer a{
  color:#94a3b8;
  font-size:14px;
}

.footer a{
  display:block;
  text-decoration:none;
  margin:7px 0;
}

.footer a:hover{
  color:white;
}

.copyright{
  max-width:1200px;
  margin:30px auto 0;
  padding-top:20px;
  border-top:1px solid #1e293b;
  text-align:center;
  color:#64748b;
  font-size:13px;
}

/* MOBILE */

@media(max-width:900px){

  .subjects{
    grid-template-columns:repeat(2,1fr);
  }

  .notes{
    grid-template-columns:repeat(2,1fr);
  }

  .jee-grid,
  .formulas,
  .features{
    grid-template-columns:1fr;
  }
}

@media(max-width:700px){

  .menu{
    display:block;
    background:var(--card);
    color:var(--dark);
    border:1px solid var(--border);
    padding:8px 12px;
    border-radius:8px;
    cursor:pointer;
    font-size:20px;
  }

  nav{
    display:none;
    position:absolute;
    top:64px;
    left:0;
    right:0;
    background:var(--card);
    flex-direction:column;
    align-items:flex-start;
    padding:20px;
    border-bottom:1px solid var(--border);
  }

  nav.show{
    display:flex;
  }

  .nav-buttons{
    margin-left:auto;
    margin-right:10px;
  }

  .subjects,
  .notes{
    grid-template-columns:1fr;
  }

  .footer{
    grid-template-columns:1fr;
  }

  .hero{
    padding:65px 18px;
  }

  .hero p{
    font-size:16px;
  }

  .section{
    padding:55px 16px;
  }

  .jee{
    padding:40px 20px;
  }

  .jee h2{
    font-size:30px;
  }
}
</style>
</head>

<body>

<header>

<div class="navbar">

<a href="#home" class="logo">
Study<span>Boost</span>
</a>

<nav id="nav">

<a href="#home">Home</a>
<a href="#subjects">Subjects</a>
<a href="#notes">Notes</a>
<a href="#formulas">Formulas</a>
<a href="#jee">JEE</a>
<a href="#contact">Contact</a>

</nav>

<div class="nav-buttons">

<button class="icon-btn" onclick="toggleDark()" title="Dark Mode">
🌙
</button>

<button class="menu" onclick="toggleMenu()">
☰
</button>

</div>

</div>

</header>


<section class="hero" id="home">

<div class="badge">
🎓 Free Class 11 Study Resources
</div>

<h1>
Learn Smart.<br>
<span>Score Better.</span>
</h1>

<p>
Free Class 11 Science notes, formulas, important questions
and JEE preparation resources — all in one place.
</p>

<div class="buttons">

<a href="#notes" class="btn primary">
📚 Explore Notes
</a>

<a href="#jee" class="btn secondary">
🚀 JEE Preparation
</a>

</div>

</section>


<section class="section" id="subjects">

<div class="title">

<h2>📚 Explore Subjects</h2>

<p>
Choose your subject and start learning.
</p>

</div>

<div class="subjects">

<div class="subject">

<div class="subject-icon">⚛️</div>

<h3>Physics</h3>

<p>
Concepts, formulas, numericals and important questions.
</p>

<a href="#physics" class="btn primary">
Explore
</a>

</div>


<div class="subject">

<div class="subject-icon">🧪</div>

<h3>Chemistry</h3>

<p>
Physical, Inorganic and Organic Chemistry.
</p>

<a href="#chemistry" class="btn primary">
Explore
</a>

</div>


<div class="subject">

<div class="subject-icon">📐</div>

<h3>Mathematics</h3>

<p>
Concepts, formulas and practice questions.
</p>

<a href="#maths" class="btn primary">
Explore
</a>

</div>


<div class="subject">

<div class="subject-icon">💻</div>

<h3>Computer Science</h3>

<p>
Python, programming and computer concepts.
</p>

<a href="#cs" class="btn primary">
Explore
</a>

</div>

</div>

</section>


<section class="section" id="notes">

<div class="title">

<h2>🔎 Notes Library</h2>

<p>
Search and filter Class 11 study material.
</p>

</div>

<div class="search-box">

<input
id="search"
type="text"
placeholder="Search chapter, subject or topic..."
onkeyup="filterNotes()">

</div>

<div class="filters">

<button class="filter active" onclick="setFilter('all',this)">
All
</button>

<button class="filter" onclick="setFilter('physics',this)">
Physics
</button>

<button class="filter" onclick="setFilter('chemistry',this)">
Chemistry
</button>

<button class="filter" onclick="setFilter('maths',this)">
Mathematics
</button>

<button class="filter" onclick="setFilter('cs',this)">
Computer Science
</button>

</div>


<div class="notes" id="notesList">


<div class="note" data-subject="physics">

<span class="tag">PHYSICS</span>

<h3>Units & Measurements</h3>

<p>
Units, dimensions, errors and significant figures.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


<div class="note" data-subject="physics">

<span class="tag">PHYSICS</span>

<h3>Motion in a Straight Line</h3>

<p>
Distance, displacement, velocity and acceleration.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


<div class="note" data-subject="physics">

<span class="tag">PHYSICS</span>

<h3>Motion in a Plane</h3>

<p>
Vectors, projectile motion and circular motion.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


<div class="note" data-subject="physics">

<span class="tag">PHYSICS</span>

<h3>Laws of Motion</h3>

<p>
Newton's laws, friction and circular dynamics.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


<div class="note" data-subject="chemistry">

<span class="tag">CHEMISTRY</span>

<h3>Some Basic Concepts</h3>

<p>
Mole concept, molar mass and stoichiometry.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="Class_XI_Chemistry_Ch1_JEE_School_All_Topics_Notes.pdf" class="small pdf" target="_blank">
📥 PDF
</a>

</div>

</div>


<div class="note" data-subject="chemistry">

<span class="tag">CHEMISTRY</span>

<h3>Structure of Atom</h3>

<p>
Atomic models, quantum numbers and electronic configuration.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


<div class="note" data-subject="chemistry">

<span class="tag">CHEMISTRY</span>

<h3>Periodic Classification</h3>

<p>
Periodic table and periodic properties.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


<div class="note" data-subject="chemistry">

<span class="tag">CHEMISTRY</span>

<h3>Chemical Bonding</h3>

<p>
Ionic, covalent bonding and molecular structure.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


<div class="note" data-subject="maths">

<span class="tag">MATHEMATICS</span>

<h3>Sets</h3>

<p>
Sets, subsets, intervals and operations.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


<div class="note" data-subject="maths">

<span class="tag">MATHEMATICS</span>

<h3>Relations & Functions</h3>

<p>
Relations, functions and important concepts.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


<div class="note" data-subject="maths">

<span class="tag">MATHEMATICS</span>

<h3>Trigonometric Functions</h3>

<p>
Identities, equations and graphs.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


<div class="note" data-subject="cs">

<span class="tag">COMPUTER SCIENCE</span>

<h3>Python Basics</h3>

<p>
Variables, data types and basic programming.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


<div class="note" data-subject="cs">

<span class="tag">COMPUTER SCIENCE</span>

<h3>Conditional Statements</h3>

<p>
if, elif and else statements.
</p>

<div class="note-buttons">

<a href="#" class="small read">📖 Read Notes</a>

<a href="#" class="small pdf">📥 PDF</a>

</div>

</div>


</div>

</section>


<section class="section" id="physics">

<div class="title">

<h2>⚛️ Physics</h2>

<p>Class 11 Physics chapter resources.</p>

</div>

<div class="notes">

<div class="note">

<span class="tag">CHAPTER 1</span>

<h3>Units & Measurements</h3>

<p>
Dimensions, errors, significant figures and units.
</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>


<div class="note">

<span class="tag">CHAPTER 2</span>

<h3>Motion in a Straight Line</h3>

<p>
Motion, velocity, acceleration and graphs.
</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>


<div class="note">

<span class="tag">CHAPTER 3</span>

<h3>Motion in a Plane</h3>

<p>
Vectors, projectile motion and circular motion.
</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>


<div class="note">

<span class="tag">CHAPTER 4</span>

<h3>Laws of Motion</h3>

<p>
Newton's laws, friction and dynamics.
</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>

</div>

</section>


<section class="section" id="chemistry">

<div class="title">

<h2>🧪 Chemistry</h2>

<p>Class 11 Chemistry resources.</p>

</div>

<div class="notes">

<div class="note">

<span class="tag">CHEMISTRY</span>

<h3>Some Basic Concepts</h3>

<p>Mole concept and stoichiometry.</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>


<div class="note">

<span class="tag">CHEMISTRY</span>

<h3>Structure of Atom</h3>

<p>Atomic models and electronic configuration.</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>


<div class="note">

<span class="tag">CHEMISTRY</span>

<h3>Periodic Classification</h3>

<p>Periodic table and periodic properties.</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>

</div>

</section>


<section class="section" id="maths">

<div class="title">

<h2>📐 Mathematics</h2>

<p>Class 11 Mathematics resources.</p>

</div>

<div class="notes">

<div class="note">

<span class="tag">MATHS</span>

<h3>Sets</h3>

<p>Sets, subsets and operations.</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>


<div class="note">

<span class="tag">MATHS</span>

<h3>Relations & Functions</h3>

<p>Relations, functions and concepts.</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>


<div class="note">

<span class="tag">MATHS</span>

<h3>Trigonometric Functions</h3>

<p>Identities, equations and graphs.</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>

</div>

</section>


<section class="section" id="cs">

<div class="title">

<h2>💻 Computer Science</h2>

<p>Class 11 Computer Science resources.</p>

</div>

<div class="notes">

<div class="note">

<span class="tag">PYTHON</span>

<h3>Python Basics</h3>

<p>Variables, data types and basic programming.</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>


<div class="note">

<span class="tag">PYTHON</span>

<h3>Conditional Statements</h3>

<p>if, elif and else statements.</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>


<div class="note">

<span class="tag">PYTHON</span>

<h3>Loops</h3>

<p>for loops, while loops and practice.</p>

<a href="#notes" class="small read">Study Chapter</a>

</div>

</div>

</section>


<section class="section" id="formulas">

<div class="title">

<h2>📝 Formula Sheets</h2>

<p>Quick revision formulas.</p>

</div>

<div class="formulas">

<div class="formula">

<h3>⚛️ Physics</h3>

<div class="equation">
v = u + at
</div>

<p>Equation of motion</p>

</div>


<div class="formula">

<h3>🧪 Chemistry</h3>

<div class="equation">
n = m / M
</div>

<p>Mole calculation</p>

</div>


<div class="formula">

<h3>📐 Mathematics</h3>

<div class="equation">
sin²θ + cos²θ = 1
</div>

<p>Trigonometric identity</p>

</div>

</div>

</section>


<section class="section" id="jee">

<div class="jee">

<h2>🚀 JEE Preparation</h2>

<p>
Build a strong Class 11 foundation with smart preparation,
consistent practice and regular revision.
</p>

<div class="jee-grid">

<div class="jee-card">

<h3>📅 Study Plan</h3>

<p>
Create a balanced daily and weekly study routine.
</p>

</div>


<div class="jee-card">

<h3>🎯 Chapter Strategy</h3>

<p>
Understand concepts before moving to difficult questions.
</p>

</div>


<div class="jee-card">

<h3>🧠 Revision</h3>

<p>
Revise short notes and formulas regularly.
</p>

</div>


<div class="jee-card">

<h3>✍️ Practice</h3>

<p>
Practice NCERT, school and JEE-style questions.
</p>

</div>


<div class="jee-card">

<h3>📊 Mock Tests</h3>

<p>
Test yourself and analyse your mistakes.
</p>

</div>


<div class="jee-card">

<h3>🔥 Consistency</h3>

<p>
Small daily progress creates a strong foundation.
</p>

</div>

</div>

</div>

</section>


<section class="section">

<div class="title">

<h2>✨ Why StudyBoost?</h2>

<p>Simple tools for smarter study.</p>

</div>

<div class="features">

<div class="feature">

<div class="feature-icon">🆓</div>

<h3>Free Resources</h3>

<p>
Useful educational resources in one place.
</p>

</div>


<div class="feature">

<div class="feature-icon">📱</div>

<h3>Mobile Friendly</h3>

<p>
Study comfortably on phone, tablet or computer.
</p>

</div>


<div class="feature">

<div class="feature-icon">⚡</div>

<h3>Quick Revision</h3>

<p>
Find important concepts and formulas quickly.
</p>

</div>

</div>

</section>


<section class="section" id="contact">

<div class="title">

<h2>📩 Contact</h2>

<p>Have a suggestion or question?</p>

</div>

<div class="contact">

<form onsubmit="sendMessage(event)">

<input
type="text"
id="name"
placeholder="Your Name"
required>

<input
type="email"
id="email"
placeholder="Your Email"
required>

<textarea
id="message"
placeholder="Your Message"
required></textarea>

<button class="btn primary">
Send Message
</button>

</form>

</div>

</section>


<footer>

<div class="footer">

<div>

<h3>StudyBoost 🚀</h3>

<p>
Free Class 11 Science notes, formulas,
important questions and JEE preparation resources.
</p>

</div>


<div>

<h3>Quick Links</h3>

<a href="#home">Home</a>
<a href="#subjects">Subjects</a>
<a href="#notes">Notes</a>
<a href="#formulas">Formulas</a>
<a href="#jee">JEE</a>

</div>


<div>

<h3>Subjects</h3>

<a href="#physics">Physics</a>
<a href="#chemistry">Chemistry</a>
<a href="#maths">Mathematics</a>
<a href="#cs">Computer Science</a>

</div>

</div>


<div class="copyright">

© 2026 StudyBoost. Free educational resources for students.

</div>

</footer>


<script>

function toggleMenu(){

document
.getElementById("nav")
.classList
.toggle("show");

}


function toggleDark(){

document.body.classList.toggle("dark");

}


let currentFilter = "all";


function setFilter(subject,button){

currentFilter = subject;

document
.querySelectorAll(".filter")
.forEach(function(btn){

btn.classList.remove("active");

});

button.classList.add("active");

filterNotes();

}


function filterNotes(){

const search =
document
.getElementById("search")
.value
.toLowerCase();

const cards =
document.querySelectorAll("#notesList .note");

cards.forEach(function(card){

const text =
card.innerText.toLowerCase();

const subject =
card.dataset.subject;

const matchesSearch =
text.includes(search);

const matchesFilter =
currentFilter === "all" ||
subject === currentFilter;

if(matchesSearch && matchesFilter){

card.style.display="block";

}else{

card.style.display="none";

}

});

}


function sendMessage(event){

event.preventDefault();

const name =
document
.getElementById("name")
.value;

alert(
"Thank you, " +
name +
"! Your message has been received."
);

event.target.reset();

}

</script>

</body>
</html>
