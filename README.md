<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>To The Person I Loved</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <audio id="bg-music" loop>
    <source src="your-song.mp3" type="audio/mp3" />
    Your browser does not support the audio element.
  </audio>

  <header class="landing">
    <h1>To the person I loved deeply and kept admiring from afar.</h1>
    <button id="play-btn">Play Music</button>
    <a href="#main" class="enter-btn">Enter</a>
  </header>

  <main id="main">
    <!-- Unsent Letters -->
    <section id="letters">
      <h2>Unsent But Felt</h2>
      <div class="heart-grid">
        <div class="heart" onclick="openLetter(0)">❤️</div>
        <div class="heart" onclick="openLetter(1)">❤️</div>
        <div class="heart" onclick="openLetter(2)">❤️</div>
      </div>
    </section>

    <!-- Spotify Playlist -->
    <section id="playlist">
      <h2>The Songs That Still Taste Like You</h2>
      <iframe
        src="https://open.spotify.com/embed/playlist/YOUR_PLAYLIST_ID"
        width="100%" height="152" frameborder="0"
        allow="autoplay; clipboard-write; encrypted-media; picture-in-picture"
      ></iframe>
    </section>

    <!-- Moodboard -->
    <section id="moodboard">
      <h2>The Aesthetic of You</h2>
      <div class="board-images">
        <img src="img1.jpg" />
        <img src="img2.jpg" />
        <img src="img3.jpg" />
      </div>
    </section>

    <!-- Things I Loved -->
    <section id="loved">
      <h2>Things I Loved About You</h2>
      <div class="loved-grid">
        <div class="card">Your sleepy voice</div>
        <div class="card">The way you laughed</div>
        <div class="card">How you cared in silence</div>
      </div>
    </section>

    <!-- Book Club -->
    <section id="books">
      <h2>The Pages I Wished You Read With Me</h2>
      <ul>
        <li>Book Title 1 — “This book felt like you...”</li>
        <li>Book Title 2 — “I thought about you every chapter.”</li>
      </ul>
      <input type="password" id="codeInput" placeholder="Enter code to comment" />
      <button onclick="checkCode()">Submit</button>
      <textarea id="commentBox" style="display:none;" placeholder="Leave your comment here"></textarea>
    </section>

    <!-- Future Wishlist -->
    <section id="wishlist">
      <h2>Things I Wish We Did Together</h2>
      <div class="wish-gallery">
        <div class="wish">
          <img src="wish1.jpg" />
          <p>I wish I got to hold your hand here.</p>
        </div>
      </div>
    </section>
  </main>

  <div id="letterModal" class="modal">
    <div class="modal-content" id="letterText"></div>
    <button onclick="closeLetter()">Close</button>
  </div>

  <script src="script.js"></script>
</body>
</html>
