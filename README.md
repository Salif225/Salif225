- 👋 Hi, I’m @Salif225
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Salif225/Salif225 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SALIF Cissé - Freelance Créateur de Contenu et Développeur</title>
  <style>
    /* Couleurs Catalan et Ivoirien */
    :root {
      --green: #1D6F33; /* Vert Ivoirien */
      --orange: #FF6A13; /* Orange Ivoirien */
      --white: #FFFFFF;
      --dark-gray: #333333;
    }

    /* Styles généraux */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f4;
    }

    header {
      background-color: var(--dark-gray);
      color: var(--white);
      padding: 20px;
      text-align: center;
    }

    header nav ul {
      list-style-type: none;
      padding: 0;
    }

    header nav ul li {
      display: inline;
      margin-right: 15px;
    }

    header nav ul li a {
      color: var(--white);
      text-decoration: none;
      font-weight: bold;
    }

    header nav ul li a:hover {
      color: var(--orange);
    }

    section {
      padding: 20px;
      margin: 20px 0;
    }

    h2 {
      color: var(--dark-gray);
    }

    ul {
      list-style-type: none;
      padding: 0;
    }

    ul li {
      margin: 10px 0;
    }

    .testimonials {
      background-color: #e9e9e9;
      padding: 20px;
      margin-top: 20px;
      border-radius: 8px;
    }

    footer {
      text-align: center;
      background-color: var(--dark-gray);
      color: var(--white);
      padding: 10px;
      position: fixed;
      width: 100%;
      bottom: 0;
    }

    /* Formulaire de contact */
    form {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
    }

    label {
      margin: 5px 0;
    }

    input, textarea {
      padding: 8px;
      margin: 5px 0;
      width: 300px;
      max-width: 100%;
    }

    button {
      padding: 10px 20px;
      background-color: var(--green);
      color: var(--white);
      border: none;
      cursor: pointer;
      font-weight: bold;
    }

    button:hover {
      background-color: var(--orange);
    }

    /* Styles pour la validation de formulaire */
    .error {
      color: red;
      font-size: 0.9em;
    }
  </style>
</head>
<body>

  <header>
    <h1>Bienvenue sur le site de SALIF Cissé</h1>
    <p>Créateur de contenu | Développeur web | Rédacteur</p>
    <nav>
      <ul>
        <li><a href="#about">À propos</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#portfolio">Portfolio</a></li>
        <li><a href="#testimonials">Témoignages</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="about">
    <h2>À propos de moi</h2>
    <p>Bonjour, je suis SALIF Cissé, un créateur de contenu passionné et un développeur spécialisé dans la création de sites web, la rédaction de contenu, et la création d'applications. À 24 ans, j'aide les entreprises et les particuliers à réaliser leurs projets numériques avec des solutions créatives et fonctionnelles.</p>
  </section>

  <section id="services">
    <h2>Mes services</h2>
    <ul>
      <li><strong>Création de Sites Web</strong> : Je conçois des sites web modernes et responsives adaptés à vos besoins.</li>
      <li><strong>Rédaction de Contenu</strong> : Je rédige des articles de blog, des descriptions de produits et du contenu optimisé SEO.</li>
      <li><strong>Création d'Applications</strong> : Je développe des applications mobiles et web pour une expérience utilisateur fluide et innovante.</li>
    </ul>
  </section>

  <section id="portfolio">
    <h2>Mon portfolio</h2>
    <p>Voici quelques exemples de mes projets récents :</p>
    <ul>
      <li>Développement d'un site web pour un restaurant local.</li>
      <li>Création d'une application mobile pour une start-up.</li>
      <li>Rédaction de contenu pour un blog sur les technologies web.</li>
    </ul>
  </section>

  <section id="testimonials">
    <h2>Témoignages</h2>
    <div class="testimonials">
      <p><strong>Client 1:</strong> "Salif a créé un site web incroyable pour notre entreprise, avec une interface simple et intuitive."</p>
      <p><strong>Client 2:</strong> "Très satisfait de la rédaction des articles. Ils sont bien structurés et optimisés SEO!"</p>
      <p><strong>Client 3:</strong> "L'application mobile qu'il a développée pour nous fonctionne parfaitement. Très professionnel."</p>
    </div>
  </section>

  <section id="contact">
    <h2>Contactez-moi</h2>
    <form id="contactForm" onsubmit="return validateForm()">
      <label for="name">Nom :</label>
      <input type="text" id="name" name="name" required>

      <label for="email">Email :</label>
      <input type="email" id="email" name="email" required>

      <label for="message">Message :</label>
      <textarea id="message" name="message" rows="4" required></textarea>

      <button type="submit">Envoyer</button>
    </form>
    <p id="errorMessage" class="error"></p>
  </section>

  <footer>
    <p>&copy; 2024 SALIF Cissé. Tous droits réservés.</p>
  </footer>

  <script>
    function validateForm() {
      const name = document.getElementById('name').value;
      const email = document.getElementById('email').value;
      const message = document.getElementById('message').value;
      const errorMessage = document.getElementById('errorMessage');

      // Reset error message
      errorMessage.textContent = '';

      // Validation simple
      if (name === '' || email === '' || message === '') {
        errorMessage.textContent = 'Tous les champs sont obligatoires.';
        return false; // Prevent form submission
      }
      
      // Validate email format
      const emailRegex = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,6}$/;
      if (!emailRegex.test(email)) {
        errorMessage.textContent = 'Veuillez entrer un email valide.';
        return false;
      }

      // If validation passes, return true (form will be submitted)
      return true;
    }
  </script>

</body>
</html>
