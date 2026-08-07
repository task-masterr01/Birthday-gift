<div class="dock-container">
  <nav class="blocks">
    
    <!-- Button 1 -->
    <a href="#landing" class="block">
      <span class="tooltip">The Beginning</span> <!-- The hover message -->
      <div class="block__item"></div>
    </a>
    
    <!-- Button 2 -->
    <a href="#vault" class="block">
      <span class="tooltip">The Vault</span>
      <div class="block__item"></div>
    </a>
    
    <!-- Button 3 -->
    <a href="#roast" class="block">
      <span class="tooltip">The Roast</span>
      <div class="block__item"></div>
    </a>

  </nav>
</div>

<!-- Example of the sections we will surf to -->
<section id="landing" class="full-screen">Section 1</section>
<section id="vault" class="full-screen">Section 2</section>
<section id="roast" class="full-screen">Section 3</section>


.letter-image.is-open .animated-mail .letter {
  height: 320px; /* Huge vertical space (visually 640px on screen!) */
  width: 300px;  /* Wide horizontal space (visually 600px on screen!) */
  left: -50px;   /* Perfectly centers the big card over the small envelope */
  bottom: 60px;  /* Floats it up and entirely out of the envelope */
  z-index: 20;   /* Jumps in front of all flaps */
  overflow-y: auto; /* MAGIC: Adds a scrollbar if your text is super long! */
  overflow-x: hidden;
  box-shadow: 0 15px 35px rgba(0,0,0,0.25);
  
  /* OPENING ANIMATION: Jumps to front immediately, then gracefully expands */
  transition: bottom 0.4s ease, height 0.5s ease, width 0.5s ease, left 0.5s ease, z-index 0s;
}


/* --- Styling the New Massive Text Area --- */
.long-message {
  padding: 10px 15px;
  font-size: 11px; /* Because of the 2x scale, this will render at a very readable 22px */
  color: #333;
  line-height: 1.6;
  opacity: 0;
  transform: translateY(10px);
  transition: all 0.4s 0.2s ease; /* Fades in slightly after the letter opens */
}

.long-message p {
  margin-bottom: 10px;
}

/* Make the text fade in only when the letter is open */
.letter-image.is-open .animated-mail .letter .long-message {
  opacity: 1;
  transform: translateY(0);
}

/* Cute Custom Scrollbar for the Letter */
.animated-mail .letter::-webkit-scrollbar {
  width: 6px;
}
.animated-mail .letter::-webkit-scrollbar-track {
  background: transparent;
}
.animated-mail .letter::-webkit-scrollbar-thumb {
  background: rgba(255, 117, 140, 0.5); /* Matches the envelope pink */
  border-radius: 10px;
}




.chat-layout {
  display: flex;
  flex-direction: column;
  gap: 10px;
  margin-bottom: 8px;
  border-bottom: 1px dashed rgba(0,0,0,0.1);
  padding-bottom: 10px;
}

.chat-row {
  display: flex;
  align-items: flex-end; /* Aligns avatar to the bottom of the chat stack */
  gap: 4px;
  width: 100%;
}

.right-chat {
  justify-content: flex-end;
}

.chat-avatar {
  width: 16px; /* Renders as 32px on screen */
  height: 16px;
  border-radius: 50%;
  background: #fff;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  padding: 2px;
  object-fit: contain;
  flex-shrink: 0;
}

.chat-bubbles {
  display: flex;
  flex-direction: column;
  gap: 2px;
  max-width: 75%; /* Prevents text from going all the way across */
}

.chat-bubbles p {
  margin: 0;
  padding: 4px 7px; 
  font-size: 5.5px; /* Renders at a super readable 11px */
  line-height: 1.4;
  border-radius: 8px;
  box-shadow: 0 1px 2px rgba(0,0,0,0.05);
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
}

/* --- Left Chat Bubbles (Gray) --- */
.left-chat .chat-bubbles p {
  background: #e5e5ea;
  color: #000;
  /* Authentic chat tail effect */
  border-bottom-left-radius: 2px; 
}
.left-chat .chat-bubbles p:not(:last-child) {
  /* Removes tail from upper messages so they stack cleanly */
  border-bottom-left-radius: 8px; 
}

/* --- Right Chat Bubbles (Pink Gradient) --- */
.right-chat .chat-bubbles p {
  background: linear-gradient(to right, #FF758C, #FF82A9);
  color: #fff;
  align-self: flex-end;
  /* Authentic chat tail effect */
  border-bottom-right-radius: 2px; 
}
.right-chat .chat-bubbles p:not(:last-child) {
  /* Removes tail from upper messages so they stack cleanly */
  border-bottom-right-radius: 8px; 
}




  
            <div class="mid-b">
                <div class="letter-stamp">
                  <!-- <div class="letter-stamp-inner">
                    <img src="https://cdn-icons-png.flaticon.com/512/1864/1864514.png" alt="Cat Stamp">
                  </div> -->
                </div>
                <!-- <div class="letter-context">
                  🎶tum jiyo hazaro saal itni si hai aarzu 🎶🤞😂
                </div> -->
            </div>