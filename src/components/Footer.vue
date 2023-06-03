<template>
  <footer class="footer">
    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <div class="footer-section">
            <h4 class="footer-section-title">Enlaces útiles</h4>
            <ul class="footer-links">
              <li><a href="#">Inicio</a></li>
              <li><a href="#">Acerca de nosotros</a></li>
              <li><a href="#">Servicios</a></li>
              <li><a href="#">Contacto</a></li>
            </ul>
          </div>
        </div>
        <div class="col-md-4">
          <div class="footer-section">
            <h4 class="footer-section-title">Redes sociales</h4>
            <div class="social-icons">
              <a
                href="https://www.facebook.com/"
                class="social-icon"
                target="_blank"
              >
                <img
                  src="../assets/faceLogo.png"
                  alt="Facebook"
                  class="icon-img"
                />
              </a>
              <a
                href="https://twitter.com/"
                class="social-icon"
                target="_blank"
              >
                <img
                  src="../assets/twitterLogo.png"
                  alt="Twitter"
                  class="icon-img"
                />
              </a>
              <a
                href="https://www.instagram.com/"
                class="social-icon"
                target="_blank"
              >
                <img
                  src="../assets/insta.png"
                  alt="Instagram"
                  class="icon-img"
                />
              </a>
              <a
                href="https://www.tiktok.com/"
                class="social-icon"
                target="_blank"
              >
                <img
                  src="../assets/tiktokFondo.png"
                  alt="TikTok"
                  class="icon-img"
                />
              </a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="footer-section">
            <h4 class="footer-section-title">Información de contacto</h4>
            <ul class="footer-links">
              <li>Dirección: Wall Street</li>
              <li>Teléfono: 123456789</li>
              <li>Email: locangas@gmail.com</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooteR",
};
</script>

<style>
.footer {
  background-color: #888888;
  padding: 30px 0;
  color: #fff;
}

.footer .container {
  max-width: 1200px;
  margin: 0 auto;
}

.footer .row {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

.footer-section {
  margin-bottom: 30px;
  text-align: center;
}

.footer-section-title {
  color: #fff;
  font-size: 18px;
  font-weight: bold;
  margin-bottom: 10px;
}

.footer-links {
  list-style: none;
  padding: 0;
  margin: 0;
}

.footer-links li {
  margin-bottom: 5px;
}

.footer-links a {
  color: #fff;
  text-decoration: none;
  transition: color 0.3s, border-bottom-color 0.3s;
}

.footer-links a:hover,
.footer-links a:focus {
  color: #000;
  border-bottom: 1px solid #000;
}

.social-icons {
  display: flex;
  justify-content: center;
}

.social-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background-color: #fff;
  margin: 5px;
  transition: transform 0.3s;
}

.icon-img {
  width: 24px;
  height: 24px;
}

.social-icon:hover {
  transform: scale(1.2);
}
</style>
