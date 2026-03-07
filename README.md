<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Vibe Pro Auto Moto et Garage SARL</title>
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
<style>
* { margin:0; padding:0; box-sizing:border-box; font-family:'Roboto',sans-serif; }
body { line-height:1.6; color:#333; background:#fafafa; }
header { background:#1e1e2f; color:white; padding:20px; text-align:center; }
header h1 { font-size:2rem; margin-bottom:10px; }
nav a { color:white; margin:0 15px; text-decoration:none; font-weight:500; }
nav a:hover { text-decoration:underline; }
.hero { background:url('https://images.unsplash.com/photo-1552519507-da3b142c6e3d') center/cover no-repeat; color:white; height:450px; display:flex; align-items:center; justify-content:center; text-align:center; animation:fadeIn 2s; }
.hero h2 { font-size:2.4rem; background:rgba(0,0,0,0.5); padding:15px 25px; border-radius:10px; }
.services, .about, .gallery, .contact { padding:60px 20px; text-align:center; }
.services h2, .about h2, .gallery h2, .contact h2 { margin-bottom:40px; font-size:2rem; }
.service-cards { display:flex; flex-wrap:wrap; justify-content:center; gap:25px; }
.card { background:#fff; padding:20px; width:260px; border-radius:15px; box-shadow:0 4px 12px rgba(0,0,0,0.1); transition:transform 0.3s; }
.card:hover { transform:translateY(-7px); }
.card img { width:100%; height:160px; object-fit:cover; border-radius:10px; margin-bottom:12px; }
.about { background:#e8e8e8; border-radius:15px; margin:0 10px; padding:60px 20px; }
.gallery { position:relative; overflow:hidden; border-radius:15px; }
.slider { display:flex; transition:transform 0.5s ease-in-out; }
.slider img { width:100%; flex-shrink:0; border-radius:15px; }
.contact form { max-width:520px; margin:auto; display:flex; flex-direction:column; gap:15px; background:#fff; padding:25px; border-radius:15px; box-shadow:0 4px 12px rgba(0,0,0,0.1); }
.contact input, .contact textarea, .contact select { padding:12px; border-radius:8px; border:1px solid #ccc; }
.contact button { padding:12px; background:#1e1e2f; color:white; border:none; border-radius:8px; cursor:pointer; transition:background 0.3s; }
.contact button:hover { background:#333; }
footer { background:#1e1e2f; color:white; padding:25px; text-align:center; }
.whatsapp { position:fixed; bottom:20px; right:20px; background:#25D366; color:white; border-radius:50%; width:65px; height:65px; display:flex; align-items:center; justify-content:center; font-size:32px; text-decoration:none; box-shadow:2px 2px 8px rgba(0,0,0,0.3); }
@keyframes fadeIn { 0%{opacity:0} 100%{opacity:1} }
@media(max-width:768px){ .service-cards { flex-direction:column; align-items:center; } }
</style>
</head>
<body>

<header>
<h1>Vibe Pro Auto Moto et Garage SARL</h1>
<nav>
<a href="#services">Services</a>
<a href="#about">À propos</a>
<a href="#gallery">Galerie</a>
<a href="#contact">Contact</a>
</nav>
</header>

<section class="hero">
<h2>Votre garage de confiance à Ouagadougou</h2>
</section>

<section id="services" class="services">
<h2>Nos Services</h2>
<div class="service-cards">
<div class="card"><img src="https://images.unsplash.com/photo-1581091870625-19dc36a47ff7" alt="Réparation auto"><h3>Réparation automobile</h3><p>Entretien et réparation complète de tous types de véhicules.</p></div>
<div class="card"><img src="https://images.unsplash.com/photo-1606932399192-c84b42d6b51c" alt="Réparation moto"><h3>Réparation moto</h3><p>Diagnostic et réparation rapide de motos et scooters.</p></div>
<div class="card"><img src="https://images.unsplash.com/photo-1610381481006-3b0d2c68b179" alt="Diagnostic"><h3>Diagnostic électronique</h3><p>Analyse complète des problèmes électroniques de votre véhicule.</p></div>
<div class="card"><img src="https://images.unsplash.com/photo-1571607380475-6896ed3a89d3" alt="Lavage"><h3>Lavage et entretien</h3><p>Lavage complet, intérieur et extérieur, pour voitures et motos.</p></div>
</div>
</section>

<section id="about" class="about">
<h2>À propos de nous</h2>
<p>Vibe Pro Auto Moto et Garage SARL est un garage basé à Ouagadougou, spécialisé dans la réparation automobile et moto. Professionnalisme, rapidité et satisfaction client sont nos priorités.</p>
</section>

<section id="gallery" class="gallery">
<h2>Galerie</h2>
<div class="slider" id="slider">
<img src="https://images.unsplash.com/photo-1581093448793-5e7a2a142d8a" alt="Projet 1">
<img src="https://images.unsplash.com/photo-1598575934095-4f64f15a7c6a" alt="Projet 2">
<img src="https://images.unsplash.com/photo-1611095973510-d1e6f1caa2b3" alt="Projet 3">
</div>
</section>

<section id="contact" class="contact">
<h2>Prendre rendez-vous / Contact</h2>
<form id="appointmentForm">
<input type="text" placeholder="Nom complet" required>
<input type="email" placeholder="Email" required>
<input type="tel" placeholder="Téléphone" required>
<select required>
<option value="">Sélectionnez le service</option>
<option value="auto">Réparation automobile</option>
<option value="moto">Réparation moto</option>
<option value="diagnostic">Diagnostic électronique</option>
<option value="lavage">Lavage et entretien</option>
</select>
<input type="date" required>
<input type="time" required>
<textarea rows="3" placeholder="Message" required></textarea>
<button type="submit">Envoyer</button>
</form>
</section>

<a href="https://wa.me/226XXXXXXXX" class="whatsapp" target="_blank">📱</a>

<footer>
<p>&copy; 2026 Vibe Pro Auto Moto et Garage SARL | Ouagadougou, Burkina Faso</p>
</footer>

<script>
// Slider automatique
let slider = document.getElementById('slider');
let index = 0;
setInterval(() => {
index = (index + 1) % slider.children.length;
slider.style.transform = `translateX(-${index * 100}%)`;
}, 3000);

// Formulaire avec WhatsApp + email
document.getElementById('appointmentForm').addEventListener('submit', function(e){
e.preventDefault();
let nom = this[0].value;
let email = this[1].value;
let tel = this[2].value;
let service = this[3].value;
let date = this[4].value;
let time = this[5].value;
let message = this[6].value;

// Message WhatsApp
let waMessage = `Bonjour,%0ANom: ${nom}%0AEmail: ${email}%0ATéléphone: ${tel}%0AService: ${service}%0ADate: ${date}%0AHeure: ${time}%0AMessage: ${message}`;
window.open(`https://wa.me/226XXXXXXXX?text=${waMessage}`, '_blank');

// Confirmation alert
alert('Merci ! Votre rendez-vous a été soumis. Nous vous contacterons bientôt.');
this.reset();

// Ici, tu peux aussi ajouter un envoi email via un backend ou service tiers
});
</script>

</body>
</html>
