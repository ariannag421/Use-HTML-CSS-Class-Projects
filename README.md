# Use-HTML-CSS-Class-Projects
HTML labs for IT-2310 Web Programming.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="author" content="Arianna Garrett">
    <meta name="description" content="This is a sample page created for Lab 1.">
    <title>Lab 1 – My First Web Page</title>
</head>
<body>
    <h1>Arianna Garrett</h1>

    <p>Hello! My name is Arianna, and this is my first web page I have ever attempted. I am excited and intimidated, but I am determined to learn it.</p>
    
    <p>I love music and my taste varies so I never get bored. I could go to a baseball game everyday but I prefer going to local games. The summer time is my favorite season.</p>

    <ul>
        <li>Old school R&B</li>
        <li>Guardians games</li>
        <li>Swimming and tanning poolside</li>
        <li>Time with family and friends</li>
        <li>Making s'mores with my children</li>
    </ul>

    <p>One of the websites I use frequently to learn and reference web technologies is 
        <a href="https://developer.mozilla.org/" target="_blank">MDN Web Docs</a>.
    </p>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Lab 2 – Home</title>
</head>
<body>
    <h1>Welcome to Lab 2</h1>

    <p>This lab focuses on building structured navigation using HTML tables and hyperlinks, and practicing both relative and absolute linking.</p>

    <table border="1">
        <thead>
            <tr>
                <th>Link Name</th>
                <th>Destination</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>About Lab 2</td>
                <td><a href="lab2-about.html">Go to About Page</a></td>
            </tr>
            <tr>
                <td>Mozilla Homepage</td>
                <td><a href="https://www.mozilla.org" target="_blank">Visit Mozilla</a></td>
            </tr>
            <tr>
                <td>Tri-C Homepage</td>
                <td><a href="https://www.tri-c.edu" target="_blank">Visit Tri-C</a></td>
            </tr>
            <tr>
                <td>Tri-C IT Page</td>
                <td><a href="https://www.tri-c.edu/IT" target="_blank">Visit Tri-C IT</a></td>
            </tr>
        </tbody>
    </table>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Lab 2 – About</title>
</head>
<body>
    <h1>About Lab 2</h1>

    <p>In Lab 2, we are learning how to build HTML pages using structured elements like headings, paragraphs, tables, and links. We're also practicing how to use both relative and absolute URLs, and how to collect user input through web forms.</p>

    <table border="1">
        <thead>
            <tr>
                <th>Link Description</th>
                <th>Link</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Home Page</td>
                <td><a href="lab2-home.html">Go to Home</a></td>
            </tr>
            <tr>
                <td>Contact Me</td>
                <td><a href="mailto:your-email@example.com">Send Email</a></td>
            </tr>
        </tbody>
    </table>
</body>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Lab 2 – Coffee Order Form</title>
</head>
<body>
    <h1>Coffee Order Form</h1>
    <p>Please fill out the form below to place your coffee order. We’ll prepare it just the way you like it!</p>

    <form action="https://www.w3schools.com/action_page.php" method="get">
        <!-- Customer Name -->
        <label for="name">Customer Name:</label><br>
        <input type="text" id="name" name="customer_name" value="Alex" required><br><br>

        <!-- Email Address -->
        <label for="email">Email Address:</label><br>
        <input type="email" id="email" name="email" value="a123@yahoo.com" required><br><br>

        <!-- Coffee Type -->
        <label for="coffee">Coffee Type:</label><br>
        <select id="coffee" name="coffee_type" required>
            <option value="latte">Latte</option>
            <option value="cappuccino">Cappuccino</option>
            <option value="espresso">Espresso</option>
            <option value="americano">Americano</option>
            <option value="mocha">Mocha</option>
        </select><br><br>

        <!-- Size -->
        <label>Size:</label><br>
        <input type="radio" id="small" name="size" value="small" required>
        <label for="small">Small</label><br>
        <input type="radio" id="medium" name="size" value="medium">
        <label for="medium">Medium</label><br>
        <input type="radio" id="large" name="size" value="large">
        <label for="large">Large</label><br><br>

        <!-- Extras -->
        <label>Extras:</label><br>
        <input type="checkbox" id="whipped" name="extras" value="whipped_cream">
        <label for="whipped">Whipped Cream</label><br>
        <input type="checkbox" id="shot" name="extras" value="extra_shot">
        <label for="shot">Extra Shot</label><br>
        <input type="checkbox" id="almond" name="extras" value="almond_milk">
        <label for="almond">Almond Milk</label><br><br>

        <!-- Special Instructions -->
        <label for="instructions">Special Instructions:</label><br>
        <textarea id="instructions" name="instructions" rows="4" cols="40" placeholder="Any special requests?"></textarea><br><br>

        <!-- Submit -->
        <input type="submit" value="Place Order">
    </form>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Lab 3 - CSS Formatting Basics</title>

  <style>
    /* Apply a light background and Arial font to the whole page */
    body {
      background-color: #FFFACD; /* LemonChiffon */
      font-family: Arial, sans-serif;
    }

    /* Style the <h1>: custom color, center, and padding */
    h1 {
      color: #8B4513;      /* Custom brown */
      text-align: center;
      padding: 10px;
    }

    /* Style unordered list and bullets */
    ul {
      list-style: none;
      padding-left: 20px;
    }

    ul li {
      position: relative;
      padding-left: 20px;
      color: #800080; /* Purple text color for list items */
    }

    ul li::before {
      content: "•";
      color: #FF4500; /* OrangeRed custom bullet color */
      position: absolute;
      left: 0;
    }

    /* Link styling */
    a {
      color: blue;
      text-decoration: none;
    }

    a:hover {
      text-decoration: none;
    }

    /* Styled box */
    .styled-box {
      border: 2px solid #333;
      background-color: #d3d3d3;
      padding: 15px;
      text-align: center;
      margin-top: 20px;
      border-radius: 5px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to Lab 3</h1>
  </header>
  <main>
    <p>This is the first paragraph. It contains some placeholder text for styling practice.</p>
    <p>This is the second paragraph. Feel free to add more content if you'd like.</p>
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
    </ul>
    <a href="https://www.tri-c.edu">Visit Cuyahoga Community College</a>
    <div class="styled-box">
      <p>This is a styled box. Add your CSS rules to make it look great!</p>
    </div>
  </main>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Styling Text and Fonts</title>
  <style>
    /* Apply a sans-serif font to the entire document */
    body {
      font-family: sans-serif;
      margin: 0;
      padding: 20px;
    }

    /* Style <h1>: font-size 3rem, bold, center-aligned, with red shadow */
    h1 {
      font-size: 3rem;
      font-weight: bold;
      text-align: center;
      text-shadow: 2px 2px 4px red;
    }

    /* Style <h2>: font-size 2rem, light font weight, and uppercase */
    h2 {
      font-size: 2rem;
      font-weight: 300;
      text-transform: uppercase;
    }

    /* Justify all paragraph text and set line height */
    p {
      text-align: justify;
      line-height: 1.6;
    }

    /* Capitalize first letter of each word in Transforming Text section */
    section:nth-of-type(3) p {
      text-transform: capitalize;
    }

    /* Add subtle gray shadow to "Text Shadow" paragraph */
    section:nth-of-type(4) p {
      text-shadow: 1px 1px 2px #888888;
    }

    /* Center-align the footer */
    footer {
      text-align: center;
      margin-top: 40px;
      font-size: 0.9em;
      color: #666;
    }

    /* Square bullets for unordered list */
    ul {
      list-style-type: square;
      padding-left: 20px;
    }

    /* Uppercase Roman numerals for ordered list */
    ol {
      list-style-type: upper-roman;
      padding-left: 20px;
    }

    /* Add margin between list items */
    li {
      margin: 1rem 0;
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to Text Styling Lab</h1>
  </header>
  <main>
    <section>
      <h2>Font Properties</h2>
      <p>This paragraph demonstrates the use of font-family, font-size, and font-weight properties.</p>
    </section>
    <section>
      <h2>Text Alignment</h2>
      <p>This paragraph demonstrates how to align text using the text-align property.</p>
    </section>
    <section>
      <h2>Transforming Text</h2>
      <p>This paragraph demonstrates text transformation with uppercase, lowercase, and capitalization.</p>
    </section>
    <section>
      <h2>Text Shadow</h2>
      <p>This paragraph demonstrates how to add shadow effects to text.</p>
    </section>
    <section>
      <h2>Lists</h2>
      <ul>
        <li>Item One</li>
        <li>Item Two</li>
        <li>Item Three</li>
      </ul>
      <ol>
        <li>First Step</li>
        <li>Second Step</li>
        <li>Third Step</li>
      </ol>
    </section>
  </main>
  <footer>
    <p>Styling Text and Fonts Lab © 2025</p>
  </footer>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Java Haven</title>
  <style>
    /* Import a cozy serif font for warm feel */
    @import url('https://fonts.googleapis.com/css2?family=Playfair+Display&family=Roboto&display=swap');

    /* Reset default margin/padding */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      display: grid;
      grid-template-areas:
        "header"
        "nav"
        "main"
        "footer";
      grid-template-rows: auto 50px 1fr auto;
      grid-template-columns: 1fr;
      min-height: 100vh;
      font-family: 'Roboto', sans-serif;
      background-color: #f5f1ea; /* Creamy warm background */
      color: #4b3621; /* Dark coffee brown text */
    }

    .header {
      grid-area: header;
      background-color: #6f4e37; /* Rich coffee brown */
      color: #f5f1ea; /* Cream text */
      padding: 30px 20px;
      text-align: center;
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: 2.8rem;
      letter-spacing: 2px;
      text-shadow: 1px 1px 3px rgba(0,0,0,0.3);
    }

    .header p {
      font-family: 'Roboto', sans-serif;
      font-weight: 400;
      font-size: 1.2rem;
      margin-top: 8px;
      font-style: italic;
      color: #e6d8c3;
      text-shadow: 1px 1px 2px rgba(0,0,0,0.2);
    }

    .nav {
      grid-area: nav;
      background-color: #a67b5b; /* Medium warm brown */
      padding: 12px 0;
      box-shadow: inset 0 -2px 4px rgba(0,0,0,0.15);
    }

    .nav ul {
      display: flex;
      justify-content: center;
      list-style: none;
      gap: 35px;
      font-family: 'Roboto', sans-serif;
      font-weight: 600;
      letter-spacing: 1px;
    }

    .nav a {
      text-decoration: none;
      color: #f5f1ea;
      font-size: 1.1rem;
      transition: color 0.3s ease;
      padding: 4px 8px;
      border-radius: 4px;
    }

    .nav a:hover,
    .nav a:focus {
      background-color: #f5f1ea;
      color: #6f4e37;
      box-shadow: 0 0 6px #6f4e37aa;
    }

    .main-content {
      grid-area: main;
      padding: 25px 30px;
      background-color: #fdf8f1; /* Soft cream */
      font-family: 'Playfair Display', serif;
    }

    .main-content h2 {
      font-size: 2.2rem;
      margin-bottom: 20px;
      color: #6f4e37;
      text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
    }

    .flex-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      margin-top: 15px;
      gap: 20px;
    }

    .flex-item {
      background-color: #a67b5b; /* warm brown */
      color: #f5f1ea; /* cream text */
      padding: 20px 25px;
      border-radius: 8px;
      flex: 1 1 150px;
      max-width: 200px;
      text-align: center;
      font-weight: 700;
      font-family: 'Roboto', sans-serif;
      font-size: 1.1rem;
      box-shadow: 2px 3px 6px rgba(101, 67, 33, 0.4);
      transition: background-color 0.3s ease;
      cursor: default;
      user-select: none;
    }

    .flex-item:hover {
      background-color: #855e42;
      box-shadow: 3px 5px 10px rgba(101, 67, 33, 0.6);
    }

    .footer {
      grid-area: footer;
      background-color: #6f4e37;
      color: #f5f1ea;
      text-align: center;
      padding: 18px 0;
      font-size: 0.9rem;
      font-family: 'Roboto', sans-serif;
      box-shadow: inset 0 2px 5px rgba(0,0,0,0.3);
    }
  </style>
</head>
<body>
  <header class="header">
    <h1>Java Haven</h1>
    <p>Your daily dose of caffeine and comfort.</p>
  </header>
  
  <nav class="nav">
    <ul>
      <li><a href="#menu">Menu</a></li>
      <li><a href="#about">About Us</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
  
  <main class="main-content">
    <h2>Featured Coffees</h2>
    <div class="flex-container">
      <div class="flex-item">Espresso</div>
      <div class="flex-item">Cappuccino</div>
      <div class="flex-item">Latte</div>
      <div class="flex-item">Mocha</div>
    </div>
  </main>
  
  <footer class="footer">
    <p>&copy; 2025 Java Haven. All Rights Reserved.</p>
  </footer>
</body>
</html>
