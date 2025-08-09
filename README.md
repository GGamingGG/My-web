# My-web [Upl<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gamer's Arena</title>
<style>
    body {
        margin: 0;
        font-family: Arial, sans-serif;
        color: white;
        background: linear-gradient(135deg, #1a1a2e, #16213e, #0f3460, #53354a, #e94560);
        background-size: 400% 400%;
        animation: bgShift 15s ease infinite;
        overflow-x: hidden;
    }

    @keyframes bgShift {
        0% { background-position: 0% 50%; }
        50% { background-position: 100% 50%; }
        100% { background-position: 0% 50%; }
    }

    header {
        text-align: center;
        padding: 50px 20px;
        font-size: 2.5rem;
        backdrop-filter: blur(5px);
    }

    .container {
        display: flex;
        justify-content: center;
        gap: 20px;
        flex-wrap: wrap;
        padding: 20px;
    }

    .card {
        width: 250px;
        background: rgba(255, 255, 255, 0.1);
        border-radius: 15px;
        cursor: pointer;
        transform: translateX(-100vw);
        transition: transform 0.5s ease, box-shadow 0.3s ease;
        overflow: hidden;
    }

    .card:hover {
        box-shadow: 0 0 20px #fff;
        transform: scale(1.05);
    }

    .card h2 {
        margin: 0;
        padding: 15px;
        text-align: center;
        background: rgba(0,0,0,0.3);
    }

    .content {
        display: none;
        padding: 15px;
        font-size: 1rem;
        background: rgba(0,0,0,0.2);
    }

    .from-left { animation: slideInLeft 1s forwards; }
    .from-right { animation: slideInRight 1s forwards; }

    @keyframes slideInLeft { to { transform: translateX(0); } }
    @keyframes slideInRight { to { transform: translateX(0); } }
</style>
</head>
<body>

<header>🔥 Gamer's Arena — WoT Blitz & Starblast 🔥</header>

<div class="container">
    <div class="card from-left">
        <h2>World of Tanks Blitz</h2>
        <div class="content">
            World of Tanks Blitz is a free-to-play tank shooter where you command legendary armored vehicles in fast-paced 7v7 battles. Here I share my tips, favorite tanks like the E 100 and Maus, and epic battle strategies.
        </div>
    </div>

    <div class="card from-right">
        <h2>Starblast.io</h2>
        <div class="content">
            Starblast.io is an action-packed space shooter where you mine asteroids, upgrade your ship, and battle other players in intense space dogfights. I cover ship builds, tactics, and pro moves to dominate.
        </div>
    </div>

    <div class="card from-left">
        <h2>Pro Tips</h2>
        <div class="content">
            - In WoT Blitz, always angle your armor to bounce shots.<br>
            - In Starblast, collect gems early to get an upgrade lead.<br>
            - Keep moving — being predictable is your enemy's best friend.<br>
            - Learn the maps, so you can control choke points.
        </div>
    </div>

    <div class="card from-right">
        <h2>Gameplay of WoT Blitz</h2>
        <div class="content">
            <iframe width="100%" height="200" src="https://www.youtube.com/embed/E51VPxJhKHw" frameborder="0" allowfullscreen></iframe>
        </div>
    </div>
</div>

<script>
    // Slide in effect
    document.querySelectorAll('.card').forEach((card, index) => {
        setTimeout(() => {
            if (index % 2 === 0) {
                card.classList.add('from-left');
            } else {
                card.classList.add('from-right');
            }
        }, index * 300);
    });

    // Toggle content when clicked
    document.querySelectorAll('.card').forEach(card => {
        card.addEventListener('click', () => {
            const content = card.querySelector('.content');
            content.style.display = content.style.display === 'block' ? 'none' : 'block';
        });
    });
</script>

</body>
</html>
oading my web.html…]()

js open it :)
