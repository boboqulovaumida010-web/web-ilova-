
<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Chatly Messenger</title>

<style>
:root {
 --primary:#6855ed;
 --primary2:#8878ff;
 --bg:#f4f5fb;
 --panel:#fff;
 --text:#24243a;
 --muted:#9295aa;
 --border:#ececf3;
 --hover:#f1efff;
}
*{box-sizing:border-box;margin:0;padding:0;font-family:Arial,sans-serif}
body{background:var(--bg);color:var(--text);height:100vh;overflow:hidden}
body.dark{
 --bg:#111321;--panel:#1b1e30;--text:#f4f4ff;
 --muted:#999db5;--border:#30334a;--hover:#292644;
}
button{cursor:pointer}
.app{height:100vh;padding:12px;display:grid;grid-template-columns:70px 320px 1fr;gap:12px}
.sidebar,.contacts,.chat{background:var(--panel);border-radius:18px;overflow:hidden}
.sidebar{display:flex;align-items:center;flex-direction:column;padding:20px 8px;gap:22px}
.logo{width:44px;height:44px;border-radius:15px;background:linear-gradient(135deg,var(--primary),#a08aff);display:grid;place-items:center;color:white;font-size:23px;font-weight:bold}
.side-btn{width:46px;height:46px;border:0;background:transparent;border-radius:13px;font-size:22px;color:var(--muted)}
.side-btn:hover,.side-btn.active{background:var(--hover);color:var(--primary)}
.side-bottom{margin-top:auto}
.contacts{display:flex;flex-direction:column}
.contact-head{padding:24px 20px 12px}
.contact-head h1{font-size:25px}
.contact-head p{font-size:12px;color:var(--muted);margin-top:7px}
.search{margin:12px 15px;padding:13px;border:1px solid var(--border);background:var(--bg);color:var(--text);border-radius:12px;outline:none}
.primary-btn{margin:0 15px 14px;padding:13px;background:var(--primary);border:0;color:white;border-radius:12px;font-weight:bold}
.contact-list{overflow:auto;flex:1}
.contact{display:flex;align-items:center;gap:12px;padding:14px 15px;cursor:pointer;border-bottom:1px solid var(--border)}
.contact:hover,.contact.active{background:var(--hover)}
.avatar{width:48px;height:48px;flex-shrink:0;border-radius:50%;background:linear-gradient(135deg,#9584ff,#5848d9);display:grid;place-items:center;color:white;font-weight:bold;font-size:18px}
.contact-info{min-width:0;flex:1}
.contact-info h4{font-size:14px;margin-bottom:6px}
.contact-info p{font-size:12px;color:var(--muted);white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.contact-time{font-size:10px;color:var(--muted)}
.chat{display:flex;flex-direction:column;position:relative}
.chat-header{height:78px;display:flex;align-items:center;gap:13px;padding:12px 22px;border-bottom:1px solid var(--border)}
.chat-user{flex:1}
.chat-user h3{font-size:16px;margin-bottom:5px}
.chat-user p{font-size:12px;color:#23b783}
.header-btn{border:0;background:var(--bg);color:var(--text);padding:11px;border-radius:11px;font-size:17px}
.messages{flex:1;overflow:auto;padding:24px;display:flex;flex-direction:column;gap:13px}
.day{text-align:center;font-size:11px;color:var(--muted);padding:10px}
.message{max-width:70%;padding:12px 15px;border-radius:15px;font-size:14px;line-height:1.5;overflow-wrap:anywhere;position:relative}
.received{background:var(--bg);align-self:flex-start;border-bottom-left-radius:4px}
.sent{background:var(--primary);color:white;align-self:flex-end;border-bottom-right-radius:4px}
.message img{max-width:240px;width:100%;border-radius:10px;display:block}
.message-time{display:block;text-align:right;font-size:10px;opacity:.7;margin-top:5px}
.message-tools{display:flex;justify-content:flex-end;gap:5px;margin-top:5px}
.message-tools button{font-size:10px;border:0;background:#ffffff25;color:inherit;padding:3px 6px;border-radius:5px}
.composer{padding:14px 18px;display:flex;gap:9px;align-items:center;border-top:1px solid var(--border)}
.composer input[type=text]{flex:1;min-width:0;padding:14px;border:1px solid var(--border);border-radius:12px;background:var(--bg);color:var(--text);outline:none}
.tool-btn{border:0;background:var(--bg);color:var(--text);padding:12px;border-radius:11px;font-size:19px}
.send-btn{border:0;background:var(--primary);color:white;padding:14px 20px;border-radius:12px;font-size:18px}
.panel{display:none;position:absolute;bottom:80px;left:18px;width:min(330px,90%);max-height:340px;overflow:auto;background:var(--panel);border:1px solid var(--border);box-shadow:0 8px 30px #0002;border-radius:16px;padding:14px;z-index:10}
.panel.open{display:block}
.panel h4{margin:8px 0 12px;font-size:13px}
.emoji-grid,.sticker-grid{display:grid;grid-template-columns:repeat(7,1fr);gap:5px}
.emoji-grid button,.sticker-grid button{border:0;background:var(--bg);border-radius:9px;padding:8px 2px;font-size:22px}
.sticker-grid{grid-template-columns:repeat(4,1fr)}
.sticker-grid button{font-size:32px;padding:12px 3px}
.empty{margin:auto;text-align:center;color:var(--muted);padding:20px}
.empty .big{font-size:55px;margin-bottom:15px}
.mobile-back{display:none}
.modal-bg{position:fixed;inset:0;background:#0008;display:none;align-items:center;justify-content:center;z-index:50;padding:15px}
.modal-bg.open{display:flex}
.modal{width:100%;max-width:390px;background:var(--panel);border-radius:18px;padding:22px}
.modal h2{margin-bottom:17px}
.modal input{width:100%;padding:13px;border:1px solid var(--border);background:var(--bg);color:var(--text);border-radius:10px;margin-bottom:12px;outline:none}
.modal-actions{display:flex;gap:10px}
.modal-actions button{flex:1;padding:12px;border:0;border-radius:10px}
@media(max-width:850px){
 .app{grid-template-columns:55px 260px 1fr;gap:7px;padding:7px}
 .sidebar{padding:15px 4px}
}
@media(max-width:600px){
 body{overflow:hidden}
 .app{display:block;padding:0}
 .sidebar{display:none}
 .contacts{height:100vh;border-radius:0}
 .chat{display:none;height:100vh;border-radius:0}
 body.chat-open .contacts{display:none}
 body.chat-open .chat{display:flex}
 .mobile-back{display:block}
 .messages{padding:14px}
 .chat-header{padding:10px}
 .composer{padding:9px}
 .message{max-width:85%}
 .header-btn{padding:9px}
}
</style>
</head>

<body>
<div class="app">

<aside class="sidebar">
 <div class="logo">C</div>
 <button class="side-btn active" title="Chatlar">💬</button>
 <button class="side-btn" title="Kontaktlar" onclick="newChat()">👥</button>
 <button class="side-btn" title="Mavzu" onclick="toggleTheme()">🌙</button>
 <div class="side-bottom">
  <button class="side-btn" title="Profil" onclick="showProfile()">👤</button>
 </div>
</aside>

<section class="contacts">
 <div class="contact-head">
  <h1>Chatly</h1>
  <p>Har doim aloqada bo‘ling</p>
 </div>

 <input class="search" id="search" placeholder="🔎 Suhbat qidirish..." oninput="renderContacts()">
 <button class="primary-btn" onclick="newChat()">＋ Yangi suhbat</button>
 <div class="contact-list" id="contactList"></div>
</section>

<main class="chat">
 <header class="chat-header">
  <button class="header-btn mobile-back" onclick="backChats()">←</button>
  <div class="avatar" id="headAvatar">C</div>
  <div class="chat-user">
   <h3 id="headName">Chatly</h3>
   <p id="headStatus">● Suhbatni tanlang</p>
  </div>
  <button class="header-btn" onclick="showInfo()">ⓘ</button>
  <button class="header-btn" onclick="toggleTheme()">🌙</button>
 </header>

 <div class="messages" id="messages">
  <div class="empty"><div class="big">💬</div><h2>Chatly Messenger</h2><p>Suhbatni tanlang yoki yangi suhbat boshlang</p></div>
 </div>

 <div class="panel" id="emojiPanel">
  <h4>😊 Emojilar</h4>
  <div class="emoji-grid" id="emojiGrid"></div>
  <h4>🎨 Stikerlar</h4>
  <div class="sticker-grid" id="stickerGrid"></div>
 </div>

 <div class="composer">
  <button class="tool-btn" title="Fayl biriktirish" onclick="document.getElementById('imageFile').click()">📎</button>
  <input type="file" id="imageFile" accept="image/*" hidden onchange="sendImage(event)">
  <button class="tool-btn" title="Emoji va stikerlar" onclick="toggleEmoji()">😊</button>
  <input type="text" id="messageInput" placeholder="Xabaringizni yozing..." onkeydown="if(event.key==='Enter')sendMessage()">
  <button class="send-btn" onclick="sendMessage()">➤</button>
 </div>
</main>
</div>

<div class="modal-bg" id="newModal">
 <div class="modal">
  <h2>Yangi suhbat</h2>
  <input id="newName" placeholder="Ismni kiriting">
  <div class="modal-actions">
   <button onclick="closeModal()" style="background:var(--bg);color:var(--text)">Bekor qilish</button>
   <button onclick="createChat()" style="background:var(--primary);color:white">Yaratish</button>
  </div>
 </div>
</div>

<script>
const initialChats = [
 {id:1,name:"Azizbek Karimov",last:"Salom! Qalaysan?",messages:[
  {id:11,text:"Assalomu alaykum! 😊",type:"received",time:"09:30"},
  {id:12,text:"Va alaykum assalom!",type:"sent",time:"09:32"}
 ]},
 {id:2,name:"Madina",last:"Yaxshi, rahmat ❤️",messages:[
  {id:21,text:"Bugun vaqting bormi?",type:"received",time:"10:10"},
  {id:22,text:"Ha, albatta!",type:"sent",time:"10:12"}
 ]},
 {id:3,name:"Javohir",last:"Ko‘rishguncha",messages:[
  {id:31,text:"Salom, ishlaring yaxshimi?",type:"received",time:"11:00"}
 ]},
 {id:4,name:"Diyora",last:"Rahmat 🌹",messages:[
  {id:41,text:"Yangi loyiha qanday ketyapti?",type:"received",time:"11:30"}
 ]}
];

let chats;
try{
 chats=JSON.parse(localStorage.getItem("chatly_data")) || initialChats;
 if(!Array.isArray(chats)) chats=initialChats;
}catch(e){chats=initialChats;}

let activeId=null;

function save(){
 localStorage.setItem("chatly_data",JSON.stringify(chats));
}

function currentChat(){
 return chats.find(c=>c.id===activeId);
}

function timeNow(){
 return new Date().toLocaleTimeString("uz-UZ",{hour:"2-digit",minute:"2-digit"});
}

function safeText(text){
 return String(text);
}

function renderContacts(){
 const list=document.getElementById("contactList");
 const query=document.getElementById("search").value.toLowerCase();
 list.innerHTML="";

 chats.filter(c=>c.name.toLowerCase().includes(query)).forEach(c=>{
  const div=document.createElement("div");
  div.className="contact"+(c.id===activeId?" active":"");

  const avatar=document.createElement("div");
  avatar.className="avatar";
  avatar.textContent=c.name.charAt(0).toUpperCase();

  const info=document.createElement("div");
  info.className="contact-info";

  const name=document.createElement("h4");
  name.textContent=c.name;

  const last=document.createElement("p");
  last.textContent=c.last||"Yangi suhbat";

  info.append(name,last);
  div.append(avatar,info);
  div.onclick=()=>openChat(c.id);
  list.append(div);
 });
}

function openChat(id){
 activeId=id;
 const chat=currentChat();
 if(!chat)return;

 document.body.classList.add("chat-open");
 document.getElementById("headName").textContent=chat.name;
 document.getElementById("headAvatar").textContent=chat.name.charAt(0).toUpperCase();
 document.getElementById("headStatus").textContent="● Lokal suhbat";
 document.getElementById("emojiPanel").classList.remove("open");
 renderContacts();
 renderMessages();
}

function renderMessages(){
 const box=document.getElementById("messages");
 const chat=currentChat();
 if(!chat)return;

 box.innerHTML="";
 const day=document.createElement("div");
 day.className="day";
 day.textContent="Suhbat xabarlari";
 box.append(day);

 chat.messages.forEach(m=>{
  const div=document.createElement("div");
  div.className="message "+m.type;

  if(m.image){
   const img=document.createElement("img");
   img.src=m.image;
   img.alt="Yuborilgan rasm";
   div.append(img);
  }else{
   div.append(document.createTextNode(safeText(m.text)));
  }

  const time=document.createElement("span");
  time.className="message-time";
  time.textContent=(m.time||"")+(m.type==="sent"?" ✓✓":"");
  div.append(time);

  if(m.type==="sent"){
   const tools=document.createElement("div");
   tools.className="message-tools";
   const del=document.createElement("button");
   del.textContent="O‘chirish";
   del.onclick=()=>deleteMessage(m.id);
   tools.append(del);
   div.append(tools);
  }
  box.append(div);
 });
 box.scrollTop=box.scrollHeight;
}

function sendMessage(){
 const input=document.getElementById("messageInput");
 const text=input.value.trim();
 const chat=currentChat();

 if(!chat){
  alert("Avval suhbatni tanlang yoki yangi suhbat yarating.");
  return;
 }
 if(!text)return;

 chat.messages.push({
  id:Date.now()+Math.random(),
  text:text,
  type:"sent",
  time:timeNow()
 });
 chat.last=text;
 input.value="";
 save();
 renderMessages();
 renderContacts();
}

function sendSticker(sticker){
 const chat=currentChat();
 if(!chat){
  alert("Avval suhbatni tanlang.");
  return;
 }
 chat.messages.push({
  id:Date.now()+Math.random(),
  text:sticker,
  type:"sent",
  time:timeNow()
 });
 chat.last=sticker;
 save();
 renderMessages();
 renderContacts();
 document.getElementById("emojiPanel").classList.remove("open");
}

function deleteMessage(id){
 const chat=currentChat();
 if(!chat)return;
 if(!confirm("Xabarni o‘chirasizmi?"))return;
 chat.messages=chat.messages.filter(m=>m.id!==id);
 chat.last=chat.messages.length?chat.messages[chat.messages.length-1].text||"📷 Rasm":"";
 save();
 renderMessages();
 renderContacts();
}

function sendImage(event){
 const file=event.target.files[0];
 if(!file)return;

 if(!file.type.startsWith("image/")){
  alert("Faqat rasm tanlang.");
  event.target.value="";
  return;
 }
 if(file.size>2*1024*1024){
  alert("Rasm 2 MB dan kichik bo‘lishi kerak.");
  event.target.value="";
  return;
 }

 const chat=currentChat();
 if(!chat){
  alert("Avval suhbatni tanlang.");
  event.target.value="";
  return;
 }

 const reader=new FileReader();
 reader.onload=()=>{
  chat.messages.push({
   id:Date.now()+Math.random(),
   image:reader.result,
   type:"sent",
   time:timeNow()
  });
  chat.last="📷 Rasm";
  save();
  renderMessages();
  renderContacts();
  event.target.value="";
 };
 reader.readAsDataURL(file);
}

function toggleEmoji(){
 document.getElementById("emojiPanel").classList.toggle("open");
}

function insertEmoji(emoji){
 const input=document.getElementById("messageInput");
 input.value+=emoji;
 input.focus();
}

const emojis=[
"😀","😃","😄","😁","😆","😅","😂","🤣",
"😊","😇","🙂","😉","😍","🥰","😘","😋",
"😎","🤩","🥳","😏","😭","🥺","😢","😡",
"🤯","😴","🤗","🤔","😱","😇","🤭","🤫",
"❤️","🧡","💛","💚","💙","💜","🖤","🤍",
"💕","💞","💓","💗","💖","💘","💝","💌",
"👍","👎","👏","🙌","🤝","🙏","💪","👋",
"🌹","🌸","🌺","🌷","🌻","⭐","✨","🔥",
"🎉","🎊","🎁","🎂","🎈","☀️","🌙","☕"
];

const stickers=[
"🥰","😍","😘","❤️","💕","💖","💗","💝",
"😂","🤣","😭","🥺","🤗","😎","😻","🙈",
"🌹","🌷","🦋","🐻","🐼","🐱","🐰","🐸",
"🎉","🎂","🎁","💐","👑","✨","🔥","🙏",
"👍","👏","🤝","💪","💋","💌","🌈","⭐"
];

function buildPickers(){
 const emojiGrid=document.getElementById("emojiGrid");
 const stickerGrid=document.getElementById("stickerGrid");

 emojis.forEach(e=>{
  const b=document.createElement("button");
  b.type="button";
  b.textContent=e;
  b.onclick=()=>insertEmoji(e);
  emojiGrid.append(b);
 });

 stickers.forEach(s=>{
  const b=document.createElement("button");
  b.type="button";
  b.textContent=s;
  b.onclick=()=>sendSticker(s);
  stickerGrid.append(b);
 });
}

function newChat(){
 document.getElementById("newModal").classList.add("open");
 document.getElementById("newName").value="";
 document.getElementById("newName").focus();
}

function closeModal(){
 document.getElementById("newModal").classList.remove("open");
}

function createChat(){
 const input=document.getElementById("newName");
 const name=input.value.trim();
 if(!name){
  alert("Ismni kiriting.");
  return;
 }

 if(chats.some(c=>c.name.toLowerCase()===name.toLowerCase())){
  alert("Bu suhbat mavjud.");
  return;
 }

 const chat={
  id:Date.now(),
  name:name,
  last:"Yangi suhbat",
  messages:[]
 };
 chats.unshift(chat);
 save();
 closeModal();
 renderContacts();
 openChat(chat.id);
}

function toggleTheme(){
 document.body.classList.toggle("dark");
 localStorage.setItem("chatly_theme",document.body.classList.contains("dark")?"dark":"light");
}

function backChats(){
 document.body.classList.remove("chat-open");
}

function showInfo(){
 const chat=currentChat();
 if(chat)alert("Suhbat: "+chat.name+"\nXabarlar: "+chat.messages.length);
}

function showProfile(){
 alert("Chatly profil\nLokal demo versiyasi");
}

document.getElementById("newName").addEventListener("keydown",e=>{
 if(e.key==="Enter")createChat();
});

document.addEventListener("click",e=>{
 const panel=document.getElementById("emojiPanel");
 if(!panel.contains(e.target)&&!e.target.closest('[title="Emoji va stikerlar"]')){
  panel.classList.remove("open");
 }
});

if(localStorage.getItem("chatly_theme")==="dark"){
 document.body.classList.add("dark");
}

buildPickers();
renderContacts();
</script>
</body>
</html>
