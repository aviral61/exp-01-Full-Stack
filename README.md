CSS Variables (:root)
css
Copy
Edit
:root {
  --primary-color: #2c3e50;
  --secondary-color: #3498db;
}
Defines custom color variables that can be reused in your CSS.

--primary-color: A dark navy/blue-gray color (#2c3e50)

--secondary-color: A bright blue (#3498db)

You can later use them like:

css
Copy
Edit
color: var(--primary-color);
background-color: var(--secondary-color);
✅ 2. .bank-interface Class
css
Copy
Edit
.bank-interface {
  display: grid;
  gap: 1rem;
  max-width: 500px;
  margin: 2rem auto;
  padding: 2rem;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
}
This class likely wraps your entire banking interface and:

Uses CSS Grid layout.

Adds spacing (gap: 1rem) between elements.

Restricts the width to 500px and centers it (margin: 2rem auto).

Adds padding inside and rounded corners.

Applies a subtle shadow for a card-like effect.

✅ 3. Responsive Design with Media Query
css
Copy
Edit
@media (max-width: 600px) {
  .bank-interface {
    padding: 1rem;
    margin: 1rem;
  }
}
If the screen width is 600px or less (e.g., on a mobile phone), this makes the interface more compact by reducing padding and margin.

Ensures the layout remains usable and nice on small screens (responsive design).

🧠 Summary:
This CSS file creates a clean, modern, responsive design for a banking interface. It uses:

CSS variables for theme colors,

Grid layout for structure,

Box shadows and spacing for visual appeal,

Media queries for mobile responsiveness.
