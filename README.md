<html lang="fi">
  <head>
    <!-- Meta tags and styles should be placed here -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Self-Help-You</title>
    <style>
      /* Reset default margin and padding */
      body, html {
        margin: 0;
        padding: 0;
        font-family: Arial, sans-serif;
      }

      /* Styling the navigation bar */
      .navbar {
        background-color: #e1705d; /* Red background color */
        overflow: hidden; /* Ensures the content is contained within the navbar */
        text-align: center; /* Centers the links */
      }

      /* Styling each link inside the navbar */
      .navbar a {
        display: inline-block; /* Display links horizontally */
        padding: 14px 20px; /* Padding inside each link */
        text-decoration: none; /* Removes underline from links */
        color: white; /* White text color */
        font-size: 16px; /* Adjusted font size */
        transition: background-color 0.3s ease; /* Smooth transition for background color change */
      }

      /* Hover effect for the links */
      .navbar a:hover {
        background-color: #ddd; /* Light background when hovered */
        color: black; /* Change text color when hovered */
      }

      /* Active link styling (when a link is clicked or active) */
      .navbar a.active {
        background-color: #0e194d; /* Blue background for active link */
        color: white; /* Keep text white for active link */
      }

      /* Hamburger menu icon styling */
      .navbar .icon {
        display: none;
        font-size: 27px;
        color: white;
        padding: 14px 20px;
        background-color: #0e194d;
        cursor: pointer;
        z-index: 2;
      }

      /* For small screens (mobile devices) */
      @media screen and (max-width: 600px) {
        .navbar a {
          display: none; /* Hide the links by default */
          width: 100%; /* Make the links take full width */
          text-align: left; /* Align links to the left */
          padding: 14px; /* Adjust padding for the links */
        }

        /* Display the hamburger icon */
        .navbar .icon {
          display: block;
        }

        /* When the hamburger icon is clicked, show the links */
        .navbar.responsive a {
          display: block;
        }

        .navbar.responsive .icon {
          position: absolute;
          right: 0;
          top: 0;
        }
      }

      /* Styling for the header with rolling text effect */
      .header {
        background-color: #0e194d;
        color: white;
        padding: 20px;
        text-align: center;
        position: relative;
        overflow: hidden;
      }

      /* Rolling text effect */
      .header h1 {
        display: inline-block;
        font-size: 27px;
        white-space: nowrap; /* Prevent the title from wrapping */
        animation: rollText 10s linear infinite; /* Apply animation to roll the text */
        position: relative;
        z-index: 2;
      }

      /* Keyframes for rolling text animation */
      @keyframes rollText {
        10% {
          transform: translateX(100%); /* Start off to the right */
        }
        100% {
          transform: translateX(-100%); /* End off to the left */
        }
      }

      /* New Text Section */
      .intro-text {
        text-align: center;
        padding: 40px;
        background-color: #f0f0f0; /* Light grey background */
        margin-top: 20px; /* Add some spacing from the header */
      }

      .intro-text h2 {
        font-size: 24px;
        color: #0e194d; /* Blue color for the title */
      }

      .intro-text p {
        font-size: 14px;
        color: #0e194d; /* Blue color for the paragraph text */
      }

      /* Box Container */
      .box-container {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 10px;
        margin-top: 40px;
      }

      /* Box Styles */
      .box {
        background-color: #38B6FF;
        box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3), -2px -2px 5px rgba(92, 97, 102, 0.5);
        border: 1px solid #ddd;
        border-radius: 8px;
        transition: transform 0.3s ease;
        text-align: center;
        overflow-wrap: break-word; /* Prevent overflow of long words */
      }

      /* Separate header, content, and footer sections */
      .box-header {
        padding: 10px 0;
        text-align: center;
      }

      .box-content {
        padding: 10px;
        text-align: center;
      }

      .box-footer {
        padding: 10px;
        text-align: center;
      }

      /* Title and text styles inside the box */
      .box h3 {
        margin: 0;
        font-size: 24px;
        color: #0e194d;
      }

      .box p {
        font-size: 14px;
        color: #0e194d;
      }

      .box-footer a {
        text-decoration: none;
        background-color: #0e194d;
        padding: 10px 15px;
        color: white;
        border-radius: 5px;
        display: inline-block; /* Make the link behave like a button */
      }

      /* Hover effect */
      .box:hover {
        transform: translateY(-10px);
      }

      footer {
        text-align: center;
        padding: 20px;
        background-color: #0e194d;
        color: white;
      }

      footer a {
        text-decoration: none;
        color: white;
        font-size: 16px;
        margin: 0 15px;
        transition: color 0.3s ease;
      }

      footer a:hover {
        color: #FF5733; /* Color when hovered (e.g., light orange) */
      }

      footer a:visited {
        color: #8E44AD; /* Purple color after the link is visited */
      }

      /* Footer Bottom */
      .footer-bottom {
        padding-top: 10px;
      }

      /* Add space between the last box and footer */
      section {
        padding-bottom: 40px; /* Space between content and footer */
      }
    </style>
  </head>
  <body>
    <!-- Top Navigation Bar placed before the header -->
    <div class="navbar" id="myNavbar">
      <a href="#home" class="active">Koti</a>
      <a href="/Meista">Meistä</a>
      <a href="/Yritys">Yritys</a>
      <a href="/Palvelut">Palvelut</a>
      <a href="/Koulutus">Koulutus</a>

      <!-- Hamburger Icon -->
      <a href="javascript:void(0);" class="icon" onclick="toggleNavbar()">&#9776;</a>
    </div>

    <!-- Header with rolling text effect -->
    <div class="header">
      <h1>Self-Help-You</h1>
    </div>

    <!-- New Section with Grey Background and Title/Text -->
    <div class="intro-text">
      <h2>- osana pienyrityksien Tulevaisuuden Suunnittelua</h2>
    </div>

    <!-- Main Content -->
    <section>
      <div class="box-container">
        <!-- Box Components -->
        <div class="box">
          <div class="box-header">
            <h3>Meistä</h3>
          </div>
          <div class="box-content">
            <p>Lue lisää meistä ja referensseistämme.</p>
          </div>
          <div class="box-footer">
            <a href="/Meista">Lue lisää</a>
          </div>
        </div>

        <div class="box">
          <div class="box-header">
            <h3>Yritys</h3>
          </div>
          <div class="box-content">
            <p>Tutustu yritykseemme sekä henkilökuntaamme.</p>
          </div>
          <div class="box-footer">
            <a href="/Yritys">Tutustu</a>
          </div>
        </div>

        <div class="box">
          <div class="box-header">
            <h3>Palvelut</h3>
          </div>
          <div class="box-content">
            <p>Kuinka voimme auttaa Sinua ja yritystoimintaasi tulevaisuuden suunnittelussa.</p>
          </div>
          <div class="box-footer">
            <a href="/Palvelut">Katso tästä</a>
          </div>
        </div>

        <div class="box">
          <div class="box-header">
            <h3>Koulutus</h3>
          </div>
          <div class="box-content">
            <p>Monipuoliset ja monimuotoiset koulutukset räätälöity Sinun yritystarpeillesi.</p>
          </div>
          <div class="box-footer">
            <a href="/Koulutus">Lue lisää</a>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer>
      <div class="footer-section contact">
        <h4>Self-Help-You - osana yrityksesi tulevaisuuden suunnittelua</h4>
        <a href="#Otayhteytta">Ota yhteyttä</a>
        <a href="#Sahkoposti">Sähköposti</a>
        <a href="#Kanavat">Kanavat</a>
      </div>
      <div class="footer-bottom">
        <p>&copy; 2025 Self-Help-You. Kaikki oikeudet pidätetään.</p>
      </div>
    </footer>

    <script>
      /* Function to toggle the navbar on small screens */
      function toggleNavbar() {
        var navbar = document.getElementById("myNavbar");
        navbar.classList.toggle("responsive");
      }
    </script>
  </body>
</html>
