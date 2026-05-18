Read me
<!DOCTYPE html>
<html lang="en">
<head>... </head>
<body>... </body>
</html>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ARV Refill Tracker Cavendish University Uganda Health Center</title>
<link rel="stylesheet" href="css/style.css">
<style>... </style>


function filterRefills(category) {
  const cards = document.querySelectorAll('.refill-card');
  cards.forEach(card => {
    if (category === 'all' || card.dataset.category === category) {
      card.style.display = 'block';
    } else {
      card.style.display = 'none';
    }
  });

  document.querySelectorAll('.filter-btn').forEach(btn => {
    btn.classList.remove('active');
  });
  event.target.classList.add('active');
}
