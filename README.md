<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Navbar with Tools Categories and Marketplace</title>
    <style>
        /* Resetting default styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Body styling */
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            padding: 20px;
        }

        /* Navbar container */
        .navbar {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 15px;
            background-color: #333;
            padding: 10px 20px;
            border-radius: 30px;
            margin-bottom: 20px;
        }

        /* Navbar buttons and links */
        .navbar-section button, .navbar-section a {
            display: inline-block;
            padding: 8px 16px;
            color: white;
            font-weight: bold;
            font-size: 14px;
            text-decoration: none;
            background-color: #444;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            transition: all 0.3s ease;
            position: relative;
        }

        .navbar-section button:hover, .navbar-section a:hover {
            background-color: #00c8ff;
            color: black;
        }

        /* Dropdown container */
        .dropdown {
            position: relative;
        }

        /* Dropdown content */
        .dropdown-content {
            display: none;
            position: absolute;
            top: 100%;
            left: 0;
            background-color: #555;
            border-radius: 8px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            overflow: hidden;
            z-index: 1000;
        }

        .dropdown-content a {
            display: block;
            padding: 8px 16px;
            color: white;
            text-decoration: none;
            font-size: 13px;
            transition: all 0.3s ease;
        }

        .dropdown-content a:hover {
            background-color: #00c8ff;
            color: black;
        }

        /* Show dropdown on hover */
        .dropdown:hover .dropdown-content {
            display: block;
        }

        /* Tools Categories Section */
        .categories-container {
            margin: 20px 0;
        }

        .categories-title {
            font-size: 20px;
            font-weight: bold;
            margin-bottom: 10px;
        }

        .categories {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .category-item {
            background-color: #444;
            color: white;
            padding: 10px 15px;
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .category-item:hover {
            background-color: #00c8ff;
            color: black;
        }

        /* Marketplace Section */
        .marketplace {
            margin-top: 30px;
        }

        .marketplace-title {
            font-size: 22px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        .ad-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
        }

        .ad-card {
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            width: 200px;
        }

        .ad-card img {
            width: 100%;
            height: 150px;
            object-fit: cover;
        }

        .ad-card .content {
            padding: 10px;
        }

        .ad-card .content h3 {
            font-size: 16px;
            margin-bottom: 5px;
        }

        .ad-card .content p {
            font-size: 14px;
            color: #555;
        }
    </style>
</head>
<body>

    <!-- Navbar -->
    <div class="navbar">
        <div class="navbar-section"><a href="#">HOME</a></div>
        <div class="navbar-section dropdown">
            <button>URL Shortener</button>
            <div class="dropdown-content">
                <a href="#">Shorten</a>
                <a href="#">Manage</a>
                <a href="#">Analytics</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>Temporary Email</button>
            <div class="dropdown-content">
                <a href="#">Generate</a>
                <a href="#">Manage</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>SMS Sender</button>
            <div class="dropdown-content">
                <a href="#">Send SMS</a>
                <a href="#">History</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>Proxy Services</button>
            <div class="dropdown-content">
                <a href="#">SOCKS5</a>
                <a href="#">HTTP</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>IP Lookup</button>
            <div class="dropdown-content">
                <a href="#">Lookup</a>
                <a href="#">Details</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>Fake Screenshot</button>
            <div class="dropdown-content">
                <a href="#">Generate</a>
                <a href="#">Options</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>US Address</button>
            <div class="dropdown-content">
                <a href="#">Generate</a>
                <a href="#">Save</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>Fake Address</button>
            <div class="dropdown-content">
                <a href="#">Generate</a>
                <a href="#">Manage</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>Front Generator</button>
            <div class="dropdown-content">
                <a href="#">Template</a>
                <a href="#">Preview</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>Temp Number</button>
            <div class="dropdown-content">
                <a href="#">Generate</a>
                <a href="#">History</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>Sent SMS</button>
            <div class="dropdown-content">
                <a href="#">History</a>
                <a href="#">Track</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>Sent Email</button>
            <div class="dropdown-content">
                <a href="#">History</a>
                <a href="#">Track</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>WhatsApp Msg</button>
            <div class="dropdown-content">
                <a href="#">Send</a>
                <a href="#">History</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>Voice Msg</button>
            <div class="dropdown-content">
                <a href="#">Send</a>
                <a href="#">History</a>
            </div>
        </div>
        <div class="navbar-section dropdown">
            <button>Email to SMS</button>
            <div class="dropdown-content">
                <a href="#">Send</a>
                <a href="#">History</a>
            </div>
        </div>
    </div>

    <!-- Tools Categories Section -->
    <div class="categories-container">
        <div class="categories-title">TOOLS CATEGORIES</div>
        <div class="categories">
            <div class="category-item">Accessibility</div>
            <div class="category-item">AI Tools</div>
            <div class="category-item">APIs</div>
            <div class="category-item">Audio & Sounds</div>
            <div class="category-item">CSS</div>
            <div class="category-item">Databases</div>
            <div class="category-item">Design</div>
            <div class="category-item">Docs</div>
            <div class="category-item">E-mail</div>
            <div class="category-item">Fonts</div>
            <div class="category-item">HTML</div>
            <div class="category-item">Images</div>
            <div class="category-item">JavaScript</div>
            <div class="category-item">Learning</div>
            <div class="category-item">Performance</div>
        </div>
    </div>

    <!-- Marketplace Section -->
    <div class="marketplace">
        <div class="marketplace-title">Marketplace Ads</div>
        <div class="ad-grid">
            <div class="ad-card">
                <img src="https://via.placeholder.com/200x150" alt="Ad 1">
                <div class="content">
                    <h3>Ad Title 1</h3>
                    <p>Ad description goes here.</p>
                </div>
            </div>
            <div class="ad-card">
                <img src="https://
