# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tonny Onwonga Responsive Webpage</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
        }

        /* Navigation Bar */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: left;
            background-color: blue;
            padding: 18px;
        }
        nav ul {
            list-style: none;
            display: flex;
            gap: 23px;
            margin: 0;
            padding: 0;
        }
        nav ul li {
            display: inline;
        }
        nav ul li a {
            color: green;
            text-decoration: none;
        }

        /* Layout using Grid */
        .container {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 23px;
            padding: 20px;
        }
        .box {
            background-color: gray;
            padding: 19px;
            text-align: center;
        }

        /* Responsive Design */
        @media (max-width: 600px) {
            .container {
                grid-template-columns: 1fr;
            }
            nav {
                flex-direction: column;
                text-align: right;
            }
        }
    </style>
</head>
<body>
    <nav>
        <h1 style="color: white;">My Website</h1>
        <ul>
            <li><a href="#">Tonny Onwonga</a></li>
            <li><a href="#">PLP Academy</a></li>
            <li><a href="#">Assignment</a></li>
        </ul>
    </nav>

    <div class="container">
        <div class="box">Box A</div>
        <div class="box">Box B</div>
        <div class="box">Box C</div>
    </div>
</body>
</html>


