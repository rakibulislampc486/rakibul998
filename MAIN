<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes, viewport-fit=cover">
    <title>Heartfelt Quest | RAKIBUL IT</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            min-height: 100vh;
            background: linear-gradient(145deg, #fbc2eb 0%, #a6c1ee 100%);
            font-family: 'Segoe UI', 'Poppins', 'Quicksand', system-ui, -apple-system, 'Helvetica Neue', sans-serif;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 16px;
            transition: all 0.3s ease;
            animation: bgPulse 8s infinite alternate;
            position: relative;
        }

        @keyframes bgPulse {
            0% {
                background: linear-gradient(145deg, #ff9a9e, #fad0c4);
            }
            50% {
                background: linear-gradient(145deg, #fbc2eb, #a1c4fd);
            }
            100% {
                background: linear-gradient(145deg, #ffdde1, #ee9ca7);
            }
        }

        /* main glass card container - fully responsive */
        .card {
            background: rgba(255, 255, 255, 0.25);
            backdrop-filter: blur(20px);
            border-radius: 2rem;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2), 0 0 0 1px rgba(255, 255, 255, 0.3);
            width: 100%;
            max-width: 500px;
            margin: 0 auto;
            padding: 1.8rem 1.5rem;
            text-align: center;
            transition: transform 0.3s ease;
            animation: floatGlow 3s infinite ease-in-out;
        }

        @keyframes floatGlow {
            0% {
                transform: translateY(0px);
                box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
            }
            100% {
                transform: translateY(-6px);
                box-shadow: 0 30px 50px rgba(0, 0, 0, 0.25);
            }
        }

        h1 {
            font-size: clamp(1.8rem, 7vw, 2.4rem);
            font-weight: 700;
            background: linear-gradient(135deg, #fff5e6, #ffe6f0);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            text-shadow: 0 2px 5px rgba(0,0,0,0.1);
            margin-bottom: 0.5rem;
            letter-spacing: -0.3px;
        }

        .question {
            font-size: clamp(1.3rem, 5vw, 1.9rem);
            font-weight: 700;
            margin: 1.2rem 0 1rem;
            color: #2d1b3c;
            background: rgba(255,248,225,0.85);
            display: inline-block;
            padding: 0.4rem 1.2rem;
            border-radius: 60px;
            backdrop-filter: blur(4px);
            line-height: 1.3;
        }

        .options {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin: 1.5rem 0;
            flex-wrap: wrap;
        }

        /* fancy touch-friendly labels */
        .choice-label {
            background: rgba(30, 20, 40, 0.75);
            backdrop-filter: blur(8px);
            border-radius: 60px;
            padding: 0.7rem 1.6rem;
            cursor: pointer;
            transition: all 0.2s ease;
            font-weight: 600;
            font-size: clamp(1rem, 4.5vw, 1.3rem);
            color: white;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            box-shadow: 0 6px 14px rgba(0,0,0,0.2);
            border: 1px solid rgba(255,255,255,0.5);
            min-width: 110px;
            justify-content: center;
        }

        .choice-label:active {
            transform: scale(0.97);
            background: rgba(80, 50, 100, 0.9);
        }

        input[type="checkbox"] {
            width: 22px;
            height: 22px;
            accent-color: #ff6b9d;
            cursor: pointer;
            transform: scale(1.05);
            margin: 0;
            flex-shrink: 0;
        }

        .hidden-page {
            display: none;
        }

        .active-page {
            display: block;
            animation: fadeSlideUp 0.5s cubic-bezier(0.2, 0.9, 0.4, 1.1);
        }

        @keyframes fadeSlideUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .next-btn, .reset-btn {
            border: none;
            font-family: inherit;
            font-weight: bold;
            border-radius: 60px;
            cursor: pointer;
            transition: all 0.2s ease;
            width: 85%;
            max-width: 280px;
            padding: 12px 20px;
            font-size: 1.1rem;
            letter-spacing: 0.5px;
            margin-top: 1rem;
        }

        .next-btn {
            background: linear-gradient(95deg, #ff8a5c, #ff4d6d);
            color: white;
            box-shadow: 0 8px 18px rgba(0,0,0,0.25);
        }

        .next-btn:active {
            transform: scale(0.97);
            background: linear-gradient(95deg, #ff6a3a, #ff2f5e);
        }

        .reset-btn {
            background: rgba(0, 0, 0, 0.45);
            backdrop-filter: blur(4px);
            border: 1px solid rgba(255,255,240,0.8);
            color: white;
        }

        .reset-btn:active {
            transform: scale(0.96);
            background: rgba(0, 0, 0, 0.7);
        }

        /* LOVE animation */
        .love-message {
            font-size: clamp(2rem, 10vw, 4rem);
            font-weight: 900;
            background: linear-gradient(45deg, #ff0844, #ffb199);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            animation: heartbeat 1.2s infinite, glitchLove 2.8s infinite;
            margin: 20px 0;
            letter-spacing: 2px;
        }

        @keyframes heartbeat {
            0% { transform: scale(1); opacity: 1; text-shadow: 0 0 0px #ff2e6b; }
            50% { transform: scale(1.15); text-shadow: 0 0 18px #ff2e6b; }
            100% { transform: scale(1); opacity: 1; }
        }

        @keyframes glitchLove {
            0%, 100% { letter-spacing: 2px; filter: blur(0);}
            5% { letter-spacing: 6px; filter: blur(0.6px);}
            10% { letter-spacing: 1px; filter: blur(0);}
        }

        .respect-message {
            font-size: clamp(1.2rem, 5vw, 1.8rem);
            font-weight: 700;
            background: #fff9e8;
            display: inline-block;
            padding: 0.8rem 1.2rem;
            border-radius: 60px;
            color: #3a2a3f;
            margin: 1.5rem 0;
            box-shadow: 0 8px 18px rgba(0,0,0,0.1);
            word-break: break-word;
        }

        .instruction {
            font-size: 0.75rem;
            opacity: 0.85;
            margin-top: 0.8rem;
            color: #2c1a33;
            background: rgba(255,245,230,0.5);
            display: inline-block;
            padding: 4px 12px;
            border-radius: 30px;
        }

        /* floating hearts / particles */
        .heart-emoji {
            position: absolute;
            font-size: 1.6rem;
            animation: floatUpMobile 1.8s ease-out forwards;
            pointer-events: none;
        }

        @keyframes floatUpMobile {
            0% {
                transform: translateY(0) scale(0.8);
                opacity: 1;
            }
            100% {
                transform: translateY(-90px) scale(1.2);
                opacity: 0;
            }
        }

        .float-area {
            position: relative;
            height: 100px;
            width: 100%;
            margin: 10px 0;
            overflow: hidden;
        }

        /* Footer - RAKIBUL IT */
        .footer {
            position: fixed;
            bottom: 0;
            left: 0;
            width: 100%;
            text-align: center;
            padding: 10px 16px;
            background: rgba(0, 0, 0, 0.65);
            backdrop-filter: blur(12px);
            color: #fff5e6;
            font-size: 0.8rem;
            font-weight: 500;
            z-index: 200;
            border-top: 1px solid rgba(255, 200, 180, 0.6);
            letter-spacing: 0.5px;
        }

        .footer span.highlight {
            background: linear-gradient(135deg, #ffd89b, #ffb77c);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            font-weight: bold;
            font-size: 0.85rem;
        }

        .footer .heart-beat {
            display: inline-block;
            animation: footHeart 1s infinite;
            margin: 0 4px;
        }

        @keyframes footHeart {
            0%,100%{ transform: scale(1);}
            50%{ transform: scale(1.2); color: #ff6680; }
        }

        /* prevent footer overlapping content */
        body {
            padding-bottom: 70px;
        }

        /* mobile extra tuning */
        @media (max-width: 550px) {
            .card {
                padding: 1.3rem 1.2rem;
                border-radius: 1.8rem;
            }
            .choice-label {
                padding: 0.6rem 1.2rem;
                min-width: 95px;
            }
            .next-btn, .reset-btn {
                width: 90%;
                padding: 10px 16px;
                font-size: 1rem;
            }
            .footer {
                font-size: 0.7rem;
                padding: 7px 12px;
            }
        }

        @media (max-width: 400px) {
            .options {
                gap: 0.7rem;
            }
            .choice-label {
                padding: 0.5rem 0.9rem;
                font-size: 0.9rem;
            }
        }

        button {
            cursor: pointer;
        }
    </style>
</head>
<body>

<div class="card" id="appRoot">
    <!-- PAGE 1: ARE YOU SINGLE? -->
    <div id="page1" class="active-page">
        <h1>✨ Heart Compass ✨</h1>
        <div class="question">💖 ARE YOU SINGLE ? 💖</div>
        <div class="options">
            <label class="choice-label">
                <input type="checkbox" name="singleOption" value="yes" id="singleYes"> YES 💘
            </label>
            <label class="choice-label">
                <input type="checkbox" name="singleOption" value="no" id="singleNo"> NO 💔
            </label>
        </div>
        <div class="instruction">✨ choose one, follow your heart ✨</div>
        <button class="next-btn" id="proceedBtn">→ Continue →</button>
        <div class="instruction" style="margin-top: 18px;">🌸 a magical journey awaits 🌸</div>
    </div>

    <!-- PAGE 2: ARE YOU WANT TO LOVE ME? -->
    <div id="page2" class="hidden-page">
        <h1>🌹 Deeper Feelings 🌹</h1>
        <div class="question">💞 ARE YOU WANT TO LOVE ME? 💞</div>
        <div class="options">
            <label class="choice-label">
                <input type="checkbox" name="loveOption" value="yes" id="loveYes"> YES ❤️‍🔥
            </label>
            <label class="choice-label">
                <input type="checkbox" name="loveOption" value="no" id="loveNo"> NO 🚫
            </label>
        </div>
        <div class="instruction">💭 whisper your true feeling 💭</div>
        <button class="next-btn" id="decideLoveBtn">✨ Reveal destiny ✨</button>
        <button class="reset-btn" id="resetFromPage2">↺ Start Over</button>
    </div>

    <!-- PAGE 3: FINAL RESULT (animated / respectful) -->
    <div id="page3" class="hidden-page">
        <div id="resultContent"></div>
        <button class="reset-btn" id="resetFromResult">⟳ Begin Again</button>
    </div>
</div>

<!-- FOOTER: PROJECT FROM RAKIBUL IT -->
<div class="footer">
    <span class="highlight">✨ THIS PROJECT FROM RAKIBUL IT ✨</span> 
    <span class="heart-beat">❤️</span> 
    <span style="opacity:0.9;">| spreading love & code</span>
</div>

<script>
    // DOM elements
    const page1 = document.getElementById('page1');
    const page2 = document.getElementById('page2');
    const page3 = document.getElementById('page3');
    const proceedBtn = document.getElementById('proceedBtn');
    const decideLoveBtn = document.getElementById('decideLoveBtn');
    const resetFromPage2 = document.getElementById('resetFromPage2');
    const resetFromResult = document.getElementById('resetFromResult');
    const singleYes = document.getElementById('singleYes');
    const singleNo = document.getElementById('singleNo');
    const loveYes = document.getElementById('loveYes');
    const loveNo = document.getElementById('loveNo');

    // Helper: switch pages with smooth transition
    function showPage(pageNum) {
        [page1, page2, page3].forEach(page => {
            page.classList.remove('active-page');
            page.classList.add('hidden-page');
        });
        let target;
        if (pageNum === 1) target = page1;
        else if (pageNum === 2) target = page2;
        else target = page3;
        target.classList.remove('hidden-page');
        target.classList.add('active-page');
    }

    // full reset to initial state
    function fullReset() {
        singleYes.checked = false;
        singleNo.checked = false;
        loveYes.checked = false;
        loveNo.checked = false;
        showPage(1);
        const resultDiv = document.getElementById('resultContent');
        if (resultDiv) resultDiv.innerHTML = '';
        // remove any floating warning leftovers
        document.querySelectorAll('.temp-warning, .polite-no-msg, .single-warning').forEach(el => el.remove());
    }

    // get single status (null if invalid)
    function getSingleStatus() {
        const yes = singleYes.checked;
        const no = singleNo.checked;
        if ((yes && no) || (!yes && !no)) return null;
        return yes ? 'yes' : 'no';
    }

    function getLoveDecision() {
        const yes = loveYes.checked;
        const no = loveNo.checked;
        if ((yes && no) || (!yes && !no)) return null;
        return yes ? 'yes' : 'no';
    }

    // floating hearts creator (mobile optimized)
    function spawnFloatingHearts(containerEl, count = 16) {
        if (!containerEl) return;
        const oldHearts = containerEl.querySelectorAll('.dynamic-heart');
        oldHearts.forEach(h => h.remove());
        for (let i = 0; i < count; i++) {
            const heart = document.createElement('div');
            heart.classList.add('heart-emoji', 'dynamic-heart');
            const heartsList = ['❤️', '💖', '💗', '💓', '💘', '💕', '💞', '❣️', '🧡'];
            heart.innerHTML = heartsList[i % heartsList.length];
            heart.style.position = 'absolute';
            heart.style.left = `${Math.random() * 100}%`;
            heart.style.bottom = '0px';
            heart.style.fontSize = `${1 + Math.random() * 1.8}rem`;
            heart.style.animationDuration = `${1.2 + Math.random() * 1.6}s`;
            heart.style.animationDelay = `${i * 0.08}s`;
            heart.style.opacity = '0.9';
            containerEl.appendChild(heart);
            setTimeout(() => {
                if (heart && heart.remove) heart.remove();
            }, 2200);
        }
    }

    function createSparkles(parent) {
        const sparkContainer = document.createElement('div');
        sparkContainer.style.position = 'relative';
        sparkContainer.style.height = '70px';
        sparkContainer.style.margin = '8px 0';
        for (let i = 0; i < 24; i++) {
            const star = document.createElement('div');
            star.innerHTML = '✨';
            star.style.position = 'absolute';
            star.style.left = `${Math.random() * 100}%`;
            star.style.top = `${Math.random() * 100}%`;
            star.style.fontSize = `${0.8 + Math.random() * 1.2}rem`;
            star.style.animation = `floatUpMobile 1.5s ease-out forwards`;
            star.style.animationDelay = `${i * 0.07}s`;
            star.style.opacity = '0.8';
            sparkContainer.appendChild(star);
            setTimeout(() => star.remove(), 1800);
        }
        parent.appendChild(sparkContainer);
        setTimeout(() => sparkContainer.remove(), 2000);
    }

    // I LOVE YOU animated page (full of love)
    function renderLovePage() {
        const container = document.getElementById('resultContent');
        if (!container) return;
        container.innerHTML = '';

        const loveWrapper = document.createElement('div');
        loveWrapper.style.textAlign = 'center';
        loveWrapper.style.animation = 'fadeSlideUp 0.4s ease';

        const loveText = document.createElement('div');
        loveText.className = 'love-message';
        loveText.innerText = '✨ I LOVE YOU ✨';

        const sub = document.createElement('div');
        sub.style.fontSize = 'clamp(1rem, 4vw, 1.3rem)';
        sub.style.margin = '15px 0';
        sub.style.background = 'rgba(255,245,240,0.85)';
        sub.style.display = 'inline-block';
        sub.style.padding = '0.5rem 1rem';
        sub.style.borderRadius = '50px';
        sub.style.backdropFilter = 'blur(4px)';
        sub.innerHTML = '💗 You make my heart dance 💗';

        const floatArea = document.createElement('div');
        floatArea.className = 'float-area';
        floatArea.style.height = '110px';

        loveWrapper.appendChild(loveText);
        loveWrapper.appendChild(sub);
        loveWrapper.appendChild(floatArea);
        container.appendChild(loveWrapper);

        // spawn multiple heart bursts
        spawnFloatingHearts(floatArea, 18);
        setTimeout(() => spawnFloatingHearts(floatArea, 14), 700);
        setTimeout(() => spawnFloatingHearts(floatArea, 12), 1500);
        createSparkles(container);
        
        // extra shake of joy
        const heartCard = document.querySelector('.card');
        if (heartCard) {
            heartCard.style.animation = 'none';
            setTimeout(() => heartCard.style.animation = 'floatGlow 3s infinite ease-in-out', 100);
        }
    }

    // Respectful message for "NO"
    function renderRespectPage() {
        const container = document.getElementById('resultContent');
        if (!container) return;
        container.innerHTML = '';

        const wrapper = document.createElement('div');
        wrapper.style.textAlign = 'center';
        wrapper.style.animation = 'gentleFade 0.5s ease';

        const icon = document.createElement('div');
        icon.innerHTML = '🤝💫';
        icon.style.fontSize = '3.5rem';
        icon.style.margin = '10px 0';

        const message = document.createElement('div');
        message.className = 'respect-message';
        message.innerHTML = `💙 ITS OKAY. I ALWAYS RESPECT YOUR DECISION 💙`;
        message.style.fontSize = 'clamp(1rem, 4.5vw, 1.5rem)';

        const extra = document.createElement('div');
        extra.style.marginTop = '15px';
        extra.style.fontSize = '1rem';
        extra.style.background = 'rgba(255,250,210,0.9)';
        extra.style.padding = '0.4rem 1rem';
        extra.style.borderRadius = '2rem';
        extra.innerHTML = '🌷 Sending you warmth & kindness 🌷';

        wrapper.appendChild(icon);
        wrapper.appendChild(message);
        wrapper.appendChild(extra);
        container.appendChild(wrapper);

        // peaceful floating flowers & stars
        const peacefulArea = document.createElement('div');
        peacefulArea.style.position = 'relative';
        peacefulArea.style.height = '80px';
        peacefulArea.style.margin = '10px 0';
        for (let i = 0; i < 18; i++) {
            const particle = document.createElement('div');
            const icons = ['🌸', '🌼', '⭐', '💫', '🍃', '🌿'];
            particle.innerHTML = icons[i % icons.length];
            particle.style.position = 'absolute';
            particle.style.left = `${Math.random() * 100}%`;
            particle.style.bottom = '0px';
            particle.style.fontSize = '1.2rem';
            particle.style.animation = `floatUpMobile ${1.8 + Math.random() * 1.5}s ease-out forwards`;
            particle.style.animationDelay = `${i * 0.1}s`;
            particle.style.opacity = '0.75';
            peacefulArea.appendChild(particle);
            setTimeout(() => particle.remove(), 2500);
        }
        container.appendChild(peacefulArea);
    }

    // handle final decision on page2
    function handleLoveFinal() {
        const decision = getLoveDecision();
        if (decision === null) {
            const warn = document.createElement('div');
            warn.innerText = '💭 Please select either YES or NO 💭';
            warn.className = 'temp-warning';
            warn.style.background = '#fff0d4';
            warn.style.padding = '8px 14px';
            warn.style.borderRadius = '40px';
            warn.style.margin = '8px auto';
            warn.style.fontSize = '0.85rem';
            warn.style.fontWeight = '500';
            const oldWarn = document.querySelector('.temp-warning');
            if (oldWarn) oldWarn.remove();
            page2.insertBefore(warn, page2.querySelector('.options').nextSibling);
            setTimeout(() => warn.remove(), 1900);
            return;
        }

        if (decision === 'yes') {
            renderLovePage();
        } else {
            renderRespectPage();
        }
        showPage(3);
    }

    // proceed from page1 to page2 only if single status = YES
    function goToPage2IfSingle() {
        const status = getSingleStatus();
        if (status === null) {
            const warnDiv = document.createElement('div');
            warnDiv.innerText = '💕 Please select either YES or NO (one only) 💕';
            warnDiv.style.background = '#fff5e6';
            warnDiv.style.padding = '0.5rem 1rem';
            warnDiv.style.borderRadius = '2rem';
            warnDiv.style.marginTop = '12px';
            warnDiv.style.fontSize = '0.8rem';
            warnDiv.className = 'single-warning';
            const oldWarn = document.querySelector('.single-warning');
            if (oldWarn) oldWarn.remove();
            page1.appendChild(warnDiv);
            setTimeout(() => warnDiv.remove(), 2000);
            return;
        }

        if (status === 'yes') {
            // reset love checkboxes for fresh decision
            loveYes.checked = false;
            loveNo.checked = false;
            showPage(2);
        } else {
            // polite message for "NO" single status, stay on page1
            const noMsg = document.createElement('div');
            noMsg.innerText = '🌸 Thanks for your honesty! This path is for singles, but you are always valued. 🌸';
            noMsg.style.background = 'rgba(0,0,0,0.55)';
            noMsg.style.backdropFilter = 'blur(10px)';
            noMsg.style.borderRadius = '60px';
            noMsg.style.padding = '10px 16px';
            noMsg.style.marginTop = '16px';
            noMsg.style.fontSize = '0.8rem';
            noMsg.style.fontWeight = '500';
            noMsg.className = 'polite-no-msg';
            const existing = document.querySelector('.polite-no-msg');
            if (existing) existing.remove();
            page1.appendChild(noMsg);
            setTimeout(() => noMsg.remove(), 2800);
        }
    }

    // Event listeners
    proceedBtn.addEventListener('click', goToPage2IfSingle);
    decideLoveBtn.addEventListener('click', handleLoveFinal);
    resetFromPage2.addEventListener('click', fullReset);
    resetFromResult.addEventListener('click', fullReset);

    // Mutual exclusivity for checkboxes
    function exclusiveGroup(a, b) {
        a.addEventListener('change', () => { if (a.checked) b.checked = false; });
        b.addEventListener('change', () => { if (b.checked) a.checked = false; });
    }
    exclusiveGroup(singleYes, singleNo);
    exclusiveGroup(loveYes, loveNo);

    // start clean
    fullReset();
</script>
</body>
</html>
