<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Srishti Kathoute — Portfolio</title>
  <style>
    /* ---------- Base / Reset ---------- */
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#9aa4b2; --accent:#7c3aed; --glass: rgba(255,255,255,0.04);
      --max-width:1100px;
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial; background:linear-gradient(180deg,#071029 0%, #081428 100%); color:#e6eef6}
    a{color:var(--accent); text-decoration:none}
    img{max-width:100%;height:auto;display:block}

    /* ---------- Layout ---------- */
    .container{max-width:var(--max-width);margin:0 auto;padding:28px}
    header{display:flex;align-items:center;justify-content:space-between;gap:18px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#4f46e5);display:flex;align-items:center;justify-content:center;font-weight:700;font-size:18px}
    nav{display:flex;gap:12px;align-items:center}
    nav a{padding:8px 12px;border-radius:8px;color:var(--muted);font-weight:600}
    nav a:hover{background:var(--glass);color:#e6eef6}

    main{margin-top:28px}
    .hero{display:grid;grid-template-columns:1fr 380px;gap:28px;align-items:center;padding:28px;background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);border-radius:12px}
    .intro h1{margin:0;font-size:28px}
    .intro p{color:var(--muted);line-height:1.6}
    .cta{margin-top:16px;display:flex;gap:10px}
    .btn{background:var(--accent);color:white;padding:10px 14px;border-radius:10px;border:0;cursor:pointer;font-weight:700}
    .btn.ghost{background:transparent;border:1px solid rgba(255,255,255,0.06)}

    /* ---------- Cards & Projects ---------- */
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:22px}
    .card{background:var(--card);padding:16px;border-radius:12px;box-shadow:0 6px 18px rgba(2,6,23,0.6)}
    .card h3{margin:0 0 8px 0}
    .muted{color:var(--muted);font-size:14px}
    .skills{display:flex;flex-wrap:wrap;gap:8px;margin-top:10px}
    .skill{background:rgba(255,255,255,0.03);padding:6px 8px;border-radius:999px;font-size:13px}

    /* ---------- To-do app styles ---------- */
    .todo{display:flex;flex-direction:column;gap:8px}
    .todo input[type=text]{padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit}
    .todo ul{list-style:none;padding:0;margin:0;display:flex;flex-direction:column;gap:8px}
    .task{display:flex;align-items:center;gap:10px;padding:10px;background:rgba(255,255,255,0.02);border-radius:8px;transition:background 0.2s}
    .task:hover{background:rgba(255,255,255,0.04)}
    .task.completed .label{text-decoration:line-through;color:var(--muted)}
    .task button{margin-left:auto;background:transparent;border:0;color:var(--muted);cursor:pointer;font-size:14px;padding:4px 8px;border-radius:6px;transition:color 0.2s}
    .task button:hover{color:#ff4444}
    .task input[type="checkbox"]{width:18px;height:18px;cursor:pointer;accent-color:var(--accent);}


    /* ---------- Footer / Contact ---------- */
    footer{margin-top:28px;padding:20px;text-align:center;color:var(--muted)}
    form.contact{display:flex;flex-direction:column;gap:10px}
    input, textarea{padding:10px;border-radius:10px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit}

    /* ---------- Responsive ---------- */
    @media (max-width:1000px){
      .grid{grid-template-columns:repeat(2,1fr)}
      .hero{grid-template-columns:1fr 320px}
    }
    @media (max-width:720px){
      header{flex-direction:column;align-items:flex-start}
      .hero{grid-template-columns:1fr;}
      .grid{grid-template-columns:1fr}
      nav{flex-wrap:wrap}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">SK</div>
        <div>
          <div style="font-weight:800;letter-spacing:0.2px">Srishti Kathoute</div>
          <div class="muted" style="font-size:13px">Web Developer • 7 years experience</div>
        </div>
      </div>
      <nav>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#todo">To-Do App</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <main>
      <section class="hero" id="about">
        <div class="intro">
          <h1>Showcasing Web Development Skills</h1>
          <p>Hi — I'm <strong>Srishti Kathoute</strong>. This page showcases a set of learning projects built with HTML, CSS and JavaScript. Each project is designed to illustrate key web development competencies, from basic frontend design to full-stack application concepts.</p>
          <div class="cta">
            <button class="btn" onclick="document.getElementById('projects').scrollIntoView({behavior:'smooth'})">See Projects</button>
            <a class="btn ghost" href="#contact">Contact</a>
          </div>
        </div>
        <aside class="card">
          <h3>Quick Highlights</h3>
          <p class="muted">Skills, sample projects and an interactive demo are included below.</p>
          <div style="margin-top:12px">
            <div class="skills">
              <span class="skill">HTML5</span>
              <span class="skill">CSS3 & Responsiveness</span>
              <span class="skill">Vanilla JS</span>
              <span class="skill">DOM Manipulation</span>
              <span class="skill">Node.js/Express</span>
              <span class="skill">React/MERN</span>
              <span class="skill">Database (Mongo/Firestore)</span>
            </div>
          </div>
        </aside>
      </section>

      <section id="projects" style="margin-top:40px">
        <h2>Projects & Key Learning Areas</h2>
        <div class="grid">
          <!-- Project 1 -->
          <div class="card">
            <h3>Project 1 — Core Portfolio Site</h3>
            <p class="muted">Description: The foundation of modern web development, focusing on semantic markup and basic styling for presentation.</p>
            <div style="margin-top:8px;font-weight:700">Skills Gained:</div>
            <ul class="muted">
              <li>Semantic HTML structure</li>
              <li>Core CSS styling</li>
              <li>Variables and dark theme implementation</li>
            </ul>
          </div>

          <!-- Project 2 -->
          <div class="card">
            <h3>Project 2 — Responsive Landing Page</h3>
            <p class="muted">Description: Building a page that adapts seamlessly to all screen sizes, crucial for modern web experiences.</p>
            <div style="margin-top:8px;font-weight:700">Skills Gained:</div>
            <ul class="muted">
              <li>Flexbox and Grid layout</li>
              <li>CSS Media Queries</li>
              <li>Mobile-first design principles</li>
            </ul>
          </div>

          <!-- Project 3 -->
          <div class="card">
            <h3>Project 3 — Interactive To-Do List</h3>
            <p class="muted">Description: A core application demonstrating client-side state management and user interactivity using raw JavaScript.</p>
            <div style="margin-top:8px;font-weight:700">Skills Gained:</div>
            <ul class="muted">
              <li>Advanced DOM manipulation</li>
              <li>Event handling and delegation</li>
              <li>Local Storage persistence</li>
            </ul>
          </div>

          <!-- Project 4 -->
          <div class="card">
            <h3>Project 4 — Basic Blog Application (Backend focus)</h3>
            <p class="muted">Description: Focused on setting up a server and database connection to handle content creation, retrieval, and storage.</p>
            <div style="margin-top:8px;font-weight:700">Skills Gained:</div>
            <ul class="muted">
              <li>Node.js/Express server setup</li>
              <li>Database integration (MongoDB/SQL concepts)</li>
              <li>CRUD operations (Create, Read, Update, Delete)</li>
            </ul>
          </div>

          <!-- Project 5 -->
          <div class="card">
            <h3>Project 5 — E-Commerce Website (Full Stack)</h3>
            <p class="muted">Description: A complex, large-scale project integrating frontend components with authentication and transactional backend logic.</p>
            <div style="margin-top:8px;font-weight:700">Skills Gained:</div>
            <ul class="muted">
              <li>User authentication (JWT/Sessions)</li>
              <li>Advanced state management (React/Redux/Context)</li>
              <li>Payment gateway integration concepts</li>
            </ul>
          </div>

          <!-- Project 6 -->
          <div class="card">
            <h3>Project 6 — Real-Time Chat Application</h3>
            <p class="muted">Description: Focuses on establishing persistent, low-latency connections for instantaneous data exchange between users.</p>
            <div style="margin-top:8px;font-weight:700">Skills Gained:</div>
            <ul class="muted">
              <li>WebSocket technology / Socket.IO</li>
              <li>Real-time communication patterns</li>
              <li>User session and room management</li>
            </ul>
          </div>
        </div>
      </section>

      <!-- ---------- Interactive To-Do Demo ---------- -->
      <section id="todo" style="margin-top:40px">
        <h2>Interactive To-Do List (Demo)</h2>
        <div class="card">
          <div class="todo">
            <div style="display:flex;gap:8px">
              <input id="todo-input" type="text" placeholder="Add a new task..." />
              <button id="add-btn" class="btn">Add</button>
            </div>
            <ul id="task-list"></ul>
            <div style="margin-top:8px;color:var(--muted);font-size:13px">Tip: double-click a task label to edit it. The list persists in your browser's local storage.</div>
          </div>
        </div>
      </section>

      <!-- ---------- Contact ---------- -->
      <section id="contact" style="margin-top:40px">
        <h2>Contact</h2>
        <div class="card">
          <form class="contact" onsubmit="handleContact(event)">
            <input id="name" type="text" placeholder="Your name" required />
            <input id="email" type="email" placeholder="Your email" required />
            <textarea id="message" rows="5" placeholder="Your message" required></textarea>
            <div style="display:flex;gap:8px">
              <button type="submit" class="btn">Send (demo)</button>
              <a class="btn ghost" href="mailto:hello@example.com">Email me</a>
            </div>
          </form>
          <div id="contact-status" class="muted" style="margin-top:10px; display: none;"></div>
        </div>
      </section>

    </main>

    <footer>
      Built with ❤ by Srishti Kathoute • Demo portfolio — for learning and showcasing projects
    </footer>
  </div>

  <script>
    // Constants for Firebase (MANDATORY variables for the Canvas environment)
    const appId = typeof __app_id !== 'undefined' ? __app_id : 'default-app-id';
    const firebaseConfig = typeof _firebase_config !== 'undefined' ? JSON.parse(_firebase_config) : null;

    // We will use LocalStorage for the To-Do list since Firebase setup is not strictly required for this simple demo, 
    // and the original code used it. We'll improve the contact form behavior instead of using alert().

    // ---------- To-Do App Logic (using Local Storage for simple persistence) ----------
    const input = document.getElementById('todo-input');
    const addBtn = document.getElementById('add-btn');
    const list = document.getElementById('task-list');

    // Load from localStorage
    let tasks = JSON.parse(localStorage.getItem('sk_tasks') || '[]');

    function save(){ localStorage.setItem('sk_tasks', JSON.stringify(tasks)); }

    function render(){
      list.innerHTML = '';
      tasks.forEach((t, i) => {
        const li = document.createElement('li'); 
        li.className='task' + (t.done? ' completed':'');

        const chk = document.createElement('input'); 
        chk.type='checkbox'; 
        chk.checked = !!t.done;
        chk.addEventListener('change', ()=>{ t.done = chk.checked; save(); render(); });

        const label = document.createElement('div'); 
        label.className='label'; 
        label.textContent = t.text; 
        label.style.flex = '1'; // Make label take up space
        label.style.cursor='pointer';
        
        // edit on double click
        label.addEventListener('dblclick', ()=>{
          const ed = document.createElement('input'); 
          ed.type='text'; 
          ed.value = t.text; 
          ed.style.flex='1';
          
          const finalizeEdit = () => { 
            const newText = ed.value.trim();
            if(newText) {
                t.text = newText;
            }
            save(); 
            render(); 
          }

          ed.addEventListener('keydown', (e)=>{ 
            if(e.key==='Enter'){ 
                finalizeEdit();
            } 
          });

          // Revert if focus is lost (blur)
          ed.addEventListener('blur', finalizeEdit);
          
          li.replaceChild(ed, label); 
          ed.focus();
        });
        
        const del = document.createElement('button'); 
        del.textContent='Remove';
        del.addEventListener('click', ()=>{ 
            tasks.splice(i,1); 
            save(); 
            render(); 
        });

        li.appendChild(chk); 
        li.appendChild(label); 
        li.appendChild(del);
        list.appendChild(li);
      });

      // If list is empty, display a message
      if(tasks.length === 0) {
        const emptyMsg = document.createElement('div');
        emptyMsg.textContent = "Your list is empty. Add a new task above!";
        emptyMsg.className = "muted";
        emptyMsg.style.textAlign = "center";
        emptyMsg.style.padding = "10px";
        list.appendChild(emptyMsg);
      }
    }

    addBtn.addEventListener('click', ()=>{
      const val = input.value.trim(); 
      if(!val) return; 
      tasks.push({text:val, done:false}); 
      input.value=''; 
      save(); 
      render();
    });

    input.addEventListener('keydown', (e)=>{ 
        if(e.key==='Enter'){ 
            addBtn.click(); 
        } 
    });

    // initialize
    render();

    // ---------- Contact (demo) - Replaced alert() with a message box ----------
    function handleContact(e){ 
        e.preventDefault(); 
        
        const nameInput = document.getElementById('name');
        const emailInput = document.getElementById('email');
        const messageInput = document.getElementById('message');
        const statusDiv = document.getElementById('contact-status');

        const name = nameInput.value;
        
        statusDiv.textContent = Thank you, ${name}! This is a demo contact form. A real website would send this message to a server.;
        statusDiv.style.display = 'block';
        
        // Clear inputs after 3 seconds and hide status
        e.target.reset();
        setTimeout(() => {
            statusDiv.style.display = 'none';
            statusDiv.textContent = '';
        }, 5000);
    }
  </script>
</body>
</html>
