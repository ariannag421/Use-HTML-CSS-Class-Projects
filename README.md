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
