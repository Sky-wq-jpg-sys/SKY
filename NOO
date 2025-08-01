<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Happy Birthday Darling!!</title>
    <style>
        body {
            background: linear-gradient(135deg, #f9d423 0%, #ff4e50 100%);
            font-family: 'Segoe UI', sans-serif;
            text-align: center;
            color: #fff;
            margin: 0;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }
        h1 {
            font-size: 3em;
            margin-top: 40px;
        }
        #balloons {
            margin: 30px 0;
        }
        .balloon {
            display: inline-block;
            width: 60px;
            height: 80px;
            background: radial-gradient(circle at 30% 30%, #fff 10%, #ff6f91 80%);
            border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
            margin: 0 10px;
            position: relative;
            cursor: pointer;
            transition: transform 0.2s;
        }
        .balloon.popped {
            opacity: 0.2;
            transform: scale(0.7);
            background: #ccc;
        }
        .balloon::after {
            content: '';
            display: block;
            position: absolute;
            left: 50%;
            bottom: -30px;
            width: 2px;
            height: 30px;
            background: #fff;
            transform: translateX(-50%);
        }
        #wish {
            margin-top: 30px;
            font-size: 1.5em;
            opacity: 0;
            transition: opacity 1s;
        }
        button {
            margin-top: 40px;
            padding: 12px 28px;
            font-size: 1.1em;
            border: none;
            border-radius: 25px;
            background: #ff6f91;
            color: #fff;
            cursor: pointer;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            transition: background 0.2s;
        }
        button:hover {
            background: #f9d423;
            color: #ff4e50;
        }
    </style>
</head>
<body>
    <h1> Happy Birthday! Darling </h1>
    <div id="balloons">
        <div class="balloon" data-color="#ff6f91"></div>
        <div class="balloon" data-color="#f9d423"></div>
        <div class="balloon" data-color="#6a89cc"></div>
        <div class="balloon" data-color="#38ada9"></div>
        <div class="balloon" data-color="#b33771"></div>
    </div>
    <div id="wish">Wishing you a day filled with joy and surprises! </div>
    <button id="resetBtn" style="display:none;">Reset Balloons</button>
    <script>
        const balloons = document.querySelectorAll('.balloon');
        const wish = document.getElementById('wish');
        const resetBtn = document.getElementById('resetBtn');
        let poppedCount = 0;

        balloons.forEach((balloon, idx) => {
            // Set balloon color
            balloon.style.background = `radial-gradient(circle at 30% 30%, #fff 10%, ${balloon.dataset.color} 80%)`;
            balloon.addEventListener('click', function() {
                if (!balloon.classList.contains('popped')) {
                    balloon.classList.add('popped');
                    poppedCount++;
                    if (poppedCount === balloons.length) {
                        wish.style.opacity = 1;
                        resetBtn.style.display = 'inline-block';
                    }
                }
            });
        });

        resetBtn.addEventListener('click', () => {
            balloons.forEach(balloon => balloon.classList.remove('popped'));
            wish.style.opacity = 0;
            resetBtn.style.display = 'none';
            poppedCount = 0;
        });
    </script>
</body>
</html>
<!-- Fancy cakes at the bottom -->
<style>
    #cakes {
        display: flex;
        justify-content: center;
        gap: 30px;
        margin: 40px 0 20px 0;
    }
    .cake {
        width: 70px;
        height: 90px;
        position: relative;
        display: flex;
        flex-direction: column;
        align-items: center;
        animation: bounce 2s infinite alternate;
    }
    .cake-base {
        width: 60px;
        height: 40px;
        background: linear-gradient(#fffbe7 60%, #ffb347 100%);
        border-radius: 0 0 18px 18px;
        border: 2px solid #fff;
        box-shadow: 0 4px 10px rgba(0,0,0,0.08);
        position: absolute;
        bottom: 0;
        z-index: 1;
    }
    .cake-icing {
        width: 60px;
        height: 18px;
        background: linear-gradient(90deg, #ff6f91 60%, #f9d423 100%);
        border-radius: 18px 18px 12px 12px;
        position: absolute;
        top: -10px;
        left: 0;
        z-index: 2;
    }
    .candle {
        width: 6px;
        height: 22px;
        background: #fff;
        border-radius: 3px;
        position: absolute;
        top: -28px;
        left: 50%;
        transform: translateX(-50%);
        z-index: 3;
        box-shadow: 0 0 2px #ff6f91;
    }
    .flame {
        width: 10px;
        height: 14px;
        background: radial-gradient(ellipse at center, #fffbe7 60%, #ffb347 100%);
        border-radius: 50% 50% 60% 60%;
        position: absolute;
        top: -36px;
        left: 50%;
        transform: translateX(-50%);
        z-index: 4;
        animation: flicker 1s infinite alternate;
    }
    @keyframes flicker {
        0% { opacity: 1; transform: translateX(-50%) scaleY(1);}
        100% { opacity: 0.7; transform: translateX(-50%) scaleY(1.1);}
    }
    @keyframes bounce {
        0% { transform: translateY(0);}
        100% { transform: translateY(-10px);}
    }
</style>
<div id="cakes">
    <div class="cake">
        <div class="cake-base"></div>
        <div class="cake-icing"></div>
        <div class="candle"></div>
        <div class="flame"></div>
    </div>
    <div class="cake">
        <div class="cake-base" style="background:linear-gradient(#fffbe7 60%, #6a89cc 100%);"></div>
        <div class="cake-icing" style="background:linear-gradient(90deg, #6a89cc 60%, #38ada9 100%);"></div>
        <div class="candle" style="background:#b33771;"></div>
        <div class="flame"></div>
    </div>
    <div class="cake">
        <div class="cake-base" style="background:linear-gradient(#fffbe7 60%, #38ada9 100%);"></div>
        <div class="cake-icing" style="background:linear-gradient(90deg, #b33771 60%, #ff6f91 100%);"></div>
        <div class="candle" style="background:#f9d423;"></div>
        <div class="flame"></div>
    </div>
</div>
<style>
    /* Extra cake details for realism */
    .cake-base {
        box-shadow: 0 8px 20px rgba(0,0,0,0.18), inset 0 2px 8px #fffbe7;
        border: 2px solid #fff8dc;
        position: absolute;
        bottom: 0;
        left: 50%;
        transform: translateX(-50%);
    }
    .cake-icing {
        box-shadow: 0 2px 8px #fffbe7, 0 0 0 2px #fff8dc;
        position: absolute;
        left: 50%;
        transform: translateX(-50%);
    }
    .cake-drip {
        width: 12px;
        height: 18px;
        background: linear-gradient(180deg, #fff 60%, #ffb347 100%);
        border-radius: 0 0 8px 8px;
        position: absolute;
        top: 6px;
        z-index: 3;
        opacity: 0.8;
    }
    .cake-drip.drip1 { left: 10px; }
    .cake-drip.drip2 { left: 28px; width: 8px; height: 14px;}
    .cake-drip.drip3 { left: 44px; width: 10px; height: 16px;}
    .cake-sprinkle {
        width: 4px;
        height: 4px;
        border-radius: 50%;
        position: absolute;
        top: 2px;
        z-index: 4;
        opacity: 0.85;
    }
    .cake-sprinkle.s1 { left: 12px; background: #ff6f91;}
    .cake-sprinkle.s2 { left: 22px; background: #f9d423;}
    .cake-sprinkle.s3 { left: 36px; background: #6a89cc;}
    .cake-sprinkle.s4 { left: 48px; background: #38ada9;}
    .cake-shadow {
        width: 60px;
        height: 12px;
        background: radial-gradient(ellipse at center, rgba(0,0,0,0.18) 60%, transparent 100%);
        border-radius: 50%;
        position: absolute;
        bottom: -14px;
        left: 50%;
        transform: translateX(-50%);
        z-index: 0;
        opacity: 0.7;
        pointer-events: none;
    }
</style>
<script>
    // Add drips, sprinkles, and shadow to each cake for realism
    document.querySelectorAll('.cake').forEach((cake, i) => {
        // Drips
        ['drip1','drip2','drip3'].forEach(dripClass => {
            const drip = document.createElement('div');
            drip.className = 'cake-drip ' + dripClass;
            // Match icing color
            const icing = cake.querySelector('.cake-icing');
            drip.style.background = icing ? icing.style.background || window.getComputedStyle(icing).background : '';
            cake.appendChild(drip);
        });
        // Sprinkles
        ['s1','s2','s3','s4'].forEach(sprinkleClass => {
            const sprinkle = document.createElement('div');
            sprinkle.className = 'cake-sprinkle ' + sprinkleClass;
            cake.appendChild(sprinkle);
        });
        // Shadow
        const shadow = document.createElement('div');
        shadow.className = 'cake-shadow';
        cake.appendChild(shadow);
    });
</script>
<script>
    // Show a message when a cake is clicked
    document.querySelectorAll('.cake').forEach((cake, idx) => {
        cake.addEventListener('click', () => {
            // Remove any existing cake message
            let oldMsg = document.getElementById('cakeMsg');
            if (oldMsg) oldMsg.remove();

            // Create and show the message
            const msg = document.createElement('div');
            msg.id = 'cakeMsg';
            msg.textContent = [
                "this was created 10 days before your birthday",
                "Iloveyouuusoomuchh darling enjoy your day",
                "Darling is you are seeing this,that means i didn't forget your birthday this timed video coded by me"
            ][idx % 3];
            msg.style.position = 'fixed';
            msg.style.left = '50%';
            msg.style.top = '80%';
            msg.style.transform = 'translate(-50%, 0)';
            msg.style.background = 'rgba(255,255,255,0.95)';
            msg.style.color = '#ff4e50';
            msg.style.padding = '18px 36px';
            msg.style.borderRadius = '18px';
            msg.style.fontSize = '1.3em';
            msg.style.boxShadow = '0 4px 24px rgba(0,0,0,0.12)';
            msg.style.zIndex = 1000;
            msg.style.transition = 'opacity 0.5s';
            document.body.appendChild(msg);

            setTimeout(() => {
                msg.style.opacity = 0;
                setTimeout(() => msg.remove(), 600);
            }, 2200);
        });
    });
</script>
<!-- Add cute floating hearts animation -->
<style>
.heart {
    position: fixed;
    width: 28px;
    height: 28px;
    background: pink;
    left: 50%;
    top: 100vh;
    opacity: 0.85;
    pointer-events: none;
    z-index: 999;
    transform: translateX(-50%) scale(1) rotate(-10deg);
    animation: floatHeart 5s linear forwards;
}
.heart::before,
.heart::after {
    content: '';
    position: absolute;
    width: 28px;
    height: 28px;
    background: pink;
    border-radius: 50%;
}
.heart::before {
    left: -14px;
    top: 0;
}
.heart::after {
    left: 0;
    top: -14px;
}
@keyframes floatHeart {
    0% {
        opacity: 0.9;
        transform: translateX(-50%) scale(1) rotate(-10deg);
    }
    80% {
        opacity: 0.8;
    }
    100% {
        top: -40px;
        opacity: 0;
        transform: translateX(-50%) scale(1.2) rotate(10deg);
    }
}
</style>
<script>
function randomBetween(a, b) {
    return Math.random() * (b - a) + a;
}
setInterval(() => {
    const heart = document.createElement('div');
    heart.className = 'heart';
    const colors = ['#ffb6c1', '#ff6f91', '#f9d423', '#b33771', '#6a89cc', '#38ada9'];
    heart.style.background = colors[Math.floor(Math.random() * colors.length)];
    heart.style.left = randomBetween(10, 90) + 'vw';
    heart.style.animationDuration = randomBetween(3.5, 6) + 's';
    heart.style.transform = `translateX(-50%) scale(${randomBetween(0.7,1.2)}) rotate(${randomBetween(-20,20)}deg)`;
    document.body.appendChild(heart);
    setTimeout(() => heart.remove(), 6000);
}, 700);
</script>
<!-- Add a cute footer message -->
<div style="margin-top:30px; text-align:center; font-size:1.1em; color:#fffbe7; text-shadow:0 2px 8px #ff6f91;">
    <span style="font-size:1.5em;">&#128151;</span>
    Made by Sky MWEHEHEEHEHEH :P 
    <span style="font-size:1.5em;">&#128149;</span>
</div>
