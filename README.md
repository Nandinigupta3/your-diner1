<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Diner</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-image: url(https://b.zmtcdn.com/web_assets/81f3ff974d82520780078ba1cfbd453a1583259680.png); /* Add the path to your background image */
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            background-attachment: fixed;
        }

        .body_container {
            /* Add styles for the body container if needed */
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.8); /* White container background color with opacity */
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Box shadow for container */
        }

        /* The rest of your existing styles... */

        /* Your existing styles */

        .menu_section {
            display: none;
            margin-top: 20px;
        }

        .menu_section h2 {
            margin-bottom: 10px;
        }

        .menu_section ul {
            list-style-type: none;
            padding: 0;
            margin: 0;
        }

        .menu_section li {
            margin-bottom: 10px; /* Increased margin for better spacing */
        }

        .menu_section li img {
            width: 50px; /* Adjust the width to your preference */
            height: 50px; /* Adjust the height to your preference */
            margin-right: 10px; /* Add margin for better spacing between image and text */
            border-radius: 5px; /* Add border-radius for rounded corners */
        }

        #showMenuBtn {
            margin-top: 10px;
            cursor: pointer;
            color: #333;
            background-color: #ffc107;
            border: none;
            padding: 10px;
            border-radius: 5px;
        }

        #dineOutBtn {
            margin-top: 10px;
            cursor: pointer;
            color: #fff; /* White text color */
            background-color: #333; /* Dark background color for the button */
            border: none;
            padding: 10px;
            border-radius: 5px;
        }

        .owner-section {
            margin-top: 20px;
        }

        .owner-form {
            max-width: 400px;
            margin: 0 auto;
            background-color: #f9f9f9; /* Light gray background color for the form */
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Box shadow for the form */
        }

        .owner-form h2 {
            text-align: center;
            color: #333; /* Dark text color */
        }

        .owner-form label {
            display: block;
            margin: 10px 0 5px;
            color: #555; /* Label text color */
        }

        .owner-form input {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            box-sizing: border-box;
            border: 1px solid #ccc; /* Input border color */
            border-radius: 3px;
        }

        .owner-form button {
            width: 100%;
            padding: 10px;
            background-color: #4caf50; /* Green button background color */
            color: #fff; /* White text color */
            border: none;
            border-radius: 3px;
            cursor: pointer;
        }

        .owner-form button:hover {
            background-color: #45a049; /* Darker green on hover */
        }
    </style>
</head>

<body class="body_container">

    <div class="container">

        <header class="header_container">
            <h1 class="header_title"> Your Diner</h1>
            <p class="header_desc"></p>
        </header>

        <!-- Login Form -->
        <div class="login-container">
            <div class="login-form">
                <h2>LOGIN</h2>
                <form>
                    <label for="username">Username</label>
                    <input type="text" id="username" name="username" required>

                    <label for="password">Password</label>
                    <input type="password" id="password" name="password" required>

                    <button type="submit">Login</button>
                </form>
            </div>
        </div>
        <!-- End of Login Form -->

        <button id="showMenuBtn" onclick="toggleMenu()">Show Menu</button>

        <!-- Menu Section -->
        <section class="menu_section" id="menuSection">
            <h2>Menu</h2>
            <ul>
                <!-- Appetizers -->
                <li>Appetizers:
                    <ul>
                        <li>
                            <img src="http://www.zedamagazine.com/wp-content/uploads/2018/06/Indian-Food-Samosa-Dish-HD-Wallpapers.jpg" alt="Samosas Image">
                            Samosas: Triangular pastry filled with spiced potatoes and peas.
                        </li>
                        <!-- Add similar <li> elements for other appetizers with their respective image URLs -->
                    </ul>
                </li>

                <!-- Main Courses - Vegetarian -->
                <li>Main Courses - Vegetarian:
                    <ul>
                        <!-- Add image URLs for vegetarian main courses -->
                        <li>
                            <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse3.mm.bing.net%2Fth%3Fid%3DOIP.seQ_Xm_1c2U2BfMuez4NdgHaLF%26pid%3DApi&f=1&ipt=71b2d194c5e26e74a30cb644a9409df165b7ffe76dd6fbb447782a9b63960742&ipo=images" alt="Palak Paneer Image">
                            Palak Paneer: Cottage cheese cubes in a spinach-based curry.
                        </li>
                        <li>
                            <img src="placeholder_url.jpg" alt="Chana Masala Image">
                            Chana Masala: Chickpeas in a spicy tomato-based sauce.
                        </li>
                        <!-- Add similar <li> elements for other vegetarian main courses -->
                    </ul>
                </li>

                <!-- Main Courses - Non-Vegetarian -->
                <li>Main Courses - Non-Vegetarian:
                    <ul>
                        <!-- Add image URLs for non-vegetarian main courses -->
                        <li>
                            <img src="placeholder_url.jpg" alt="Butter Chicken Image">
                            Butter Chicken (Chicken Makhani): Creamy and tomato-based curry with tender chicken pieces.
                        </li>
                        <li>
                            <img src="placeholder_url.jpg" alt="Rogan Josh Image">
                            Rogan Josh: Kashmiri lamb curry with aromatic spices.
                        </li>
                        <!-- Add similar <li> elements for other non-vegetarian main courses -->
                    </ul>
                </li>

                <!-- Breads -->
                <li>Breads:
                    <ul>
                        <!-- Add image URLs for breads -->
                        <li>
                            <img src="placeholder_url.jpg" alt="Naan Image">
                            Naan: Soft, leavened Indian bread.
                        </li>
                        <li>
                            <img src="placeholder_url.jpg" alt="Roti Image">
                            Roti: Whole wheat flatbread.
                        </li>
                        <!-- Add similar <li> elements for other breads -->
                    </ul>
                </li>

                <!-- Rice -->
                <li>Rice:
                    <ul>
                        <!-- Add image URLs for rice dishes -->
                        <li>
                            <img src="placeholder_url.jpg" alt="Vegetable Biryani Image">
                            Vegetable Biryani: Fragrant rice cooked with mixed vegetables and biryani spices.
                        </li>
                        <li>
                            <img src="placeholder_url.jpg" alt="Jeera Rice Image">
                            Jeera Rice: Basmati rice tempered with cumin seeds.
                        </li>
                        <!-- Add similar <li> elements for other rice dishes -->
                    </ul>
                </li>

                <!-- Desserts -->
                <li>Desserts:
                    <ul>
                        <!-- Add image URLs for desserts -->
                        <li>
                            <img src="placeholder_url.jpg" alt="Gulab Jamun Image">
                            Gulab Jamun: Deep-fried milk dumplings soaked in sugar syrup.
                        </li>
                        <li>
                            <img src="placeholder_url.jpg" alt="Rasgulla Image">
                            Rasgulla: Spongy cheese balls in sugar syrup.
                        </li>
                        <!-- Add similar <li> elements for other desserts -->
                    </ul>
                </li>
            </ul>
        </section>
        <!-- End Menu Section -->

        <!-- Dine Out Button -->
        <button id="dineOutBtn" onclick="showDineOutDetails()">Dine Out</button>

        <!-- Owner Section -->
        <section class="owner-section">
            <div class="owner-form">
                <h2>Restaurant Owner</h2>
                <form>
                    <label for="ownerName">Owner's Name</label>
                    <input type="text" id="ownerName" name="ownerName" required>

                    <label for="restaurantName">Restaurant Name</label>
                    <input type="text" id="restaurantName" name="restaurantName" required>

                    <label for="contactEmail">Contact Email</label>
                    <input type="email" id="contactEmail" name="contactEmail" required>

                    <button type="submit">Submit</button>
                </form>
            </div>
        </section>
        <!-- End Owner Section -->

        <!-- Main Content Section -->
        <main class="main_container">
            <!-- Add your existing content here -->
        </main>
        <!-- End Main Content Section -->

    </div>

    <script>
        function toggleMenu() {
            var menuSection = document.getElementById("menuSection");
            menuSection.style.display = (menuSection.style.display === "none") ? "block" : "none";
        }

        function showDineOutDetails() {
            // You can add logic to display more details about the dine out option here
            alert("Dine Out details: Visit our restaurant to enjoy a delightful dining experience!");
        }
    </script>

</body>

</html>
