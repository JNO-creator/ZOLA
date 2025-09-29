  .navbar {
    background-color: #e1705d;
    overflow: hidden;
    text-align: center;
    height: 48px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .navbar a {
    display: inline-block;
    padding: 14px 20px;
    text-decoration: none;
    color: white;
    font-size: 16px;
    transition: background-color 0.3s ease;
  }

  .navbar a:hover {
    background-color: #ddd;
    color: black;
  }

  .navbar a.active {
    background-color: #0e194d;
    color: white;
  }

  .navbar .icon {
    display: none;
    font-size: 27px;
    color: white;
    padding: 14px 20px;
    background-color: #0e194d;
    cursor: pointer;
    z-index: 2;
  }

  @media screen and (max-width: 600px) {
    .navbar a {
      display: none;
      width: 100%;
      text-align: left;
      padding: 14px;
    }
    .navbar .icon {
      display: block;
    }
    .navbar.responsive a {
      display: block;
    }
    .navbar.responsive .icon {
      position: absolute;
      right: 0;
      top: 0;
    }
  }

  .header {
    background-color: #0e194d;
    color: white;
    padding: 20px;
    text-align: center;
    position: relative;
    overflow: hidden;
  }
  .header h1 {
    display: inline-block;
    font-size: 27px;
    white-space: nowrap;
    animation: rollText 10s linear infinite;
    position: relative;
    z-index: 2;
  }

  @keyframes rollText {
    10% {
      transform: translateX(100%);
    }
    100% {
      transform: translateX(-100%);
    }
  }

  .intro-text {
    text-align: center;
    padding: 40px;
    background-color: #f0f0f0;
    margin-top: 20px;
  }

  .intro-text h2 {
    font-size: 24px;
    color: #0e194d;
  }

  .intro-text p {
    font-size: 14px;
    color: #0e194d;
  }

  .box-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 10px;
    margin-top: 40px;
  }

  .box {
    background-color: #38B6FF;
    box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3), -2px -2px 5px rgba(92, 97, 102, 0.5);
    border: 1px solid #ddd;
    border-radius: 8px;
    transition: transform 0.3s ease;
    text-align: center;
    overflow-wrap: break-word;
  }

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
    display: inline-block;
  }

  .box:hover {
    transform: translateY(-10px);
  }

  footer {
    text-align: center;
    padding: 0;
    background-color: #0e194d;
    color: white;
    height: 48px;
    display: flex;
    align-items: center;
    justify-content: center;
    box-sizing: border-box;
  }

  footer .footer-section {
    width: 100%;
  }

  footer h4, footer a, footer p {
    margin: 0;
    padding: 0 8px;
    font-size: 16px;
    line-height: 1.2;
    vertical-align: middle;
  }

  footer a {
    text-decoration: none;
    color: white;
    font-size: 16px;
    margin: 0 15px;
    transition: color 0.3s ease;
  }

  footer a:hover {
    color: #FF5733;
  }

  footer a:visited {
    color: #8E44AD;
  }

  .footer-bottom {
    display: none; /* Hide the separate bottom section, as everything fits in one line now */
  }

  section {
    padding-bottom: 40px;
  }
</style>
KotiMeistäYritysPalvelutKoulutus
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
</section>

<!-- Footer -->
  <footer>
      <div class="footer-section contact">
          <h4>Self-Help-You</h4>
          <a href="/Otayhteytta" class="cta-btn">Ota yhteyttä</a>
          <a href="/Sahkoposti" class="cta-btn">Sähköposti</a>
          <a href="/Kanavat" class="cta-btn">Kanavat</a>
      </div>
      <div class="footer-bottom">
          <p>&copy; 2025 Self-Help-You. Kaikki oikeudet pidätetään.</p>
      </div>
  </footer>
<footer>
  <div class="footer-section contact">
    <h4>Self-Help-You - osana yrityksesi tulevaisuuden suunnittelua</h4>
    <a href="#Otayhteytta">Ota yhteyttä</a>
    <a href="#Sahkoposti">Sähköposti</a>
    <a href="#Kanavat">Kanavat</a>
    <span style="margin-left: 16px;">&copy; 2025 Self-Help-You. Kaikki oikeudet pidätetään.</span>
  </div>
</footer>

  <script>
      /* Function to toggle the navbar on small screens */
      function toggleNavbar() {
          var navbar = document.getElementById("myNavbar");
          navbar.classList.toggle("responsive");
      }
  </script>
<script>
  function toggleNavbar() {
    var navbar = document.getElementById("myNavbar");
    navbar.classList.toggle("responsive");
  }
</script>
