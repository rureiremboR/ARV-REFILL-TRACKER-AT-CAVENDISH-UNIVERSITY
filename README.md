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
css.styles

/* Order Form Container */
#order {
  padding: 40px 20px;
}

/* Form Card - matches your existing dashboard-card */
#orderForm.dashboard-card {
  background: #13313d;
  border: 2px solid #37d422;
  border-radius: 16px;
  padding: 30px;
  width: 100%;
  max-width: 600px;
  margin: 20px auto;
  text-align: left;
  box-shadow: 0 8px 20px rgba(55, 212, 34, 0.2);
}

/* Form Labels */
#orderForm label {
  display: block;
  margin: 12px 0 5px;
  color: #ffeb3b;
  font-weight: bold;
  font-size: 0.95em;
}

/* Input, Select, Textarea Fields */
#orderForm input,
#orderForm select,
#orderForm textarea {
  width: 100%;
  padding: 10px 12px;
  border-radius: 6px;
  border: 1px solid #009688;
  background: #0e252e;
  color: white;
  font-size: 1em;
  box-sizing: border-box;
  transition: border-color 0.2s ease;
}

/* Placeholder Text */
#orderForm input::placeholder,
#orderForm textarea::placeholder {
  color: #aaa;
}

/* Focus State */
#orderForm input:focus,
#orderForm select:focus,
#orderForm textarea:focus {
  outline: none;
  border-color: #37d422;
  box-shadow: 0 0 0 2px rgba(55, 212, 34, 0.2);
}

/* Readonly Fields */
#orderForm input[readonly] {
  background: #1a3a46;
  color: #ccc;
  cursor: not-allowed;
}

/* Submit Button - reuses your filter-btn style */
#orderForm.filter-btn {
  background: #004080;
  color: white;
  border: 1px solid #009688;
  padding: 10px 18px;
  margin-top: 15px;
  border-radius: 6px;
  cursor: pointer;
  font-size: 1em;
  transition: background 0.2s ease;
}

#orderForm.filter-btn:hover {
  background: #009688;
}

/* Success/Error Message */
#formMsg {
  text-align: center;
  color: #37d422;
  margin-top: 10px;
  font-weight: 500;
}

/* Responsive */
@media (max-width: 600px) {
  #orderForm.dashboard-card {
    padding: 20px;
    margin: 15px;
  }

  #order h2 {
    font-size: 1.5em;
  }
  The form looks consistent with your dashboard cards, has clear focus states for accessibility, and works well on mobile
}
