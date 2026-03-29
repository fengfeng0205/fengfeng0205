<template>
  <div>
    <!-- ==================== 主页 ==================== -->
    <div v-if="currentPage === 'home'" class="app">
      <!-- 导航栏 -->
      <nav class="navbar">
        <div class="container">
          <div class="nav-content">
            <div class="logo">Mas...</div>
            <div class="nav-links">
              <a href="#">Features</a>
              <a href="#">Testimonials</a>
              <a href="#">Company</a>
            </div>
            <button class="btn-download">Download</button>
          </div>
        </div>
      </nav>

      <!-- Hero 区域 -->
      <section class="hero">
        <div class="container">
          <div class="hero-content">
            <span class="badge">WANT MORE COMPONENTS?</span>
            <h1>Maximize Your Efficiency with ProductivityPro</h1>
            <p>Our intuitive platform helps you manage tasks, projects, and deadlines with ease.</p>
            <button class="btn-primary" @click="currentPage = 'signup'">
              Get started for free today!
            </button>
          </div>
        </div>
      </section>

      <!-- 功能区域 1 - 三个核心功能（添加背景图案） -->
      <section class="features">
        <div class="container">
          <h2 class="section-title">Maximize Your Efficiency with ProductivityPro</h2>
          <div class="features-grid">
            <div class="feature-card">
              <!-- 添加背景图案 -->
              <div class="bg-pattern pattern-checklist"></div>
              <div class="bg-pattern pattern-flow"></div>
              <div class="feature-icon">📋</div>
              <h3>Test Management</h3>
              <ul>
                <li>Test management for your team.</li>
                <li>Track progress and identify bottlenecks.</li>
              </ul>
            </div>
            <div class="feature-card">
              <!-- 添加背景图案 -->
              <div class="bg-pattern pattern-clock"></div>
              <div class="bg-pattern pattern-trend"></div>
              <div class="feature-icon">⏱️</div>
              <h3>Time Tracking</h3>
              <ul>
                <li>Track time spent on tasks.</li>
                <li>Analyze productivity trends.</li>
              </ul>
            </div>
            <div class="feature-card">
              <!-- 添加背景图案 -->
              <div class="bg-pattern pattern-team"></div>
              <div class="bg-pattern pattern-chat"></div>
              <div class="feature-icon">🤝</div>
              <h3>Collaboration Tools</h3>
              <ul>
                <li>Collaborate with colleagues in real-time.</li>
                <li>Share files, comments, and chat.</li>
              </ul>
            </div>
          </div>
        </div>
      </section>

      <!-- 目标区域 1 - 带背景图案 -->
      <section class="goals">
        <div class="container">
          <div class="goals-content">
            <h2>Set and track your goals for success</h2>
            <div class="goals-list">
              <div class="goal-item">
                <div class="bg-pattern pattern-target"></div>
                <div class="bg-pattern pattern-dots"></div>
                <h3>Set and track your goals for success</h3>
                <ul>
                  <li>Define clear objectives.</li>
                  <li>Monitor progress regularly.</li>
                </ul>
              </div>
              <div class="goal-item">
                <div class="bg-pattern pattern-chart"></div>
                <div class="bg-pattern pattern-lines"></div>
                <h3>Test and track your goals for success</h3>
                <ul>
                  <li>Test new features or changes.</li>
                  <li>Measure performance against goals.</li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- 目标区域 2 - 带背景图案 -->
      <section class="goals-alt">
        <div class="container">
          <div class="goals-content">
            <h2>Set and track your goals for success</h2>
            <div class="goals-list">
              <div class="goal-item">
                <div class="bg-pattern pattern-star"></div>
                <div class="bg-pattern pattern-wave"></div>
                <h3>Set and track your goals for success</h3>
                <ul>
                  <li>Define specific targets.</li>
                  <li>Track progress towards goals.</li>
                </ul>
              </div>
              <div class="goal-item">
                <div class="bg-pattern pattern-gear"></div>
                <div class="bg-pattern pattern-grid"></div>
                <h3>Test and track your goals for success</h3>
                <ul>
                  <li>Test new features or changes.</li>
                  <li>Measure performance against goals.</li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- 评价区域 - 带背景图案 -->
      <section class="testimonials">
        <div class="container">
          <h2 class="section-title">Testimonials from our members</h2>
          <div class="testimonials-grid">
            <div class="testimonial-card">
              <div class="bg-pattern pattern-quote"></div>
              <p class="quote">"I love how easy it is to manage my tasks and projects. The interface is intuitive and saves me hours every week."</p>
              <p class="author">— John Doe</p>
            </div>
            <div class="testimonial-card">
              <div class="bg-pattern pattern-heart"></div>
              <p class="quote">"The platform is user-friendly and has helped me stay organized. My productivity has increased by 40%."</p>
              <p class="author">— Jane Smith</p>
            </div>
            <div class="testimonial-card">
              <div class="bg-pattern pattern-star-sm"></div>
              <p class="quote">"I highly recommend ProductivityPro to anyone looking to improve their productivity. It's a game-changer!"</p>
              <p class="author">— Sarah Johnson</p>
            </div>
            <div class="testimonial-card">
              <div class="bg-pattern pattern-bubble"></div>
              <p class="quote">"I've been using ProductivityPro for a few months now and I'm really impressed with the features."</p>
              <p class="author">— Mark Thompson</p>
            </div>
            <div class="testimonial-card">
              <div class="bg-pattern pattern-sparkle"></div>
              <p class="quote">"This platform has made managing my workload so much easier."</p>
              <p class="author">— Emily Davis</p>
            </div>
            <div class="testimonial-card">
              <div class="bg-pattern pattern-crown"></div>
              <p class="quote">"I never thought I'd achieve such high productivity with just a few clicks."</p>
              <p class="author">— Michael Brown</p>
            </div>
          </div>
        </div>
      </section>

      <!-- CTA 区域 -->
      <section class="cta">
        <div class="container">
          <div class="cta-content">
            <h2>Ready to get started?</h2>
            <button class="btn-cta" @click="currentPage = 'signup'">Get In Touch</button>
          </div>
        </div>
      </section>

      <!-- 页脚 -->
      <footer class="footer">
        <div class="container">
          <div class="footer-content">
            <div class="footer-section">
              <h3>Company Info</h3>
              <ul>
                <li><a href="#">About Us</a></li>
                <li><a href="#">Careers</a></li>
                <li><a href="#">Contact</a></li>
                <li><a href="#">Legal</a></li>
                <li><a href="#">Privacy Policy</a></li>
              </ul>
            </div>
            <div class="footer-section">
              <h3>Features</h3>
              <ul>
                <li><a href="#">Easy to use interface</a></li>
                <li><a href="#">Powerful search</a></li>
                <li><a href="#">Customizable templates</a></li>
              </ul>
            </div>
            <div class="footer-section">
              <h3>Testimonials</h3>
              <ul>
                <li><a href="#">Read what our customers say</a></li>
                <li><a href="#">Success stories</a></li>
              </ul>
            </div>
            <div class="footer-section">
              <h3>Get In Touch</h3>
              <ul>
                <li><a href="#">support@productivitypro.com</a></li>
                <li><a href="#">+1 (555) 123-4567</a></li>
              </ul>
            </div>
          </div>
          <div class="footer-bottom">
            <p>© 2025 ProductivityPro. All rights reserved.</p>
          </div>
        </div>
      </footer>
    </div>

    <!-- ==================== 注册页面 ==================== -->
    <div v-if="currentPage === 'signup'" class="signup-page">
      <div class="container">
        <button class="back-btn" @click="currentPage = 'home'">← 返回首页</button>
      </div>
      <div class="form-container">
        <div class="form-card">
          <h1>Get Started for Free</h1>
          <p>Join ProductivityPro today and boost your productivity!</p>
          <form @submit.prevent="handleSubmit">
            <div class="form-group">
              <label>Full Name *</label>
              <input type="text" v-model="formData.name" placeholder="Enter your full name" required>
            </div>
            <div class="form-group">
              <label>Phone Number *</label>
              <input type="tel" v-model="formData.phone" placeholder="Enter your phone number" required>
            </div>
            <div class="form-group">
              <label>Email Address *</label>
              <input type="email" v-model="formData.email" placeholder="Enter your email address" required>
            </div>
            <div class="form-group">
              <label>Company Name (Optional)</label>
              <input type="text" v-model="formData.company" placeholder="Enter your company name">
            </div>
            <button type="submit" class="submit-btn">Start Free Trial →</button>
          </form>
          <p class="terms">By signing up, you agree to our <a href="#">Terms of Service</a> and <a href="#">Privacy Policy</a></p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, reactive } from 'vue'

const currentPage = ref('home')

const formData = reactive({
  name: '',
  phone: '',
  email: '',
  company: ''
})

const handleSubmit = () => {
  if (!formData.name || !formData.phone || !formData.email) {
    alert('请填写所有必填字段！')
    return
  }
  alert(`欢迎 ${formData.name}！\n我们已收到您的信息，稍后会有专员联系您。\n电话：${formData.phone}\n邮箱：${formData.email}`)
  formData.name = ''
  formData.phone = ''
  formData.email = ''
  formData.company = ''
  currentPage.value = 'home'
}
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen', sans-serif;
  color: #333;
  line-height: 1.6;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.app {
  background: linear-gradient(135deg, #e0f2fe 0%, #d1fae5 50%, #e0f2fe 100%);
  min-height: 100vh;
}

/* 导航栏 */
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  background: rgba(255, 255, 255, 0.95);
  backdrop-filter: blur(10px);
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
  z-index: 1000;
  padding: 1rem 0;
}

.nav-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
  background: linear-gradient(135deg, #3b82f6, #10b981);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
}

.nav-links {
  display: flex;
  gap: 2rem;
}

.nav-links a {
  text-decoration: none;
  color: #4b5563;
  font-weight: 500;
  transition: color 0.3s;
}

.nav-links a:hover {
  color: #3b82f6;
}

.btn-download {
  padding: 0.5rem 1.5rem;
  background: linear-gradient(135deg, #3b82f6, #10b981);
  color: white;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  font-weight: 500;
  transition: transform 0.3s;
}

.btn-download:hover {
  transform: translateY(-2px);
}

/* Hero 区域 */
.hero {
  padding: 120px 0 80px;
  background: linear-gradient(135deg, #3b82f6, #10b981);
  color: white;
  text-align: center;
}

.hero-content {
  max-width: 800px;
  margin: 0 auto;
}

.badge {
  display: inline-block;
  background: rgba(255,255,255,0.2);
  padding: 0.5rem 1rem;
  border-radius: 20px;
  font-size: 0.875rem;
  margin-bottom: 1.5rem;
}

.hero h1 {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.hero p {
  font-size: 1.125rem;
  margin-bottom: 2rem;
}

.btn-primary {
  padding: 1rem 2rem;
  background: white;
  color: #3b82f6;
  border: none;
  border-radius: 8px;
  font-size: 1rem;
  font-weight: 600;
  cursor: pointer;
  transition: transform 0.3s;
}

.btn-primary:hover {
  transform: translateY(-2px);
}

/* 功能区域 */
.features {
  padding: 80px 0;
  background: rgba(255, 255, 255, 0.5);
}

.section-title {
  text-align: center;
  font-size: 2rem;
  margin-bottom: 3rem;
  color: #1f2937;
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.feature-card {
  background: rgba(255, 255, 255, 0.9);
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  transition: transform 0.3s, box-shadow 0.3s;
  position: relative;
  overflow: hidden;
}

.feature-card:hover {
  transform: translateY(-5px);
  background: white;
  box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}

.feature-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
  position: relative;
  z-index: 1;
}

.feature-card h3 {
  margin-bottom: 1rem;
  color: #1f2937;
  position: relative;
  z-index: 1;
}

.feature-card ul {
  list-style: none;
  padding-left: 0;
  position: relative;
  z-index: 1;
}

.feature-card li {
  padding: 0.5rem 0;
  color: #4b5563;
  padding-left: 1.5rem;
  position: relative;
}

.feature-card li:before {
  content: "✓";
  color: #10b981;
  position: absolute;
  left: 0;
}

/* 功能卡片专属图案 */
.pattern-checklist {
  width: 80px;
  height: 80px;
  background: repeating-linear-gradient(45deg, #3b82f6 0px, #3b82f6 2px, transparent 2px, transparent 15px);
  right: -20px;
  top: -20px;
  border-radius: 50%;
}

.pattern-flow {
  width: 100px;
  height: 100px;
  background: radial-gradient(circle, #10b981 2px, transparent 2px);
  background-size: 18px 18px;
  left: -30px;
  bottom: -30px;
}

.pattern-clock {
  width: 70px;
  height: 70px;
  background: repeating-linear-gradient(135deg, #3b82f6 0px, #3b82f6 2px, transparent 2px, transparent 12px);
  right: 15px;
  top: 15px;
  border-radius: 50%;
}

.pattern-trend {
  width: 90px;
  height: 90px;
  background: repeating-linear-gradient(0deg, #10b981 0px, #10b981 1px, transparent 1px, transparent 20px);
  left: -20px;
  bottom: -20px;
  transform: rotate(-15deg);
}

.pattern-team {
  width: 80px;
  height: 80px;
  background: radial-gradient(circle, #3b82f6 1.5px, transparent 1.5px);
  background-size: 15px 15px;
  right: -25px;
  bottom: -25px;
}

.pattern-chat {
  width: 70px;
  height: 70px;
  background: repeating-linear-gradient(45deg, #10b981 0px, #10b981 1px, transparent 1px, transparent 10px);
  left: 15px;
  top: 15px;
  border-radius: 8px;
}

/* 目标区域 */
.goals, .goals-alt {
  padding: 80px 0;
}

.goals-alt {
  background: rgba(209, 250, 229, 0.6);
}

.goals-content h2 {
  text-align: center;
  font-size: 2rem;
  margin-bottom: 3rem;
  color: #1f2937;
}

.goals-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
}

.goal-item {
  background: rgba(255, 255, 255, 0.95);
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  cursor: pointer;
  position: relative;
  overflow: hidden;
}
··
.goal-item:hover {
  transform: scale(1.05);
  box-shadow: 0 8px 20px rgba(59,130,246,0.2);
  background: white;
}

.goal-item h3 {
  margin-bottom: 1rem;
  background: linear-gradient(135deg, #3b82f6, #10b981);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
  position: relative;
  z-index: 1;
}

.goal-item ul {
  list-style: none;
  padding-left: 0;
  position: relative;
  z-index: 1;
}

.goal-item li {
  padding: 0.5rem 0;
  color: #4b5563;
  padding-left: 1.5rem;
  position: relative;
}

.goal-item li:before {
  content: "→";
  color: #10b981;
  position: absolute;
  left: 0;
}

/* 通用背景图案样式 */
.bg-pattern {
  position: absolute;
  opacity: 0.12;
  pointer-events: none;
  z-index: 0;
  transition: opacity 0.3s;
}

.feature-card:hover .bg-pattern,
.goal-item:hover .bg-pattern,
.testimonial-card:hover .bg-pattern {
  opacity: 0.2;
}

/* 目标卡片图案 */
.pattern-target {
  width: 80px;
  height: 80px;
  background: radial-gradient(circle, #3b82f6 2px, transparent 2px);
  background-size: 15px 15px;
  right: -20px;
  bottom: -20px;
  border-radius: 50%;
}

.pattern-dots {
  width: 100px;
  height: 100px;
  background: radial-gradient(circle, #10b981 2px, transparent 2px);
  background-size: 20px 20px;
  left: -30px;
  top: -30px;
}

.pattern-chart {
  width: 70px;
  height: 70px;
  background: repeating-linear-gradient(45deg, #3b82f6 0px, #3b82f6 2px, transparent 2px, transparent 12px);
  right: 15px;
  top: 15px;
  border-radius: 8px;
}

.pattern-lines {
  width: 120px;
  height: 120px;
  background: repeating-linear-gradient(90deg, #10b981 0px, #10b981 1px, transparent 1px, transparent 15px);
  left: -40px;
  bottom: -40px;
  transform: rotate(15deg);
}

.pattern-star {
  width: 90px;
  height: 90px;
  background: repeating-linear-gradient(45deg, #fbbf24 0px, #fbbf24 2px, transparent 2px, transparent 20px);
  right: -20px;
  bottom: -20px;
  border-radius: 50%;
}

.pattern-wave {
  width: 100px;
  height: 100px;
  background: repeating-linear-gradient(45deg, #10b981 0px, #10b981 2px, transparent 2px, transparent 20px);
  left: -30px;
  top: -30px;
  border-radius: 50%;
}

.pattern-gear {
  width: 80px;
  height: 80px;
  background: repeating-linear-gradient(135deg, #3b82f6 0px, #3b82f6 2px, transparent 2px, transparent 15px);
  right: 10px;
  top: 10px;
  border-radius: 50%;
}

.pattern-grid {
  width: 100px;
  height: 100px;
  background: linear-gradient(90deg, #10b981 1px, transparent 1px) 0 0 / 20px 20px,
              linear-gradient(#10b981 1px, transparent 1px) 0 0 / 20px 20px;
  left: -30px;
  bottom: -30px;
}

/* 评价区域 */
.testimonials {
  padding: 80px 0;
  background: rgba(224, 242, 254, 0.6);
}

.testimonials-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 2rem;
}

.testimonial-card {
  background: rgba(255, 255, 255, 0.9);
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  transition: transform 0.3s;
  position: relative;
  overflow: hidden;
}

.testimonial-card:hover {
  transform: translateY(-5px);
  background: white;
}

.pattern-quote {
  width: 50px;
  height: 50px;
  right: 15px;
  top: 15px;
  color: #3b82f6;
}

.pattern-quote::before {
  content: "“";
  font-size: 60px;
  font-family: serif;
  position: absolute;
}

.pattern-heart {
  width: 40px;
  height: 40px;
  left: 15px;
  bottom: 15px;
  color: #10b981;
}

.pattern-heart::before {
  content: "❤";
  font-size: 40px;
  position: absolute;
}

.pattern-star-sm {
  width: 80px;
  height: 80px;
  right: 10px;
  bottom: 10px;
  background: repeating-linear-gradient(45deg, #fbbf24 0px, #fbbf24 2px, transparent 2px, transparent 15px);
  border-radius: 50%;
}

.pattern-bubble {
  width: 80px;
  height: 80px;
  left: -20px;
  top: -20px;
  background: radial-gradient(circle, #10b981 3px, transparent 3px);
  background-size: 20px 20px;
}

.pattern-sparkle {
  width: 60px;
  height: 60px;
  right: 20px;
  top: 20px;
  background: repeating-linear-gradient(45deg, #fbbf24 0px, #fbbf24 1px, transparent 1px, transparent 10px);
}

.pattern-crown {
  width: 50px;
  height: 50px;
  left: 20px;
  top: 20px;
  color: #fbbf24;
}

.pattern-crown::before {
  content: "👑";
  font-size: 40px;
  position: absolute;
}

.quote {
  font-size: 1rem;
  line-height: 1.6;
  color: #4b5563;
  margin-bottom: 1rem;
  font-style: italic;
  position: relative;
  z-index: 1;
}

.author {
  font-weight: 600;
  background: linear-gradient(135deg, #3b82f6, #10b981);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
  position: relative;
  z-index: 1;
}

/* CTA 区域 */
.cta {
  padding: 80px 0;
  background: linear-gradient(135deg, #3b82f6, #10b981);
  text-align: center;
}

.cta-content h2 {
  font-size: 2.5rem;
  margin-bottom: 1.5rem;
  color: white;
}

.btn-cta {
  padding: 1rem 2.5rem;
  background: white;
  color: #3b82f6;
  border: none;
  border-radius: 8px;
  font-size: 1.125rem;
  font-weight: 600;
  cursor: pointer;
  transition: transform 0.3s;
}

.btn-cta:hover {
  transform: translateY(-2px);
}

/* 页脚 */
.footer {
  background: rgba(31, 41, 55, 0.95);
  color: white;
  padding: 3rem 0 1rem;
}

.footer-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  margin-bottom: 2rem;
}

.footer-section h3 {
  margin-bottom: 1rem;
  font-size: 1.125rem;
  background: linear-gradient(135deg, #3b82f6, #10b981);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
}

.footer-section ul {
  list-style: none;
  padding: 0;
}

.footer-section li {
  margin-bottom: 0.5rem;
}

.footer-section a {
  color: #9ca3af;
  text-decoration: none;
  transition: color 0.3s;
}

.footer-section a:hover {
  color: #10b981;
}

.footer-bottom {
  text-align: center;
  padding-top: 2rem;
  border-top: 1px solid rgba(255,255,255,0.1);
  color: #9ca3af;
}

/* 注册页面 */
.signup-page {
  min-height: 100vh;
  background: linear-gradient(135deg, #e0f2fe 0%, #d1fae5 100%);
  padding: 2rem 0;
}

.back-btn {
  background: rgba(59,130,246,0.2);
  color: #3b82f6;
  border: 1px solid #3b82f6;
  padding: 0.5rem 1rem;
  border-radius: 6px;
  cursor: pointer;
  font-size: 0.9rem;
  transition: all 0.3s;
}

.back-btn:hover {
  background: #3b82f6;
  color: white;
}

.form-container {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: calc(100vh - 100px);
  padding: 2rem;
}

.form-card {
  background: rgba(255, 255, 255, 0.95);
  max-width: 500px;
  width: 100%;
  padding: 2.5rem;
  border-radius: 16px;
  box-shadow: 0 20px 40px rgba(0,0,0,0.1);
}

.form-card h1 {
  font-size: 2rem;
  background: linear-gradient(135deg, #3b82f6, #10b981);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
  margin-bottom: 0.5rem;
  text-align: center;
}

.form-card > p {
  text-align: center;
  color: #6b7280;
  margin-bottom: 2rem;
}

.form-group {
  margin-bottom: 1.5rem;
}

.form-group label {
  display: block;
  margin-bottom: 0.5rem;
  font-weight: 600;
  color: #374151;
}

.form-group input {
  width: 100%;
  padding: 0.75rem;
  border: 2px solid #e5e7eb;
  border-radius: 8px;
  font-size: 1rem;
  transition: border-color 0.3s;
}

.form-group input:focus {
  outline: none;
  border-color: #10b981;
}

.submit-btn {
  width: 100%;
  padding: 1rem;
  background: linear-gradient(135deg, #3b82f6, #10b981);
  color: white;
  border: none;
  border-radius: 8px;
  font-size: 1.125rem;
  font-weight: 600;
  cursor: pointer;
  transition: transform 0.2s;
}

.submit-btn:hover {
  transform: translateY(-2px);
}

.terms {
  margin-top: 1.5rem;
  text-align: center;
  font-size: 0.875rem;
  color: #6b7280;
}

.terms a {
  color: #10b981;
  text-decoration: none;
}

@media (max-width: 768px) {
  .nav-links {
    display: none;
  }
  .hero h1 {
    font-size: 2rem;
  }
  .section-title {
    font-size: 1.5rem;
  }
  .features-grid,
  .goals-list,
  .testimonials-grid {
    grid-template-columns: 1fr;
  }
  .footer-content {
    grid-template-columns: 1fr;
    text-align: center;
  }
  .form-card {
    padding: 1.5rem;
  }
  .form-card h1 {
    font-size: 1.5rem;
  }
}
</style>
