
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mouv+ — Votre solution de transport à Djibouti</title>
    <meta name="description" content="Réservez votre taxi, bus ou livraison cargo à Djibouti. Paiement D-Money et Wave. Rapide et fiable.">
    <link href="https://fonts.googleapis.com/css2?family=Syne:wght@700;800&family=DM+Sans:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #E8A020; --rust: #C84B2F; --deep: #0D1B2A;
            --light: #FAF6EF; --sand: #F5E6C8; --white: #FFFFFF;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        html { scroll-behavior: smooth; }
        body { font-family: 'DM Sans', sans-serif; background: var(--light); color: var(--deep); line-height: 1.6; }

        /* HEADER */
        nav {
            position: fixed; top: 0; width: 100%; z-index: 1000;
            background: rgba(13, 27, 42, 0.98); padding: 1rem 5%;
            display: flex; justify-content: space-between; align-items: center;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        .logo { font-family: 'Syne', sans-serif; font-weight: 800; font-size: 1.5rem; color: var(--sand); text-decoration: none; }
        .logo span { color: var(--gold); }
        .nav-links { display: none; } /* Hidden on mobile for simplicity */

        /* HERO SECTION */
        #hero {
            padding: 120px 5% 60px; background: var(--deep); color: var(--sand);
            text-align: center; position: relative; overflow: hidden;
        }
        .hero-badge {
            background: rgba(232,160,32,0.2); border: 1px solid var(--gold);
            color: var(--gold); padding: 5px 15px; border-radius: 20px;
            font-size: 0.8rem; font-weight: bold; display: inline-block; margin-bottom: 20px;
        }
        h1 { font-family: 'Syne', sans-serif; font-size: 2.5rem; line-height: 1.1; margin-bottom: 20px; }
        h1 span { color: var(--gold); }
        .hero-sub { color: rgba(245, 230, 200, 0.7); margin-bottom: 30px; font-size: 1.1rem; }
        
        .btn-main {
            background: var(--rust); color: white; padding: 15px 30px;
            border-radius: 10px; text-decoration: none; font-weight: bold;
            display: inline-block; transition: 0.3s; border: none; cursor: pointer;
        }
        .btn-main:hover { transform: scale(1.05); background: #b03a22; }

        /* SERVICES GRID */
        #services { padding: 60px 5%; }
        .section-title { text-align: center; margin-bottom: 40px; font-family: 'Syne', sans-serif; }
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; }
        .card { background: var(--white); padding: 25px; border-radius: 15px; box-shadow: 0 5px 15px rgba(0,0,0,0.05); }
        .card h3 { color: var(--rust); margin-bottom: 10px; }

        /* FORM */
        #booking { background: var(--sand); padding: 60px 5%; }
        .form-container { background: var(--white); padding: 30px; border-radius: 20px; max-width: 600px; margin: 0 auto; }
        .form-group { margin-bottom: 15px; }
        label { display: block; font-weight: bold; font-size: 0.9rem; margin-bottom: 5px; }
        input, select { width: 100%; padding: 12px; border: 1px solid #ddd; border-radius: 8px; font-size: 1rem; }

        /* FOOTER */
        footer { background: var(--deep); color: #888; padding: 40px 5%; text-align: center; }
        .footer-logo { color: var(--white); font-family: 'Syne', sans-serif; margin-bottom: 10px; display: block; }

        /* TOAST */
        #toast {
            position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%);
            background: #333; color: white; padding: 12px 25px; border-radius: 30px;
            display: none; z-index: 2000;
        }

        @media (min-width: 768px) {
            h1 { font-size: 4rem; }
            .nav-links { display: flex; gap: 20px; list-style: none; }
            .nav-links a { color: var(--sand); text-decoration: none; font-weight: 500; }
        }
    </style>
</head>
<body>

<nav>
    <a href="#" class="logo">Mouv<span>+</span></a>
    <ul class="nav-links">
        <li><a href="#services">Services</a></li>
        <li><a href="#booking">Réserver</a></li>
        <li><a href="tel:+25377000000">Contact</a></li>
    </ul>
    <a href="#booking" class="btn-main" style="padding: 8px 15px; font-size: 0.8rem;">Réserver</a>
</nav>

<section id="hero">
    <div class="hero-badge">L'EXCELLENCE À DJIBOUTI 🇩🇯</div>
    <h1>Bougez <span>librement</span><br>dans la ville.</h1>
    <p class="hero-sub">Taxi, Bus et Cargo. Simple, rapide et sécurisé.</p>
    <a href="#booking" class="btn-main">Réserver une course maintenant</a>
</section>

<section id="services">
    <div class="section-title">
        <h2>Nos Solutions</h2>
    </div>
    <div class="grid">
        <div class="card">
            <h3>🚕 Taxi Express</h3>
            <p>Un chauffeur chez vous en moins de 5 minutes. Idéal pour vos rendez-vous urgents.</p>
        </div>
        <div class="card">
            <h3>📦 Cargo & Logistique</h3>
            <p>Besoin de déplacer des marchandises ? Nos camions sont prêts pour le port et la ville.</p>
        </div>
        <div class="card">
            <h3>🚌 Navette Groupe</h3>
            <p>Transport collectif confortable pour les entreprises et les familles.</p>
        </div>
    </div>
</section>

<section id="booking">
    <div class="form-container">
        <h2 style="text-align: center; margin-bottom: 20px;">Faire une demande</h2>
        <div class="form-group">
            <label>Service souhaité</label>
            <select id="f-service">
                <option value="Taxi">Taxi Standard (1 500 FDJ)</option>
                <option value="Moto">Moto Express (500 FDJ)</option>
                <option value="Cargo">Livraison Cargo (3 000 FDJ)</option>
            </select>
        </div>
        <div class="form-group">
            <label>Point de départ</label>
            <input type="text" id="f-from" placeholder="Ex: Balbala, Avenue 26">
        </div>
        <div class="form-group">
            <label>Destination</label>
            <input type="text" id="f-to" placeholder="Ex: Heron, Rue de Venise">
        </div>
        <div class="form-group">
            <label>Votre Nom</label>
            <input type="text" id="f-name" placeholder="Votre nom">
        </div>
        <button class="btn-main" style="width: 100%;" onclick="sendWhatsApp()">Envoyer via WhatsApp</button>
    </div>
</section>

<footer>
    <span class="footer-logo">Mouv+ Djibouti</span>
    <p>Paiements acceptés : D-Money, Wave, Cash</p>
    <p style="margin-top: 20px; font-size: 0.7rem;">© 2026 Mouv+. Créé avec passion pour Djibouti.</p>
</footer>

<div id="toast">Demande envoyée !</div>

<script>
    function sendWhatsApp() {
        const service = document.getElementById('f-service').value;
        const from = document.getElementById('f-from').value;
        const to = document.getElementById('f-to').value;
        const name = document.getElementById('f-name').value;

        if(!from || !to || !name) {
            alert("Merci de remplir tous les champs.");
            return;
        }

        // REMPLACEZ PAR VOTRE NUMÉRO DJIBOUTIEN CI-DESSOUS
        const phone = "25377000000"; 
        
        const message = `Bonjour Mouv+ ! %0AJe souhaite réserver : *${service}*%0A• Départ : ${from}%0A• Destination : ${to}%0A• Nom : ${name}`;
        
        const url = `https://wa.me/${phone}?text=${message}`;
        
        window.open(url, '_blank').focus();
        
        const toast = document.getElementById('toast');
        toast.style.display = 'block';
        setTimeout(() => { toast.style.display = 'none'; }, 3000);
    }
</script>

</body>
</html>
