<!DOCTYPE html>
<html lang="ro">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MIRELLE – Beauty Studio</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display&family=Montserrat&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Montserrat', sans-serif;
      background-color: #fffafc;
      color: #333;
      scroll-behavior: smooth;
    }

    header {
      background-image: url('https://source.unsplash.com/1600x900/?beauty,salon');
      background-size: cover;
      background-position: center;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      color: white;
      text-align: center;
      position: relative;
    }

    header::after {
      content: "";
      position: absolute;
      top: 0; left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.5);
      z-index: 1;
    }

    header h1, header p, .cta-button {
      z-index: 2;
      position: relative;
    }

    header h1 {
      font-family: 'Playfair Display', serif;
      font-size: 4rem;
      margin: 0;
    }

    header p {
      font-size: 1.5rem;
    }

    .cta-button {
      background-color: #d4a5a5;
      color: white;
      padding: 12px 30px;
      border: none;
      border-radius: 5px;
      margin-top: 20px;
      font-size: 1rem;
      cursor: pointer;
      text-decoration: none;
    }

    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }

    section h2 {
      text-align: center;
      font-family: 'Playfair Display', serif;
      margin-bottom: 20px;
    }

    .services, .gallery, .reviews {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
      text-align: center;
    }

    .services div, .reviews div {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }

    .gallery img {
      width: 100%;
      border-radius: 10px;
      box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
      max-width: 500px;
      margin: 0 auto;
    }

    form input, form textarea, form select {
      padding: 10px;
      font-size: 1rem;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    form button {
      background-color: #d4a5a5;
      color: white;
      border: none;
      padding: 12px;
      border-radius: 5px;
      font-size: 1rem;
      cursor: pointer;
    }

    footer {
      background-color: #f8eaea;
      text-align: center;
      padding: 20px;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>

  <!-- HERO -->
  <header>
    <h1>MIRELLE</h1>
    <p>Frumusețea începe cu tine</p>
    <a href="#programare" class="cta-button">Programează-te acum</a>
  </header>

  <!-- DESPRE -->
  <section id="despre">
    <h2>Despre Mirelle</h2>
    <p>La Mirelle, fiecare detaliu contează. Salonul nostru este locul unde frumusețea se întâlnește cu profesionalismul. Cu o echipă dedicată și servicii de top, transformăm rutina de înfrumusețare într-o experiență de răsfăț.</p>
  </section>

  <!-- SERVICII -->
  <section id="servicii">
    <h2>Serviciile Noastre</h2>
    <div class="services">
      <div><strong>Coafură & Styling</strong><br>Transformări moderne sau clasice</div>
      <div><strong>Make-up Profesional</strong><br>Machiaj pentru evenimente speciale</div>
      <div><strong>Manichiură & Pedichiură</strong><br>Cu produse de calitate premium</div>
      <div><strong>Tratamente Faciale</strong><br>Reîntinerire și hidratare</div>
    </div>
  </section>

  <!-- GALERIE -->
  <section id="galerie">
    <h2>Galerie</h2>
    <div class="gallery">
      <img src="https://source.unsplash.com/400x300/?hair,beauty" alt="coafură">
      <img src="https://source.unsplash.com/400x300/?makeup" alt="makeup">
      <img src="https://source.unsplash.com/400x300/?nails,salon" alt="manichiură">
    </div>
  </section>

  <!-- RECENZII -->
  <section id="recenzii">
    <h2>Ce spun clientele noastre</h2>
    <div class="reviews">
      <div>"O atmosferă de vis și servicii impecabile!"<br>– Andreea T.</div>
      <div>"Recomand cu încredere! Profesionalism și atenție la detalii."<br>– Elena M.</div>
      <div>"Cel mai frumos salon din oraș! Mereu revin cu drag."<br>– Roxana D.</div>
    </div>
  </section>

  <!-- PROGRAMARE -->
  <section id="programare">
    <h2>Fă o programare</h2>
    <form>
      <input type="text" name="nume" placeholder="Numele tău" required>
      <input type="tel" name="telefon" placeholder="Telefon" required>
      <select name="serviciu">
        <option value="">Alege serviciul</option>
        <option>Coafură</option>
        <option>Make-up</option>
        <option>Manichiură</option>
        <option>Tratamente faciale</option>
      </select>
      <input type="date" name="data" required>
      <textarea name="mesaj" placeholder="Mesaj opțional"></textarea>
      <button type="submit">Trimite cererea</button>
    </form>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <h2>Contact</h2>
    <p><strong>Adresă:</strong> Str. Eleganței Nr. 10, București</p>
    <p><strong>Telefon:</strong> 0755 123 456</p>
    <p><strong>Email:</strong> contact@mirelle.ro</p>
    <p><strong>Instagram:</strong> <a href="#">@mirelle.beauty</a></p>
  </section>

  <!-- FOOTER -->
  <footer>
    &copy; 2025 Mirelle – Toate drepturile rezervate.
  </footer>

</body>
</html>
