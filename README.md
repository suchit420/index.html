# Let's create a simple HTML file based on the provided code and save it so the user can download or host it.

html_content = """
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>MovieBuzz Links</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #121212;
      color: #ffffff;
    }
    header {
      padding: 20px;
      text-align: center;
      background-color: #1f1f1f;
    }
    h1 {
      margin: 0;
      font-size: 2em;
    }
    .about {
      text-align: center;
      padding: 10px 20px;
      font-size: 1em;
      color: #cccccc;
    }
    .movie-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 20px;
    }
    .movie-card {
      background-color: #1f1f1f;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.5);
      overflow: hidden;
      transition: transform 0.2s;
    }
    .movie-card:hover {
      transform: scale(1.02);
    }
    .movie-card img {
      width: 100%;
      height: 350px;
      object-fit: cover;
    }
    .movie-card .content {
      padding: 15px;
    }
    .movie-card h3 {
      margin: 0 0 10px;
    }
    .movie-card p {
      font-size: 0.9em;
      color: #aaaaaa;
    }
    .telegram-btn {
      display: inline-block;
      margin-top: 10px;
      padding: 10px 15px;
      background-color: #0088cc;
      color: white;
      border: none;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
    }
    .telegram-btn:hover {
      background-color: #007ab8;
    }
  </style>
</head>
<body>
  <header>
    <h1>MovieBuzz Links</h1>
    <div class="about">
      Your quick gateway to fresh movie drops. Tap and watch!
    </div>
  </header>

  <main class="movie-grid">
    <!-- Movie 1 -->
    <div class="movie-card">
      <img src="https://via.placeholder.com/300x450.png?text=Movie+Poster" alt="Movie Title">
      <div class="content">
        <h3>Movie Title 1</h3>
        <p>This is a short description of the movie. Action, Drama, Thriller!</p>
        <a class="telegram-btn" href="https://t.me/YourMovieBotLink" target="_blank">Watch on Telegram</a>
      </div>
    </div>

    <!-- Movie 2 -->
    <div class="movie-card">
      <img src="https://via.placeholder.com/300x450.png?text=Movie+Poster" alt="Movie Title">
      <div class="content">
        <h3>Movie Title 2</h3>
        <p>A fantasy world of mystery and magic awaits you.</p>
        <a class="telegram-btn" href="https://t.me/YourMovieBotLink" target="_blank">Watch on Telegram</a>
      </div>
    </div>

    <!-- Add more movies below by copying this block -->
  </main>
</body>
</html>
"""

# Save to HTML file
file_path = "/mnt/data/MovieBuzz_Links.html"
with open(file_path, "w") as f:
    f.write(html_content)

file_path
