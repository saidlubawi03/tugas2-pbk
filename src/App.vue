<template>
  <div class="container">
    <div class="header">
      <div class="left-header">
        <div class="logo">ADMIN BAIK</div>
        <div class="user-info">
          <div :class="{ 'balance': true, 'positive': balance > 0, 'negative': balance <= 0 }">{{ balance }}</div>
          <div class="points">{{ points }}</div>
        </div>
      </div>
      <div class="right-header">
        <div class="join-button">Bergabung</div>
      </div>
    </div>
    <div class="main">
      <div class="deposit-banner">
        <div class="deposit-title">FREELANCE</div>
        <div class="payment-method">AMAN DAN TERPECAYA</div>
        <div class="frelance-promo">INFO LEBIH LANJUT</div>
        <div class="instruction">BISA DI AKSES MELALUI QRIS</div>
        <div class="qr-code"></div>
        <div class="footer-deposit">ADMIN BAIK</div>
      </div>
      <div class="game-menu">
        <div class="game-item">LOGO</div>
        <div class="game-item">WEB DEVALOPMENT</div>
        <div class="game-item">PENULISAN KONTEN</div>
        <div class="game-item">FOTOGRAFI</div>
        <div class="game-item">BENNER ONLINE</div>
      </div>
      <div class="login-form">
        <div class="login-title">Masuk</div>
        <form>
          <div class="form-group">
            <label for="username">username</label>
            <input type="text" id="username" name="username" />
          </div>
          <div class="form-group">
            <label for="password">Kata sandi</label>
            <input type="password" id="password" name="password" />
          </div>
          <button type="submit">Masuk</button>
        </form>
        <div class="register-link">
          <a href="#">Daftar Sekarang</a>
        </div>
      </div>
      <div class="footer">
        <div class="footer-text">
          <a href="#">RTP ADMIN BAIK</a>
          <div class="desktop-wap">
            <a href="#">Desktop</a> |
            <a href="#">wap</a>
          </div>
        </div>
        <div class="navigation">
          <a href="#">BERANDA</a>
          <a href="#">PROMOSI</a>
          <a href="#">PERISTIWA</a>
          <a href="#">ADA APA</a>
          <a href="#">Obrolan Langsung</a>
          <span :style="{ backgroundColor: badgeColor }" class="badge">{{ notificationCount }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      balance: 13.15,
      points: 284,
      notificationCount: 7,
      badgeColor: '#007bff' 
    };
  }
};
</script>