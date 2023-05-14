<template>
    <footer class="footer">
      <div class="footer-container">
        <div class="footer-section">
          <h4>Контакты</h4>
          <p>Телефон: 123-456-789</p>
          <p>Email: info@example.com</p>
          <div class="social-icons">
            <a href="#" class="icon">
              <i class="fab fa-facebook-f"></i>
            </a>
            <a href="#" class="icon">
              <i class="fab fa-twitter"></i>
            </a>
            <a href="#" class="icon">
              <i class="fab fa-instagram"></i>
            </a>
          </div>
        </div>
        <div class="footer-section">
          <h4>Подписаться</h4>
          <div class="subscribe-form">
            <input type="email" placeholder="Введите ваш email" />
            <button>Подписаться</button>
          </div>
        </div>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'Footer',
  };
  </script>
  
  <style scoped>
  .footer {
    background-color: #9c27b0;
    padding: 20px;
    color: #fff;
    position: fixed;
    bottom: 0;
    width: 100%;
  }
  
  .footer-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  
  .footer-section {
    width: 100%;
    max-width: 300px;
    margin: 10px;
  }
  
  h4 {
    margin-bottom: 10px;
  }
  
  .subscribe-form {
    display: flex;
    margin-top: 10px;
  }
  
  .subscribe-form input {
    flex: 1;
    padding: 5px;
  }
  
  .subscribe-form button {
    background-color: #fff;
    color: #9c27b0;
    border: none;
    padding: 5px 10px;
    border-radius: 4px;
    cursor: pointer;
  }
  
  .social-icons {
    display: flex;
    justify-content: center;
    margin-top: 10px;
  }
  
  .icon {
    margin: 0 10px;
    color: #fff;
    font-size: 20px;
  }
  
  @media (min-width: 768px) {
    .footer-container {
      justify-content: space-between;
    }
  
    .footer-section {
      width: 30%;
    }
  }
  </style>
  