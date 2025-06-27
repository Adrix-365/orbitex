<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-sc
  <title>Ma Bibliothèque Anime & Manga</title>
  
  <style>
    /* === VARIABLES & RESET === */
    :root {
      --color-bg-dark: #121212;
      --color-bg-medium: #1f1f1f;
      --color-bg-light: #2c2c2c;
      --color-text-primary: #e0e0e0;
      --color-text-secondary: #a0a0a0;
      --color-accent-primary: #e53935;
      --color-accent-secondary: #f44336;
      --border-radius: 8px;
      --transition-speed: 0.3s;
    }

    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    /* === STYLES GÉNÉRAUX === */
    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
      background-color: var(--color-bg-dark);
      color: var(--color-text-primary);
      line-height: 1.6;
    }

    img {
      max-width: 100%;
      display: block;
    }

    a {
      color: var(--color-accent-secondary);
      text-decoration: none;
    }

    /* === COMPOSANTS & LAYOUT === */
    .container {
      max-width: 1200px;
      padding: 2rem 1rem;
      margin: 0 auto;
    }

    .page-header {
      background-color: var(--color-bg-medium);
      padding: 1.5rem;
      text-align: center;
      border-bottom: 4px solid var(--color-accent-primary);
    }

    .page-header__title {
      margin: 0;
      color: var(--color-accent-primary);
      font-size: 2rem;
      font-weight: 700;
    }
    
    .main-nav {
      background: var(--color-bg-light);
      padding: 0.75rem;
      text-align: center;
      margin-bottom: 1rem;
    }

    .main-nav__link {
      color: var(--color-text-primary);
      margin: 0 1rem;
      font-weight: bold;
      transition: color var(--transition-speed);
    }

    .main-nav__link:hover, .main-nav__link:focus {
      color: var(--color-accent-secondary);
      outline: none;
    }

    .page-footer {
      text-align: center;
      padding: 2rem;
      background-color: var(--color-bg-medium);
      color: var(--color-text-secondary);
      margin-top: 2rem;
      font-size: 0.9rem;
    }

    .section-title {
      color: var(--color-accent-secondary);
      border-bottom: 2px solid var(--color-accent-secondary);
      padding-bottom: 0.5rem;
      margin-bottom: 2rem;
      font-size: 1.75rem;
    }

    .btn {
      display: inline-block;
      padding: 0.75rem 1.5rem;
      text-align: center;
      background-color: var(--color-accent-primary);
      color: var(--color-text-primary);
      text-decoration: none;
      font-weight: bold;
      border-radius: var(--border-radius);
      transition: background-color var(--transition-speed) ease, transform var(--transition-speed) ease;
      border: none;
      cursor: pointer;
    }

    .btn:hover, .btn:focus {
      background-color: var(--color-accent-secondary);
      transform: translateY(-2px);
      outline: none;
    }

    /* === GRILLE DE CARTES === */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
      gap: 1.5rem;
    }

    .card {
      background-color: var(--color-bg-medium);
      border-radius: var(--border-radius);
      overflow: hidden;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
      transition: transform var(--transition-speed) ease, box-shadow var(--transition-speed) ease;
      display: flex;
      flex-direction: column;
    }

    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.5);
    }

    .card__image {
      width: 100%;
      height: 320px;
      object-fit: cover;
    }

    .card__body {
      padding: 1rem;
      display: flex;
      flex-direction: column;
      flex-grow: 1;
    }

    .card__title {
      font-size: 1.1rem;
      margin-bottom: 1rem;
      flex-grow: 1; 
    }

    .card__link {
      width: 100%;
    }
  </style>
</head>
<body>

  <header class="page-header">
    <h1 class="page-header__title">Ma Bibliothèque Anime & Manga</h1>
  </header>

  <nav class="main-nav">
    <a href="#anime" class="main-nav__link">Animes</a>
    <a href="#manga" class="main-nav__link">Scans</a>
  </nav>

  <main class="container">
    <section id="anime" aria-labelledby="anime-title">
      <h2 id="anime-title" class="section-title">Animes</h2>
      <div class="card-grid">
        
        <article class="card">
          <img src="https://www.themoviedb.org/t/p/w600_and_h900_bestv2/bXkcWvttNvfYeKk2JKr7osvLS4N.jpg" alt="Affiche de Demon Slayer" class="card__image">
          <div class="card__body">
            <h3 class="card__title">Demon Slayer S1</h3>
            <a href="https://example.com/demonslayer-ep1" target="_blank" rel="noopener noreferrer" class="btn card__link">Regarder</a>
          </div>
        </article>

        <article class="card">
          <img src="https://www.themoviedb.org/t/p/w600_and_h900_bestv2/u6Wzxf2UoIE4Up4ecOHtL4Bqha5.jpg" alt="Affiche de Attack on Titan" class="card__image">
          <div class="card__body">
            <h3 class="card__title">Attack on Titan Final</h3>
            <a href="https://example.com/aot-final" target="_blank" rel="noopener noreferrer" class="btn card__link">Regarder</a>
          </div>
        </article>

        <article class="card">
          <img src="https://www.themoviedb.org/t/p/w600_and_h900_bestv2/5B1F21o1tuA7n5nK2w2nKsmr5a2.jpg" alt="Affiche de Détective Conan" class="card__image">
          <div class="card__body">
            <h3 class="card__title">Conan - Tous les épisodes</h3>
            <a href="conan-episode.html" class="btn card__link">Voir les épisodes</a>
          </div>
        </article>

        <article class="card">
          <img src="https://www.themoviedb.org/t/p/w600_and_h900_bestv2/fA5snUj07IyzZbUOFUJcZRExVnE.jpg" alt="Affiche des films Détective Conan" class="card__image">
          <div class="card__body">
            <h3 class="card__title">Conan - Tous les films</h3>
            <a href="https://example.com/conan-films" target="_blank" rel="noopener noreferrer" class="btn card__link">Voir</a>
          </div>
        </article>
      </div>
    </section>

    <section id="manga" aria-labelledby="manga-title">
      <h2 id="manga-title" class="section-title">Scans</h2>
      <div class="card-grid">

        <article class="card">
          <img src="https://www.nautiljon.com/images/manga/00/72/mini/one_piece_121127.jpg" alt="Couverture de One Piece" class="card__image">
          <div class="card__body">
            <h3 class="card__title">One Piece Chapitre 1100</h3>
            <a href="https://example.com/onepiece-1100" target="_blank" rel="noopener noreferrer" class="btn card__link">Lire</a>
          </div>
        </article>

        <article class="card">
          <img src="https://www.themoviedb.org/t/p/w600_and_h900_bestv2/u6Wzxf2UoIE4Up4ecOHtL4Bqha5.jpg" alt="Couverture de Jujutsu Kaisen" class="card__image">
          <div class="card__body">
            <h3 class="card__title">Jujutsu Kaisen 260</h3>
            <a href="https://example.com/jujutsu260" target="_blank" rel="noopener noreferrer" class="btn card__link">Lire</a>
          </div>
        </article>
      </div>
    </section>
  </main>

  <footer class="page-footer">
    <p>© 2025 - Ma collection personnelle • Pour usage privé uniquement.</p>
  </footer>

</body>
</html>
