<template>
  <!--
    โครงสร้างใหญ่สุดของหน้า Landing Page
    ใช้ tag <div> ตัวนอกสุดเพื่อจัดพื้นหลังและจัด layout ให้ทั้งหน้า
  -->
  <div class="landing-page">

    <!-- ========== TOP NAVBAR ส่วนเมนูด้านบน ========== -->
    <header class="navbar">
      <div class="navbar-left">
        <!-- โลโก้แอป (ตอนนี้ใช้เป็นตัวหนังสือไว้ก่อน เปลี่ยนเป็นรูปภาพได้) -->
        <div class="logo">LaosDoove</div>

        <!-- เมนูนำทางบนสุด (จะใส่ลิงก์ไปหน้าอื่นทีหลังก็ได้) -->
        <nav class="nav-links">
          <a href="#features">บริการทั้งหมด</a>
          <a href="#security">ความปลอดภัย</a>
          <a href="#faq">FAQ</a>
        </nav>
      </div>

      <div class="navbar-right">
        <!-- ปุ่ม login / sign up (ต่อไปอาจใช้ router-link ได้) -->
        <button class="btn-secondary">เข้าสู่ระบบ</button>
        <button class="btn-primary">เริ่มใช้งานฟรี</button>
      </div>
    </header>

    <!-- ========== HERO SECTION ส่วนหัวใหญ่ด้านบน ========== -->
    <section class="hero">
      <!-- คอลัมน์ซ้าย: ข้อความ -->
      <div class="hero-content">
        <!-- แท็กเล็กด้านบน -->
        <div class="hero-tag">All-in-one Lifestyle & Travel SuperApp</div>

        <!-- หัวข้อหลัก -->
        <h1 class="hero-title">
          Elevate the way you move,<br />
          stay & enjoy your city.
        </h1>

        <!-- คำอธิบายย่อ -->
        <p class="hero-subtitle">
          แอปเดียวที่รวมทุกบริการในเมืองของคุณ:
          รถบัสอัจฉริยะ, EV Charging, e-Bicycle, แท็กซี่,
          จองโรงแรม, ร้านอาหาร และสั่งของสดได้ในที่เดียว
        </p>

        <!-- ปุ่ม Call to Action -->
        <div class="hero-actions">
          <button class="btn-primary">ดาวน์โหลดแอป</button>
          <button class="btn-outline">ดูวิดีโอแนะนำ</button>
        </div>

        <!-- ปุ่ม Store (แค่ UI, ยังไม่ต้องใส่ลิงก์จริงก็ได้) -->
        <div class="store-buttons">
          <button class="store-btn">
            <span class="store-line-1">Download on</span>
            <span class="store-line-2">App Store</span>
          </button>
          <button class="store-btn">
            <span class="store-line-1">Get it on</span>
            <span class="store-line-2">Google Play</span>
          </button>
        </div>

        <!-- ข้อความความน่าเชื่อถือเล็ก ๆ -->
        <p class="hero-note">
          ใช้งานฟรี ไม่มีค่าธรรมเนียมแอบแฝง ยกเลิกได้ทุกเมื่อ
        </p>
      </div>

      <!-- คอลัมน์ขวา: mockup มือถือ -->
      <div class="hero-phone">
        <!-- กล่องนี้คือ mockup มือถือง่าย ๆ ถ้าอยากเปลี่ยนเป็นรูปภาพให้เอา <img> มาใส่แทน -->
        <div class="phone-frame">
          <div class="phone-notch"></div>
          <div class="phone-screen">
            <div class="phone-header">
              <div class="phone-app-name">SuperCity</div>
              <div class="phone-balance">
                <span>Wallet</span>
                <strong>฿ 2,450.50</strong>
              </div>
            </div>

            <!-- ไอคอนเมนูของแต่ละบริการบนมือถือ -->
            <div class="phone-grid">
              <div class="phone-service">
                <div class="icon-circle">🚌</div>
                <span>Bus</span>
              </div>
              <div class="phone-service">
                <div class="icon-circle">⚡</div>
                <span>EV Charge</span>
              </div>
              <div class="phone-service">
                <div class="icon-circle">🚲</div>
                <span>e-Bicycle</span>
              </div>
              <div class="phone-service">
                <div class="icon-circle">🚕</div>
                <span>Taxi</span>
              </div>
              <div class="phone-service">
                <div class="icon-circle">🏨</div>
                <span>Hotel</span>
              </div>
              <div class="phone-service">
                <div class="icon-circle">🍽️</div>
                <span>Restaurant</span>
              </div>
              <div class="phone-service">
                <div class="icon-circle">🛒</div>
                <span>Groceries</span>
              </div>
              <div class="phone-service">
                <div class="icon-circle">🎢</div>
                <span>Fun Park</span>
              </div>
            </div>

            <!-- สรุปการเดินทางล่าสุด -->
            <div class="phone-card">
              <div class="phone-card-row">
                <span>Last trip</span>
                <span class="pill pill-success">Completed</span>
              </div>
              <p>Electric Bus Line 05 • 12.3 km</p>
              <div class="phone-card-row">
                <span>Paid with Wallet</span>
                <strong>฿ 28.00</strong>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- ========== TRUST / SERVICES HIGHLIGHT ส่วนโชว์บริการหลัก ๆ ========== -->
    <section id="features" class="section trusted">
      <p class="section-label">บริการหลักใน SuperCity</p>
      <h2 class="section-title">All your urban journeys in one app.</h2>
      <p class="section-subtitle">
        เดินทาง พักผ่อน และใช้ชีวิตในเมืองได้สะดวกขึ้น ด้วยบริการที่ออกแบบมาเพื่อคุณ
      </p>

      <!-- การ์ดแสดงฟีเจอร์หลัก -->
      <div class="trusted-grid">
        <!-- การ์ดที่ 1 -->
        <div class="feature-card">
          <div class="feature-icon">🚌</div>
          <h3>Smart Bus & Taxi</h3>
          <p>
            วางแผนเส้นทาง ติดตามรถแบบเรียลไทม์ และเรียกแท็กซี่ได้จากในแอปเดียว
          </p>
        </div>

        <!-- การ์ดที่ 2 -->
        <div class="feature-card">
          <div class="feature-icon">⚡</div>
          <h3>EV Charging</h3>
          <p>
            หาสถานีชาร์จใกล้คุณ จองคิวล่วงหน้า และจ่ายผ่าน wallet ได้ทันที
          </p>
        </div>

        <!-- การ์ดที่ 3 -->
        <div class="feature-card">
          <div class="feature-icon">🏨</div>
          <h3>Stay & Dine</h3>
          <p>
            จองโรงแรม ร้านอาหาร และสั่งของสดเข้าบ้านได้จากที่เดียว
          </p>
        </div>
      </div>
    </section>

    <!-- ========== FEATURE SECTIONS แบบบล็อกยาวๆ (ซ้าย-ขวา) ========== -->
    <!-- section: Payment & Wallet -->
    <section class="section feature-row">
      <!-- รูป mockup ด้านซ้าย (จะเปลี่ยนเป็นรูปจริงทีหลังก็ได้) -->
      <div class="feature-image">
        <div class="mini-phone">
          <div class="mini-phone-header">
            SuperCity Wallet
          </div>
          <div class="mini-phone-body">
            <p class="mini-balance-label">ຍອດເງິນຄົງເຫຼືອ</p>
            <p class="mini-balance-value">50.000.0</p>
            <div class="mini-list">
              <div class="mini-item">
                <span>Bus Ticket</span>
                <span>- ฿ 28.00</span>
              </div>
              <div class="mini-item">
                <span>Hotel Booking</span>
                <span>- ฿ 850.00</span>
              </div>
              <div class="mini-item">
                <span>Groceries</span>
                <span>- ฿ 320.00</span>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- ข้อความอธิบายด้านขวา -->
      <div class="feature-text">
        <p class="section-label">Pay with confidence</p>
        <h2 class="section-title">กระเป๋าเงินเดียว ใช้ได้ทุกบริการในเมือง</h2>
        <p class="section-subtitle">
          เติมเงินครั้งเดียว แล้วใช้จ่ายกับรถบัส แท็กซี่ EV charging
          e-bicycle โรงแรม ร้านอาหาร และซูเปอร์มาร์เก็ตได้ทั้งหมด
        </p>
        <ul class="feature-list">
          <li>จ่ายแบบ contactless ได้ทั้งบนรถและที่จุดชำระเงิน</li>
          <li>แยกรายการใช้จ่ายตามหมวดหมู่ ดูย้อนหลังได้</li>
          <li>รับ cashback และแต้มสะสมจากทุกการเดินทาง</li>
        </ul>
        <button class="btn-primary">ดูวิธีใช้งาน Wallet</button>
      </div>
    </section>

    <!-- section: Booking & Planning -->
    <section class="section feature-row feature-row-reverse">
      <div class="feature-image">
        <div class="mini-card">
          <h3>Weekend in the City</h3>
          <p>Trip Plan</p>
          <ul class="mini-trip-list">
            <li>🚕 Taxi to Fun Park</li>
            <li>🎢 Fun Park Tickets</li>
            <li>🏨 Hotel Downtown</li>
            <li>🍽️ Dinner Reservation</li>
          </ul>
          <div class="mini-trip-footer">
            <span>ทั้งหมด</span>
            <strong>฿ 2,150.00</strong>
          </div>
        </div>
      </div>

      <div class="feature-text">
        <p class="section-label">Plan & book in minutes</p>
        <h2 class="section-title">วางทริปทั้งวัน ได้ในไม่กี่คลิก</h2>
        <p class="section-subtitle">
          จากการเดินทางไปสวนสนุก จองโรงแรม ไปจนถึงร้านอาหารมื้อเย็น
          จองทุกอย่างได้จากหน้าเดียว แล้วจ่ายผ่าน wallet ได้ทันที
        </p>
        <ul class="feature-list">
          <li>แนะนำเส้นทางและวิธีเดินทางที่คุ้มค่าที่สุด</li>
          <li>ดูราคาแบบเรียลไทม์ เปรียบเทียบตัวเลือกได้</li>
          <li>ซิงก์กับปฏิทินในมือถือ ไม่พลาดทุกการจอง</li>
        </ul>
        <button class="btn-primary">สำรวจดีลพิเศษ</button>
      </div>
    </section>

    <!-- ========== SECURITY SECTION ความปลอดภัย ========== -->
    <section id="security" class="section security">
      <p class="section-label">Prime security</p>
      <h2 class="section-title">ความปลอดภัยระดับธนาคาร</h2>
      <p class="section-subtitle">
        ข้อมูลการเดินทางและการชำระเงินของคุณถูกปกป้องด้วยมาตรฐานความปลอดภัยสูงสุด
      </p>

      <div class="security-grid">
        <div class="feature-card">
          <div class="feature-icon">🔒</div>
          <h3>Two-Factor Authentication</h3>
          <p>ยืนยันตัวตนสองชั้นทุกครั้งที่เข้าสู่ระบบหรือทำธุรกรรมสำคัญ</p>
        </div>
        <div class="feature-card">
          <div class="feature-icon">🛡️</div>
          <h3>Real-time Fraud Detection</h3>
          <p>ระบบแจ้งเตือนเมื่อพบพฤติกรรมที่ผิดปกติในบัญชีของคุณ</p>
        </div>
        <div class="feature-card">
          <div class="feature-icon">📱</div>
          <h3>Biometric Login</h3>
          <p>รองรับ Face ID / Fingerprint สำหรับการเข้าแอปอย่างรวดเร็วและปลอดภัย</p>
        </div>
        <div class="feature-card">
          <div class="feature-icon">📊</div>
          <h3>Full Transparency</h3>
          <p>ดูประวัติการเข้าใช้งานและการล็อกอินจากอุปกรณ์ต่าง ๆ ได้ทุกเวลา</p>
        </div>
      </div>
    </section>

    <!-- ========== FAQ SECTION คำถามที่พบบ่อย ========== -->
    <section id="faq" class="section faq">
      <p class="section-label">FAQ</p>
      <h2 class="section-title">คำถามที่พบบ่อย</h2>

      <!--
        ตอนนี้ FAQ ยังเป็นแบบ static (ข้อมูลคงที่)
        ถ้าภายหลังอยากใช้ API ก็สามารถเปลี่ยนให้ดึงข้อมูล FAQ จาก backend ได้
        เช่น ใช้ v-for loop แทนการเขียนแต่ละข้อด้วยมือ
      -->
      <div class="faq-item">
        <button class="faq-question">
          SuperCity รองรับเมืองไหนบ้าง?
        </button>
        <div class="faq-answer">
          ตอนนี้เราเริ่มให้บริการในบางเมืองหลัก
          และกำลังขยายไปยังเมืองอื่น ๆ อย่างต่อเนื่อง
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question">
          ต้องเสียค่าสมัครสมาชิกหรือไม่?
        </button>
        <div class="faq-answer">
          ดาวน์โหลดและสมัครใช้งานฟรี ไม่มีค่าธรรมเนียมรายเดือน
          คิดเฉพาะค่าบริการที่คุณใช้จริงเท่านั้น
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question">
          ข้อมูลบัตรหรือบัญชีธนาคารปลอดภัยหรือไม่?
        </button>
        <div class="faq-answer">
          เราเข้ารหัสข้อมูลตามมาตรฐานระดับธนาคาร
          และไม่เก็บหมายเลขบัตรเต็มรูปแบบบนเซิร์ฟเวอร์ของเรา
        </div>
      </div>
    </section>

    <!-- ========== FOOTER SECTION ด้านล่างสุด ========== -->
    <footer class="footer">
      <div class="footer-top">
        <div>
          <h3 class="footer-title">Elevate the way you move with SuperCity.</h3>
          <p class="footer-subtitle">
            พร้อมพาคุณออกเดินทาง ใช้ชีวิต และพักผ่อนในเมืองได้สะดวกกว่าที่เคย
          </p>
          <div class="store-buttons">
            <button class="store-btn">
              <span class="store-line-1">Download on</span>
              <span class="store-line-2">App Store</span>
            </button>
            <button class="store-btn">
              <span class="store-line-1">Get it on</span>
              <span class="store-line-2">Google Play</span>
            </button>
          </div>
        </div>
      </div>

      <div class="footer-bottom">
        <span>© 2025 SuperCity. All rights reserved.</span>
        <div class="footer-links">
          <a href="#">Privacy</a>
          <a href="#">Terms</a>
          <a href="#">Support</a>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
// ตอนนี้หน้า Landing Page นี้ยังไม่มี logic อะไรมาก
// ถ้าภายหลังต้องการ:
// - ดึงข้อมูลจาก API (เช่น รายการบริการ, เมืองที่รองรับ)
// - ทำ FAQ ให้พับ/กางได้ (accordion)
// - เชื่อมปุ่มต่าง ๆ กับ Vue Router
// ก็สามารถเพิ่ม script ตรงนี้ได้ เช่น ใช้ ref, reactive, onMounted ฯลฯ
</script>

<style scoped>
/* ========= ตัวตั้งค่าพื้นฐานของหน้า ========= */

.landing-page {
  min-height: 100vh;
  width: 100%;
  background: linear-gradient(to bottom, #15a19a);
  font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  color: #1f2430;
}


/* ========= Navbar ========= */

.navbar {
  width: 100%;
  padding: 16px 64px;
  box-sizing: border-box;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.navbar-left {
  display: flex;
  align-items: center;
  gap: 32px;
}

.logo {
  font-weight: 800;
  font-size: 20px;
  padding: 6px 12px;
  border-radius: 999px;
  background: #ffffff;
  box-shadow: 0 8px 24px rgba(15, 23, 42, 0.08);
}

.nav-links {
  display: flex;
  gap: 16px;
  font-size: 14px;
}

.nav-links a {
  text-decoration: none;
  color: #4b4f5c;
}

.nav-links a:hover {
  color: #6c3df4;
}

.navbar-right {
  display: flex;
  align-items: center;
  gap: 12px;
}

/* ========= Buttons ========= */

.btn-primary {
  border: none;
  border-radius: 999px;
  padding: 10px 20px;
  background: #6c3df4;
  color: #fff;
  font-weight: 600;
  font-size: 14px;
  cursor: pointer;
  box-shadow: 0 10px 30px rgba(108, 61, 244, 0.35);
}

.btn-primary:hover {
  filter: brightness(1.05);
}

.btn-secondary {
  border-radius: 999px;
  padding: 8px 16px;
  border: 1px solid #d0d4ff;
  background: #ffffff;
  font-size: 14px;
  cursor: pointer;
}

.btn-outline {
  border-radius: 999px;
  padding: 9px 18px;
  border: 1px solid #d0d4ff;
  background: transparent;
  font-size: 14px;
  cursor: pointer;
}

/* ========= HERO ========= */

.hero {
  width: 100%;
  min-height: calc(100vh - 80px); /* ให้ hero สูงประมาณเต็มจอ */
  padding: 40px 64px 64px;
  box-sizing: border-box;
  display: grid;
  grid-template-columns: minmax(0, 1.2fr) minmax(0, 1fr);
  gap: 40px;
  align-items: center;
}


.hero-tag {
  display: inline-flex;
  align-items: center;
  font-size: 12px;
  padding: 4px 10px;
  border-radius: 999px;
  background: #fff;
  border: 1px solid #e2d8ff;
  margin-bottom: 16px;
}

.hero-title {
  font-size: 32px;
  line-height: 1.2;
  margin: 0 0 16px;
}

.hero-subtitle {
  font-size: 14px;
  color: #4b4f5c;
  margin-bottom: 20px;
}

.hero-actions {
  display: flex;
  gap: 12px;
  margin-bottom: 20px;
}

.store-buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-bottom: 8px;
}

.store-btn {
  border-radius: 12px;
  border: none;
  padding: 8px 14px;
  background: #070816;
  color: white;
  min-width: 120px;
  text-align: left;
  cursor: pointer;
}

.store-line-1 {
  display: block;
  font-size: 10px;
  opacity: 0.8;
}

.store-line-2 {
  display: block;
  font-size: 14px;
  font-weight: 600;
}

.hero-note {
  font-size: 12px;
  color: #6b7280;
}

/* ========= HERO PHONE MOCKUP ========= */

.hero-phone {
  display: flex;
  justify-content: center;
}

.phone-frame {
  width: 260px;
  border-radius: 32px;
  padding: 16px 12px;
  background: linear-gradient(145deg, #1a1635, #2f275f);
  box-shadow: 0 24px 60px rgba(15, 23, 42, 0.5);
  position: relative;
}

.phone-notch {
  position: absolute;
  top: 8px;
  left: 50%;
  transform: translateX(-50%);
  width: 110px;
  height: 16px;
  border-radius: 999px;
  background: #050617;
}

.phone-screen {
  background: linear-gradient(to bottom, #fdfbff, #f4f3ff);
  border-radius: 24px;
  padding: 24px 18px 18px;
  margin-top: 8px;
}

.phone-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 18px;
}

.phone-app-name {
  font-weight: 700;
  font-size: 14px;
}

.phone-balance span {
  display: block;
  font-size: 10px;
  color: #6b7280;
}

.phone-balance strong {
  font-size: 14px;
}

.phone-grid {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 10px;
  margin-bottom: 18px;
}

.phone-service {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
  font-size: 11px;
}

.icon-circle {
  width: 32px;
  height: 32px;
  border-radius: 999px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #ffffff;
  box-shadow: 0 4px 12px rgba(15, 23, 42, 0.2);
}

.phone-card {
  background: #ffffff;
  border-radius: 16px;
  padding: 10px 12px;
  font-size: 11px;
  box-shadow: 0 10px 20px rgba(15, 23, 42, 0.08);
}

.phone-card-row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 4px;
}

.pill {
  padding: 2px 8px;
  border-radius: 999px;
  font-size: 10px;
}

.pill-success {
  background: #dcfce7;
  color: #166534;
}

/* ========= SECTIONS GENERAL ========= */

.section {
  width: 100%;
  padding: 48px 64px 56px;
  box-sizing: border-box;
}

.section-label {
  text-transform: uppercase;
  font-size: 11px;
  letter-spacing: 0.08em;
  color: #6c3df4;
  margin-bottom: 8px;
}

.section-title {
  font-size: 24px;
  margin: 0 0 8px;
}

.section-subtitle {
  font-size: 14px;
  color: #4b4f5c;
  max-width: 540px;
}

/* ========= TRUSTED / FEATURE CARDS ========= */

.trusted {
  text-align: center;
}

.trusted .section-subtitle {
  margin: 0 auto 24px;
}

.trusted-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 16px;
  margin-top: 16px;
}

.feature-card {
  background: #fff;
  padding: 18px 16px;
  border-radius: 20px;
  box-shadow: 0 16px 40px rgba(15, 23, 42, 0.06);
  text-align: left;
}

.feature-icon {
  width: 32px;
  height: 32px;
  border-radius: 999px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #f3e8ff;
  margin-bottom: 10px;
}

/* ========= FEATURE ROW (ภาพ + ข้อความ) ========= */

.feature-row {
  display: grid;
  grid-template-columns: minmax(0, 1.05fr) minmax(0, 1.15fr);
  gap: 32px;
  align-items: center;
}

.feature-row-reverse {
  grid-template-columns: minmax(0, 1.15fr) minmax(0, 1.05fr);
}

.feature-row-reverse .feature-image {
  order: 2;
}

.feature-row-reverse .feature-text {
  order: 1;
}

.feature-image {
  display: flex;
  justify-content: center;
}

/* mini phone / card mockups ใน section feature */
.mini-phone {
  width: 260px;
  border-radius: 24px;
  overflow: hidden;
  background: #070816;
  color: #e5e7eb;
  box-shadow: 0 18px 40px rgba(15, 23, 42, 0.5);
}

.mini-phone-header {
  padding: 12px 16px;
  font-size: 13px;
  font-weight: 600;
  background: linear-gradient(135deg, #6c3df4, #f97316);
}

.mini-phone-body {
  padding: 16px;
  background: radial-gradient(circle at top, #111827, #020617);
}

.mini-balance-label {
  font-size: 11px;
  color: #9ca3af;
}

.mini-balance-value {
  font-size: 20px;
  margin-bottom: 12px;
}

.mini-list {
  border-radius: 14px;
  background: rgba(15, 23, 42, 0.8);
  padding: 10px 12px;
  font-size: 11px;
}

.mini-item {
  display: flex;
  justify-content: space-between;
  margin-bottom: 4px;
}

.mini-item:last-child {
  margin-bottom: 0;
}

.mini-card {
  width: 260px;
  border-radius: 22px;
  padding: 16px;
  background: #ffffff;
  box-shadow: 0 18px 40px rgba(15, 23, 42, 0.15);
}

.mini-trip-list {
  list-style: none;
  padding: 0;
  margin: 8px 0 10px;
  font-size: 12px;
}

.mini-trip-list li {
  margin-bottom: 4px;
}

.mini-trip-footer {
  display: flex;
  justify-content: space-between;
  font-size: 13px;
  margin-top: 4px;
}

/* ข้อความใน feature row */
.feature-text .section-subtitle {
  margin-bottom: 12px;
}

.feature-list {
  list-style: none;
  padding: 0;
  margin: 0 0 16px;
  font-size: 14px;
  color: #4b4f5c;
}

.feature-list li::before {
  content: "•";
  margin-right: 8px;
  color: #6c3df4;
}

/* ========= SECURITY ========= */

.security {
  background: linear-gradient(to bottom, #f7f4ff, #f4f7ff);
  border-radius: 32px;
  margin-bottom: 32px;
}

.security-grid {
  margin-top: 20px;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 16px;
}

/* ========= FAQ ========= */

.faq {
  background: #ffffff;
  border-radius: 24px;
  box-shadow: 0 20px 60px rgba(15, 23, 42, 0.08);
  margin-bottom: 32px;
}

.faq-item {
  border-top: 1px solid #e5e7eb;
}

.faq-item:first-child {
  border-top: none;
}

.faq-question {
  width: 100%;
  padding: 14px 0;
  text-align: left;
  border: none;
  background: transparent;
  font-weight: 500;
  cursor: pointer;
}

.faq-answer {
  font-size: 13px;
  color: #4b4f5c;
  padding-bottom: 12px;
}

/* ========= FOOTER ========= */

.footer {
  background: #070816;
  color: #e5e7eb;
  padding: 32px 24px 24px;
  margin-top: 24px;
}

.footer-top {
  width: 100%;
  max-width: none;
  margin: 0 0 24px;
  box-sizing: border-box;
}


.footer-title {
  font-size: 20px;
  margin-bottom: 6px;
}

.footer-subtitle {
  font-size: 13px;
  color: #9ca3af;
  margin-bottom: 12px;
}

.footer-bottom {
  width: 100%;
  box-sizing: border-box;
  border-top: 1px solid rgba(148, 163, 184, 0.5);
  padding-top: 12px;
  display: flex;
  justify-content: space-between;
  font-size: 12px;
  color: #9ca3af;
}

.footer-links {
  display: flex;
  gap: 12px;
}

.footer-links a {
  color: #9ca3af;
  text-decoration: none;
}

/* ========= RESPONSIVE สำหรับจอเล็ก ========= */

@media (max-width: 900px) {
  .hero {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .hero-actions {
    justify-content: center;
  }

  .store-buttons {
    justify-content: center;
  }

  .hero-phone {
    order: -1;
  }

  .feature-row,
  .feature-row-reverse {
    grid-template-columns: 1fr;
  }

  .footer-bottom {
    flex-direction: column;
    gap: 8px;
    align-items: flex-start;
  }
}
</style>
