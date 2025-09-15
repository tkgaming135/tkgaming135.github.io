<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <title>Anonymous School Feedback</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <style>
    body { font-family: system-ui, Arial, sans-serif; max-width: 720px; margin: 2rem auto; padding: 0 1rem; }
    h1 { margin-bottom: .5rem; }
    textarea, select, button { width: 100%; font-size: 1rem; }
    textarea { height: 160px; }
    label { display: block; margin: .75rem 0 .25rem; }
    .note { color: #555; font-size: .9rem; }
  </style>
</head>
<body>
  <h1>Anonymous Feedback</h1>
  <p class="note">No name or email is collected; only the message is sent to the school inbox.</p>

  <!-- Replace ACTION_URL with the Apps Script Web App URL from the deployment step -->
  <form action="https://script.google.com/macros/s/AKfycbwHan4dcviGZp_nhPiWZuHu94iMtfXA5x8-LzjdqPixmz4Adjz4xdMM9EXfNR6kT7EITA/exec" method="post">
    <label for="category">Category (optional)</label>
    <select id="category" name="category">
      <option>General</option>
      <option>Facilities</option>
      <option>Academics</option>
      <option>Safety</option>
      <option>Other</option>
    </select>

    <label for="message">Message</label>
    <textarea id="message" name="message" placeholder="Write feedback or a complaint..." required></textarea>

    <button type="submit">Send Anonymously</button>
  </form>
</body>
</html>
