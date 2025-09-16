<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Voyage & Valor — Vocabulary Game</title>
  <style>
    :root{--bg:#0f1724;--card:#0b1220;--accent:#6ee7b7;--accent2:#60a5fa;--muted:#9aa7bd}
    *{box-sizing:border-box;font-family:Inter,ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,'Helvetica Neue',Arial}
    html,body{height:100%;margin:0;background:linear-gradient(180deg,#07132a 0%, #041022 60%);color:#e6eef8}
    .container{max-width:1100px;margin:26px auto;padding:22px}
    header{display:flex;align-items:center;gap:18px}
    .logo{width:68px;height:68px;border-radius:14px;background:linear-gradient(135deg,var(--accent),var(--accent2));display:flex;align-items:center;justify-content:center;font-weight:800;color:#04263b;font-size:26px;box-shadow:0 8px 30px rgba(6,12,24,.6)}
    h1{margin:0;font-size:22px}
    p.lead{margin-top:6px;color:var(--muted)}
    .main{display:grid;grid-template-columns:340px 1fr;gap:18px;margin-top:18px}

    /* left panel */
    .panel{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:14px;border-radius:12px;box-shadow:0 6px 18px rgba(2,6,23,.6)}
    .menu button{display:block;width:100%;padding:12px;border-radius:10px;border:0;background:transparent;color:inherit;text-align:left;margin-bottom:8px;font-weight:600;cursor:pointer}
    .menu button.active{background:rgba(255,255,255,0.03);box-shadow:inset 0 1px 0 rgba(255,255,255,0.02)}
    .score{margin-top:12px;padding:12px;border-radius:10px;background:rgba(255,255,255,0.02)}
    .score .big{font-size:28px;font-weight:800}
    .small{color:var(--muted);font-size:13px}

    /* right content */
    .content{min-height:420px;padding:18px;border-radius:12px}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:18px;border-radius:12px}
    .controls{display:flex;gap:10px;align-items:center;margin-bottom:12px}
    .btn{background:linear-gradient(90deg,var(--accent2),var(--accent));padding:10px 14px;border-radius:10px;border:0;color:#04263b;font-weight:700;cursor:pointer}
    .ghost{background:transparent;border:1px solid rgba(255,255,255,0.04);padding:10px 12px;border-radius:10px}

    /* quiz */
    .question{font-size:20px;font-weight:700;margin:12px 0}
    .options{display:grid;grid-template-columns:1fr 1fr;gap:10px}
    .option{padding:12px;border-radius:10px;background:rgba(255,255,255,0.02);cursor:pointer;border:1px solid transparent}
    .option:hover{transform:translateY(-3px)}
    .option.correct{outline:3px solid rgba(110,231,183,0.14);background:linear-gradient(90deg, rgba(110,231,183,0.04), rgba(96,165,250,0.02));}
    .option.wrong{outline:3px solid rgba(255,94,94,0.12);opacity:.9}

    /* match */
    .match-grid{display:flex;gap:12px}
    .col{flex:1}
    .draggable{padding:10px;margin:8px 0;border-radius:8px;background:rgba(255,255,255,0.02);cursor:grab}
    .dropzone{min-height:48px;padding:8px;border-radius:8px;margin:8px 0;border:1px dashed rgba(255,255,255,0.04);background:rgba(255,255,255,0.01)}
    .dropzone.drag-over{background:rgba(110,231,183,0.1);border-color:var(--accent)}

    /* adventure map */
    .map{display:flex;gap:12px;justify-content:space-between}
    .location{flex:1;padding:12px;border-radius:12px;text-align:center;cursor:pointer}
    .locked{opacity:.4;filter:grayscale(.2)}

    /* Adventure Modal */
    .modal{display:none;position:fixed;top:0;left:0;width:100%;height:100%;background:rgba(0,0,0,0.7);z-index:1000;align-items:center;justify-content:center}
    .modal-content{background:var(--card);padding:20px;border-radius:12px;max-width:500px;width:90%;box-shadow:0 10px 30px rgba(0,0,0,0.5)}
    .modal-header{font-size:18px;font-weight:700;margin-bottom:15px}
    .modal-input{width:100%;padding:10px;margin:10px 0;border-radius:8px;background:#031524;color:#ccdef7;border:1px solid rgba(255,255,255,0.03)}
    .modal-feedback{color:var(--muted);font-size:14px;margin:10px 0;min-height:20px}
    .modal-buttons{display:flex;gap:10px;justify-content:flex-end;margin-top:15px}

    footer{margin-top:18px;color:var(--muted);font-size:13px;text-align:center}

    /* responsive */
    @media(max-width:900px){.main{grid-template-columns:1fr;}.logo{width:58px;height:58px}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="logo">V&V</div>
      <div style="flex:1">
        <h1 id="title">Voyage & Valor — Vocabulary Game</h1>
        <p class="lead" id="lead">Learn words about <strong>war</strong> and <strong>tourism</strong> with mini-games — quick quizzes, matching, and an adventure map. Designed for high schoolers.</p>
      </div>
      <div style="display:flex;flex-direction:column;gap:6px;align-items:flex-end">
        <div style="display:flex;gap:6px">
          <button id="langEn" class="ghost">EN</button>
          <button id="langVi" class="ghost">VI</button>
        </div>
        <a id="downloadBtn" class="btn" href="#" download="voyage-valor.html">Download HTML</a>
      </div>
    </header>

    <div class="main">
      <aside class="panel">
        <div class="menu">
          <button id="btn-quiz" class="active">🎯 Quick Quiz</button>
          <button id="btn-match">🧩 Match Definitions</button>
          <button id="btn-adventure">🗺️ Adventure Map</button>
          <button id="btn-edit">✏️ Edit / Add Words</button>
        </div>

        <div class="score">
          <div class="big" id="score">Score: 0</div>
          <div class="small">Streak: <span id="streak">0</span> • Level: <span id="level">1</span></div>
        </div>

        <div style="margin-top:12px;display:flex;gap:8px;">
          <button id="btn-reset" class="ghost">Reset Progress</button>
          <button id="btn-help" class="ghost">How to Play / Hosting</button>
        </div>
      </aside>

      <section class="content">
        <div id="view-quiz" class="card">
          <div class="controls">
            <select id="filterCat">
              <option value="both">All topics</option>
              <option value="war">War</option>
              <option value="tourism">Tourism</option>
            </select>
            <button id="nextQuiz" class="btn">New Question</button>
            <div style="margin-left:auto" class="small">Timer: <span id="timer">--</span></div>
          </div>
          <div id="quizArea">
            <div class="question" id="questionText">Press "New Question" to start!</div>
            <div class="options" id="options"></div>
          </div>
        </div>

        <div id="view-match" class="card" style="margin-top:12px;display:none">
          <div class="small">Drag a word and drop it onto the correct definition.</div>
          <div class="match-grid" style="margin-top:12px">
            <div class="col">
              <div id="wordList"></div>
            </div>
            <div class="col">
              <div id="defList"></div>
            </div>
          </div>
          <div style="display:flex;gap:8px;margin-top:12px">
            <button id="shuffleMatch" class="btn">Shuffle</button>
            <button id="checkMatch" class="ghost">Check Answers</button>
          </div>
        </div>

        <div id="view-adventure" class="card" style="margin-top:12px;display:none">
          <div class="small">Unlock destinations by answering vocabulary questions. Each location needs 3 correct answers.</div>
          <div class="map" style="margin-top:12px">
            <div class="location locked" data-loc="1" id="loc1">🏰 Historic Fort<br/>(Locked)</div>
            <div class="location locked" data-loc="2" id="loc2">🏝️ Beach Bay<br/>(Locked)</div>
            <div class="location locked" data-loc="3" id="loc3">🏛️ City Museum<br/>(Locked)</div>
          </div>
        </div>

        <div id="view-edit" class="card" style="margin-top:12px;display:none">
          <div class="small">Edit the vocabulary list (JSON). Keep the structure: [{"word":"...","def":"...","example":"...","viDef":"...","viExample":"...","cat":"war|tourism"}, ...]</div>
          <textarea id="vocabJson" style="width:100%;height:260px;margin-top:8px;border-radius:8px;padding:10px;background:#031524;color:#ccdef7;border:1px solid rgba(255,255,255,0.03);"></textarea>
          <div style="display:flex;gap:8px;margin-top:8px">
            <button id="saveVocab" class="btn">Save</button>
            <button id="resetVocab" class="ghost">Reset to Default</button>
          </div>
        </div>

      </section>
    </div>

    <footer id="footer">Tip: Save your progress in your browser. Want a classroom version (teams)? I can customize it.</footer>
  </div>

  <!-- Adventure Modal -->
  <div id="adventureModal" class="modal">
    <div class="modal-content">
      <div class="modal-header" id="modalTitle">Answer to unlock</div>
      <div id="modalQuestion" class="small" style="min-height:40px"></div>
      <input type="text" id="modalAnswer" class="modal-input" placeholder="Type your answer here">
      <div id="modalFeedback" class="modal-feedback"></div>
      <div class="modal-buttons">
        <button id="modalCancel" class="ghost">Cancel</button>
        <button id="modalSubmit" class="btn">Submit</button>
      </div>
    </div>
  </div>

<script>
/* ===== language & strings ===== */
let LANG='en';
const STRINGS = {
  en: {
    quick:'🎯 Quick Quiz', match:'🧩 Match Definitions', adv:'🗺️ Adventure Map', edit:'✏️ Edit / Add Words',
    tip:'Tip: Save your progress in your browser. Want a classroom version (teams)? I can customize it.',
    how: `Modes:
- Quick Quiz: multiple-choice questions.
- Match: drag words to definitions.
- Adventure: unlock locations with correct answers.
Earn points to increase level and keep streaks. You can edit the word list in Edit mode. Save progress is automatic in your browser.

Hosting (quick):
1) Create a GitHub repo (public).
2) Upload this HTML file named index.html.
3) In repo Settings → Pages, choose branch main and / (root). Save. Your game will be published at username.github.io/repo-name within a minute or two.`,
    scoring: `Scoring System:
• Quick Quiz: +10 for correct, -3 for wrong
• Match: +5 per correct match
• Adventure: +8 per correct answer
• Streak: Consecutive correct answers increase your streak
• Level: Every 5 consecutive correct answers increases your level`
  },
  vi: {
    quick:'🎯 Trắc nghiệm nhanh', match:'🧩 Ghép định nghĩa', adv:'🗺️ Bản đồ phiêu lưu', edit:'✏️ Chỉnh sửa / Thêm từ',
    tip:'Mẹo: Lưu tiến trình trong trình duyệt. Muốn phiên bản lớp học (nhóm)? Mình có thể tuỳ chỉnh.',
    how: `Chế độ:
- Trắc nghiệm nhanh: câu hỏi nhiều lựa chọn.
- Ghép: kéo từ vào định nghĩa.
- Phiêu lưu: mở khóa địa điểm bằng trả lời đúng.
Tích điểm để tăng cấp và giữ chuỗi thắng. Bạn có thể chỉnh danh sách từ ở mục Chỉnh sửa. Tiến trình được lưu tự động trong trình duyệt.

Hướng dẫn nhanh để đưa lên GitHub Pages:
1) Tạo repo trên GitHub (public).
2) Tải tệp HTML này lên và đặt tên "index.html".
3) Vào Settings → Pages, chọn branch main và thư mục root (/). Lưu. Trang sẽ xuất hiện ở username.github.io/repo-name trong vài phút.`,
    scoring: `Hệ thống tính điểm:
• Trắc nghiệm: +10 cho câu đúng, -3 cho câu sai
• Ghép từ: +5 cho mỗi cặp đúng
• Phiêu lưu: +8 cho mỗi câu trả lời đúng
• Chuỗi: Câu trả lời đúng liên tiếp tăng chuỗi của bạn
• Cấp độ: Mỗi 5 câu trả lời đúng liên tiếp sẽ tăng cấp của bạn`
  }
};
function t(k){return STRINGS[LANG][k]||k}

/* ===== vocabulary (default) ===== */
let defaultVocab = [
  {word:"armistice",def:"A formal agreement to stop fighting; a truce.",example:"The two countries signed an armistice after weeks of negotiation.",viDef:"Thỏa thuận chính thức để ngừng chiến; đình chiến.",viExample:"Hai nước ký hiệp định đình chiến sau nhiều tuần đàm phán.",cat:"war"},
  {word:"siege",def:"A military operation in which an enemy surrounds a place and cuts off supplies.",example:"The city endured a long siege before surrendering.",viDef:"Chiến dịch bao vây, nơi kẻ thù vây quanh và cắt nguồn tiếp tế.",viExample:"Thành phố bị bao vây lâu trước khi đầu hàng.",cat:"war"},
  {word:"alliance",def:"A union formed for mutual benefit, especially between countries or organizations.",example:"Several nations formed an alliance for defense.",viDef:"Liên minh được lập để cùng có lợi, đặc biệt giữa các quốc gia.",viExample:"Nhiều quốc gia đã lập liên minh để phòng thủ.",cat:"war"},
  {word:"casualty",def:"A person injured or killed in an accident or war.",example:"The battle produced many casualties.",viDef:"Người bị thương hoặc tử vong trong tai nạn hoặc chiến tranh.",viExample:"Trận chiến gây ra nhiều thương vong.",cat:"war"},
  {word:"occupation",def:"Control of a country by military forces; also a job/role.",example:"The occupation lasted for years.",viDef:"Sự chiếm đóng một quốc gia bởi lực lượng quân sự; cũng có thể là nghề nghiệp.",viExample:"Cuộc chiếm đóng kéo dài nhiều năm.",cat:"war"},
  {word:"strategy",def:"A plan of action designed to achieve a long-term goal.",example:"Their strategy helped secure the victory.",viDef:"Kế hoạch hành động nhằm đạt mục tiêu lâu dài.",viExample:"Chiến lược của họ giúp giành chiến thắng.",cat:"war"},
  {word:"guerrilla",def:"A member of a small independent group taking part in irregular fighting, typically against larger forces.",example:"Guerrilla fighters used hit-and-run tactics.",viDef:"Chiến sĩ du kích — nhóm nhỏ đánh du kích chống lực lượng lớn hơn.",viExample:"Các du kích dùng chiến thuật đánh rồi rút lui.",cat:"war"},
  {word:"troop",def:"A group of soldiers.",example:"New troops were sent to the border.",viDef:"Một nhóm binh lính.",viExample:"Quân tiếp viện được gửi đến biên giới.",cat:"war"},
  {word:"reconnaissance",def:"Military observation to locate an enemy or ascertain strategic features.",example:"Reconnaissance planes flew over the area.",viDef:"Hoạt động trinh sát quân sự để tìm địch hoặc khảo sát địa hình.",viExample:"Máy bay trinh sát bay qua khu vực.",cat:"war"},
  {word:"treaty",def:"A formally concluded and ratified agreement between states.",example:"They signed a peace treaty.",viDef:"Hiệp ước được ký kết và phê chuẩn giữa các quốc gia.",viExample:"Họ ký một hiệp ước hòa bình.",cat:"war"},

  {word:"itinerary",def:"A planned route or journey.",example:"We followed a 7-day itinerary around the country.",viDef:"Lịch trình hoặc hành trình đã được lên kế hoạch.",viExample:"Chúng tôi theo lịch trình 7 ngày vòng quanh đất nước.",cat:"tourism"},
  {word:"backpacker",def:"A person who travels with a backpack, often on a low budget.",example:"Backpackers often stay in hostels.",viDef:"Người du lịch ba lô, thường tiết kiệm.",viExample:"Người đi ba lô thường ở hostel.",cat:"tourism"},
  {word:"souvenir",def:"An object kept as a reminder of a place or event.",example:"She bought a small souvenir from the market.",viDef:"Vật lưu niệm được giữ để nhớ về một nơi hay sự kiện.",viExample:"Cô ấy mua một món đồ lưu niệm nhỏ ở chợ.",cat:"tourism"},
  {word:"landmark",def:"An important or easily recognized building or site.",example:"The Eiffel Tower is a famous landmark.",viDef:"Công trình hoặc địa điểm dễ nhận ra, mang tính biểu tượng.",viExample:"Tháp Eiffel là một địa danh nổi tiếng.",cat:"tourism"},
  {word:"hostel",def:"A cheap place where travelers can stay, often with shared rooms.",example:"We booked a bed in a hostel downtown.",viDef:"Nơi lưu trú giá rẻ cho du khách, thường là phòng chung.",viExample:"Chúng tôi đặt một giường tại hostel ở trung tâm.",cat:"tourism"},
  {word:"excursion",def:"A short journey or trip, especially one engaged in as a leisure activity.",example:"They went on a day excursion to the nearby islands.",viDef:"Chuyến đi ngắn, thường mang tính giải trí.",viExample:"Họ đi tham quan một ngày tới các đảo gần đó.",cat:"tourism"},
  {word:"tourist trap",def:"A place that attracts many tourists and charges high prices for souvenirs or food.",example:"The crowded market felt like a tourist trap.",viDef:"Nơi thu hút khách du lịch nhưng thường 'chặt chém' về giá.",viExample:"Chợ đông khách trông giống như một nơi bẫy du lịch.",cat:"tourism"},
  {word:"guide",def:"A person who shows tourists around places of interest.",example:"Our guide explained the history of the ruins.",viDef:"Hướng dẫn viên — người đưa du khách tham quan.",viExample:"Hướng dẫn viên của chúng tôi giải thích lịch sử di tích.",cat:"tourism"},
  {word:"visa",def:"An official endorsement on a passport allowing entry into a country.",example:"You may need a visa before traveling.",viDef:"Thị thực — giấy phép nhập cảnh vào một quốc gia.",viExample:"Bạn có thể cần visa trước khi đi du lịch.",cat:"tourism"},
  {word:"transit",def:"The act of passing through a place on the way to somewhere else.",example:"We had a short transit in the capital city.",viDef:"Quá cảnh — đi qua một nơi trên đường đến điểm đến khác.",viExample:"Chúng tôi có một quá cảnh ngắn ở thủ đô.",cat:"tourism"}
];

/* ===== local storage helpers ===== */
function loadVocab(){
  let v = localStorage.getItem('vv_vocab');
  if(v) try{return JSON.parse(v);}catch(e){}
  return JSON.parse(JSON.stringify(defaultVocab));
}
let vocab = loadVocab();

let state = {score:0,streak:0,level:1,unlocked:{},mapProgress:{}};
function loadState(){
  let s = localStorage.getItem('vv_state');
  if(s) try{state=Object.assign(state,JSON.parse(s));}catch(e){}
}
function saveState(){localStorage.setItem('vv_state',JSON.stringify(state));updateHUD();}
loadState();

/* ===== HUD & UI wiring ===== */
function updateHUD(){
  document.getElementById('score').innerText = (LANG==='en'? 'Score: ':'Điểm: ')+state.score;
  document.getElementById('streak').innerText = state.streak;
  document.getElementById('level').innerText = state.level;
}
updateHUD();

const views = {quiz:document.getElementById('view-quiz'),match:document.getElementById('view-match'),adventure:document.getElementById('view-adventure'),edit:document.getElementById('view-edit')};
const btnQuiz=document.getElementById('btn-quiz'),btnMatch=document.getElementById('btn-match'),btnAdv=document.getElementById('btn-adventure'),btnEdit=document.getElementById('btn-edit');
btnQuiz.onclick=()=>show('quiz');btnMatch.onclick=()=>show('match');btnAdv.onclick=()=>show('adventure');btnEdit.onclick=()=>show('edit');
function show(v){
  for(let k in views){views[k].style.display='none';}
  btnQuiz.classList.remove('active');btnMatch.classList.remove('active');btnAdv.classList.remove('active');btnEdit.classList.remove('active');
  if(v==='quiz'){views.quiz.style.display='block';btnQuiz.classList.add('active'); stopTimer(); resetQuizArea();}
  if(v==='match'){views.match.style.display='block';btnMatch.classList.add('active')}
  if(v==='adventure'){views.adventure.style.display='block';btnAdv.classList.add('active')}
  if(v==='edit'){views.edit.style.display='block';btnEdit.classList.add('active');document.getElementById('vocabJson').value = JSON.stringify(vocab,null,2)}
}

/* ===== language toggles ===== */
document.getElementById('langEn').onclick=()=>{LANG='en';applyLang();};
document.getElementById('langVi').onclick=()=>{LANG='vi';applyLang();};
function applyLang(){
  document.getElementById('btn-quiz').innerText = STRINGS[LANG].quick;
  document.getElementById('btn-match').innerText = STRINGS[LANG].match;
  document.getElementById('btn-adventure').innerText = STRINGS[LANG].adv;
  document.getElementById('btn-edit').innerText = STRINGS[LANG].edit;
  document.getElementById('footer').innerText = STRINGS[LANG].tip;
  document.getElementById('btn-help').onclick = ()=>alert(STRINGS[LANG].how);
  updateHUD();
}
applyLang();

/* ===== small controls ===== */
document.getElementById('btn-reset').onclick=()=>{if(confirm(LANG==='en'? 'Reset all progress and scores?':'Bạn có chắc muốn đặt lại tiến trình và điểm?')){localStorage.removeItem('vv_state');state={score:0,streak:0,level:1,unlocked:{},mapProgress:{}};saveState();alert(LANG==='en'? 'Progress reset.':'Đã đặt lại tiến trình.');}};
document.getElementById('btn-help').onclick=()=>alert(STRINGS[LANG].how + '\n\n' + STRINGS[LANG].scoring);

/* ===== quiz logic ===== */
let quizTimerId=null;let quizTime=20;let currentQ=null;
function pickQuestion(category){
  let pool = vocab.filter(v=>category==='both' || v.cat===category);
  if(pool.length===0) return null;
  let correct = pool[Math.floor(Math.random()*pool.length)];
  let options = [correct];
  while(options.length<4){
    let cand = vocab[Math.floor(Math.random()*vocab.length)];
    if(!options.find(o=>o.word===cand.word)) options.push(cand);
  }
  for(let i=options.length-1;i>0;i--){let j=Math.floor(Math.random()*(i+1));[options[i],options[j]]=[options[j],options[i]]}
  return {q:correct,options};
}

document.getElementById('nextQuiz').onclick=()=>startQuiz(document.getElementById('filterCat').value);
function startQuiz(cat){
  stopTimer();
  resetQuizArea();
  let q = pickQuestion(cat);
  if(!q){document.getElementById('questionText').innerText=(LANG==='en'? 'No words in this category.':'Không có từ trong mục này.');return}
  currentQ=q;
  document.getElementById('questionText').innerText = (LANG==='en'? 'Which word matches this definition?\n"':'Từ nào phù hợp với định nghĩa sau?\n"') + (LANG==='en'? q.q.def : q.q.viDef) + '"';
  let opts = document.getElementById('options');opts.innerHTML='';
  q.options.forEach(o=>{
    let b = document.createElement('div');b.className='option';b.innerText=o.word; b.onclick=()=>selectOption(b,o);
    opts.appendChild(b);
  });
  quizTime=20;document.getElementById('timer').innerText=quizTime+'s';
  quizTimerId=setInterval(()=>{quizTime--;document.getElementById('timer').innerText=quizTime+'s';if(quizTime<=0){stopTimer();revealAnswer(null)}},1000);
}

function resetQuizArea() {
  document.getElementById('questionText').innerText = (LANG==='en' ? 'Press "New Question" to start!' : 'Nhấn "Câu hỏi mới" để bắt đầu!');
  document.getElementById('options').innerHTML = '';
  document.getElementById('timer').innerText = '--';
  currentQ = null;
}

function stopTimer(){if(quizTimerId)clearInterval(quizTimerId);quizTimerId=null;document.getElementById('timer').innerText='--'}
function selectOption(el,opt){stopTimer();if(!currentQ) return;let correct = currentQ.q.word===opt.word; if(correct){el.classList.add('correct');onCorrect(10);}else{el.classList.add('wrong');onWrong(-3);revealAnswer(opt);}
  let opts = document.querySelectorAll('.option');opts.forEach(o=>{if(o.innerText===currentQ.q.word) o.classList.add('correct')})
}
function revealAnswer(selected){
  if(!currentQ) return;
  let area = document.getElementById('questionText');
  let example = LANG==='en'? currentQ.q.example : currentQ.q.viExample;
  area.innerText = (LANG==='en'? 'Definition: "':'Định nghĩa: "') + (LANG==='en'? currentQ.q.def : currentQ.q.viDef) + '"\n\n' + (LANG==='en'? 'Answer: ':'Đáp án: ') + currentQ.q.word + '\n' + (LANG==='en'? 'Example: ':'Ví dụ: ') + example;
}

function onCorrect(points){state.score+=points;state.streak++;if(state.streak%5===0)state.level++;saveState();}
function onWrong(points){state.score+=points;state.streak=0;saveState();}

/* ===== match logic ===== */
function shuffleArray(a){let b=a.slice();for(let i=b.length-1;i>0;i--){let j=Math.floor(Math.random()*(i+1));[b[i],b[j]]=[b[j],b[i]]}return b}

function renderMatch(){
  const words = shuffleArray(vocab.map(v=>v.word)).slice(0,8);
  const defs = words.map(w=>vocab.find(x=>x.word===w)[LANG==='en'? 'def':'viDef']);
  const defsShuffled=shuffleArray(defs);
  const wordList = document.getElementById('wordList');const defList=document.getElementById('defList');
  wordList.innerHTML='';defList.innerHTML='';
  words.forEach(w=>{
    let d=document.createElement('div');
    d.className='draggable';
    d.draggable=true;
    d.innerText=w;
    d.id='w-'+w;
    d.addEventListener('dragstart',ev=>{ev.dataTransfer.setData('text/plain',w)});
    wordList.appendChild(d);
  });

  defsShuffled.forEach((d,idx)=>{
    let drop=document.createElement('div');
    drop.className='dropzone';
    drop.id='d-'+idx;
    drop.innerHTML='<div class="small">'+d+'</div>';
    drop.addEventListener('dragover',ev=>{ev.preventDefault();drop.classList.add('drag-over')});
    drop.addEventListener('dragleave',ev=>{drop.classList.remove('drag-over')});
    drop.addEventListener('drop',ev=>{ev.preventDefault();drop.classList.remove('drag-over');let w=ev.dataTransfer.getData('text/plain');
      let existing=drop.querySelector('.draggable');if(existing)document.getElementById('wordList').appendChild(existing);
      let el=document.getElementById('w-'+w);if(el)drop.appendChild(el);
    });
    defList.appendChild(drop);
  });
}

document.getElementById('shuffleMatch').onclick=renderMatch;
document.getElementById('checkMatch').onclick=()=>{
  let drops = Array.from(document.querySelectorAll('.dropzone'));
  let correct=0;let total=0;
  drops.forEach(d=>{
    let defEl = d.querySelector('.small');
    if(!defEl) return;
    let def = defEl.innerText;
    let child = d.querySelector('.draggable');
    if(child){
      total++;
      let word = child.innerText;
      let real = vocab.find(v=>v.word===word)[LANG==='en'? 'def':'viDef'];
      if(real===def){d.style.borderColor='rgba(110,231,183,0.3)';correct++;}else{d.style.borderColor='rgba(255,94,94,0.2)';}
    }
  });
  if(correct===total && total>0){
    alert((LANG==='en'? 'Great! ':'Tuyệt! ')+correct+'/'+total+' '+(LANG==='en'? 'correct. +':'đúng. +')+(correct*5)+' '+(LANG==='en'? 'points':'điểm'));
    state.score+=correct*5;state.streak+=correct;saveState();
  } else {
    alert((LANG==='en'? 'You got ':'Bạn trả lời ')+correct+'/'+total+' '+(LANG==='en'? 'correct. Try again!':'đúng. Thử lại nhé!'));
    state.streak=0;saveState();
  }
}

/* ===== adventure logic & modal ===== */
function updateMap(){
  for(let i=1;i<=3;i++){
    let el=document.getElementById('loc'+i);
    let prog = state.mapProgress['loc'+i]||0;
    let label=(i===1? (LANG==='en'? '🏰 Historic Fort':'🏰 Pháo đài cổ'):(i===2? (LANG==='en'? '🏝️ Beach Bay':'🏝️ Vịnh biển'):(LANG==='en'? '🏛️ City Museum':'🏛️ Bảo tàng')));
    el.innerHTML = label + '<br/>' + (prog>=3? (LANG==='en'? 'Unlocked!':'Đã mở khóa!'):(LANG==='en'? 'Locked - ':'Khóa - ')+prog+'/3');
    if(prog>=3){el.classList.remove('locked');}else{el.classList.add('locked')}
  }
}
updateMap();
Array.from(document.querySelectorAll('.location')).forEach(el=>el.onclick=()=>{let id = el.dataset.loc; playAdventure(id);});

// Modal elements
const modal = document.getElementById('adventureModal');
const modalTitle = document.getElementById('modalTitle');
const modalQuestion = document.getElementById('modalQuestion');
const modalAnswer = document.getElementById('modalAnswer');
const modalFeedback = document.getElementById('modalFeedback');
const modalSubmit = document.getElementById('modalSubmit');
const modalCancel = document.getElementById('modalCancel');

let adventureState = { locId: null, correctCount: 0, totalNeeded: 0 };
let adventureQuestion = null; // holds the currently shown adventure question

function playAdventure(id){
  let need = 3 - (state.mapProgress['loc'+id]||0);
  if(need<=0){
    alert(LANG==='en'? 'You already unlocked this location — well done!':'Bạn đã mở khoá địa điểm này — rất tốt!');
    return;
  }

  adventureState = { locId: id, correctCount: 0, totalNeeded: need };
  modal.style.display = 'flex';
  modalTitle.textContent = LANG==='en' ? 'Answer to unlock' : 'Trả lời để mở khoá';
  modalFeedback.textContent = '';
  modalAnswer.value = '';
  showNextAdventureQuestion();
}

function showNextAdventureQuestion(){
  if(adventureState.correctCount >= adventureState.totalNeeded){
    state.mapProgress['loc'+adventureState.locId] = (state.mapProgress['loc'+adventureState.locId]||0) + adventureState.correctCount;
    if(state.mapProgress['loc'+adventureState.locId] > 3) state.mapProgress['loc'+adventureState.locId] = 3;
    saveState();
    updateMap();
    modal.style.display = 'none';
    return;
  }
  // pick and store current adventure question
  adventureQuestion = pickQuestion('both');
  if(!adventureQuestion){ modalQuestion.textContent = LANG==='en' ? 'No questions available.' : 'Không có câu hỏi.'; return; }
  modalQuestion.textContent = LANG==='en' ? adventureQuestion.q.def : adventureQuestion.q.viDef;
  modalFeedback.textContent = '';
  modalAnswer.value = '';
  modalAnswer.focus();
}

modalSubmit.onclick = function(){
  let ans = modalAnswer.value.trim();
  if(!ans) return;
  if(!adventureQuestion) return;
  if(ans.toLowerCase() === adventureQuestion.q.word.toLowerCase()){
    adventureState.correctCount++;
    state.score += 8;
    state.streak++;
    modalFeedback.textContent = (LANG==='en' ? 'Correct! ' : 'Đúng rồi! ') + (LANG==='en' ? adventureQuestion.q.example : adventureQuestion.q.viExample);
    modalFeedback.style.color = 'var(--accent)';
  } else {
    state.streak = 0;
    modalFeedback.textContent = (LANG==='en' ? 'Incorrect. The correct answer is: ' : 'Sai. Đáp án đúng là: ') + adventureQuestion.q.word;
    modalFeedback.style.color = '#ff5e5e';
  }
  saveState();
  // after a short delay, go to next
  setTimeout(()=>{ showNextAdventureQuestion(); }, 1200);
};

modalCancel.onclick = function(){ modal.style.display = 'none'; };

// close modal by clicking outside
window.onclick = function(event){ if(event.target === modal){ modal.style.display = 'none'; } };

/* ===== edit & save vocab ===== */
document.getElementById('saveVocab').onclick=()=>{
  try{
    let j = JSON.parse(document.getElementById('vocabJson').value);
    if(!Array.isArray(j)) throw (LANG==='en' ? 'Vocabulary must be an array' : 'Danh sách từ phải là một mảng');
    for(let item of j){
      if(!item.word || !item.def || !item.cat) {
        throw (LANG==='en' ? 'Each vocabulary item must have word, def, and cat properties' : 'Mỗi từ phải có thuộc tính word, def, và cat');
      }
    }
    vocab = j;
    localStorage.setItem('vv_vocab', JSON.stringify(vocab));
    alert(LANG==='en'? 'Saved successfully!' : 'Đã lưu thành công!');
    renderMatch();
  } catch(e){
    alert((LANG==='en'? 'Error: ' : 'Lỗi: ') + e);
  }
};
document.getElementById('resetVocab').onclick=()=>{if(confirm(LANG==='en'? 'Reset vocabulary to default?':'Bạn có muốn đặt lại danh sách từ về mặc định?')){vocab = JSON.parse(JSON.stringify(defaultVocab));localStorage.removeItem('vv_vocab');document.getElementById('vocabJson').value=JSON.stringify(vocab,null,2);renderMatch();alert(LANG==='en'? 'Reset to default.':'Đã đặt lại mặc định.');}}

/* ===== init ===== */
renderMatch();
document.getElementById('vocabJson').value = JSON.stringify(vocab,null,2);

/* ===== download handler (safer) ===== */
document.getElementById('downloadBtn').addEventListener('click', (e)=>{
  const blob = new Blob([document.documentElement.outerHTML], {type: 'text/html'});
  const url = URL.createObjectURL(blob);
  e.currentTarget.href = url;
});
</script>
</body>
</html>
