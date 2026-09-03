Here is the **complete, updated single-file HTML code** with your email `waqarhussain.dev12@gmail.com` updated across the site, the WhatsApp button in the navbar right beside "Get In Touch", and the full "Let's Build Something Great Together" section:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Waqar Hussain | Senior Full Stack .NET Developer</title>
  <meta name="description" content="Portfolio of Waqar Hussain - Senior Full Stack .NET Developer with 6+ years of experience specializing in ASP.NET Core 8, C#, SQL Server, Angular, and Healthcare/Enterprise ERP systems.">
  
  <!-- Google Fonts & Font Awesome Icons -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Fira+Code:wght@400;500;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

  <style>
    :root {
      --bg-primary: #0b0f19;
      --bg-secondary: #111827;
      --bg-card: rgba(17, 24, 39, 0.85);
      --bg-glass: rgba(255, 255, 255, 0.03);
      --border-color: rgba(255, 255, 255, 0.1);
      --accent-blue: #0078d4;
      --accent-cyan: #00d2ff;
      --accent-purple: #7928ca;
      --accent-whatsapp: #25D366;
      --text-main: #f3f4f6;
      --text-muted: #9ca3af;
      --text-dim: #6b7280;
      --gradient-accent: linear-gradient(135deg, #0078d4 0%, #00d2ff 100%);
      --radius-sm: 8px;
      --radius-md: 14px;
      --radius-lg: 20px;
      --shadow-glow: 0 0 25px rgba(0, 120, 212, 0.25);
      --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
      background-color: var(--bg-primary);
      color: var(--text-main);
      line-height: 1.6;
      overflow-x: hidden;
    }

    /* Ambient Background Glows */
    .glow-orb {
      position: fixed;
      width: 500px;
      height: 500px;
      border-radius: 50%;
      filter: blur(120px);
      z-index: -1;
      opacity: 0.2;
      pointer-events: none;
    }
    .glow-1 { top: -100px; left: -100px; background: var(--accent-blue); }
    .glow-2 { bottom: -100px; right: -100px; background: var(--accent-purple); }

    /* Layout Containers */
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 24px;
    }

    /* Header & Navigation */
    header {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      z-index: 1000;
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      background: rgba(11, 15, 25, 0.88);
      border-bottom: 1px solid var(--border-color);
      transition: var(--transition);
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 75px;
    }

    .logo {
      font-size: 1.35rem;
      font-weight: 800;
      color: #fff;
      text-decoration: none;
      display: flex;
      align-items: center;
      gap: 10px;
    }
    .logo span {
      background: var(--gradient-accent);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .nav-links {
      display: flex;
      gap: 18px;
      list-style: none;
      align-items: center;
    }

    .nav-links a {
      color: var(--text-muted);
      text-decoration: none;
      font-size: 0.95rem;
      font-weight: 500;
      transition: var(--transition);
      display: inline-flex;
      align-items: center;
    }
    .nav-links a:hover {
      color: var(--accent-cyan);
    }

    .social-icon-link {
      padding: 6px;
      border-radius: 6px;
      color: var(--text-muted);
    }
    .social-icon-link:hover {
      color: #fff;
      background: rgba(255, 255, 255, 0.08);
    }

    /* WhatsApp Button in Navigation (Near Get In Touch) */
    .nav-whatsapp-btn {
      display: inline-flex !important;
      align-items: center;
      gap: 7px;
      background: rgba(37, 211, 102, 0.15) !important;
      border: 1px solid rgba(37, 211, 102, 0.4);
      color: #25D366 !important;
      font-weight: 600;
      font-size: 0.88rem;
      padding: 8px 14px;
      border-radius: var(--radius-sm);
      transition: var(--transition);
    }
    .nav-whatsapp-btn:hover {
      background: #25D366 !important;
      color: #fff !important;
      transform: translateY(-2px);
      box-shadow: 0 4px 15px rgba(37, 211, 102, 0.4);
    }

    .nav-cta {
      padding: 9px 20px;
      border-radius: var(--radius-sm);
      background: var(--gradient-accent);
      color: #fff !important;
      font-weight: 600;
      text-decoration: none;
      transition: var(--transition);
      box-shadow: 0 4px 15px rgba(0, 120, 212, 0.3);
    }
    .nav-cta:hover {
      transform: translateY(-2px);
      box-shadow: 0 6px 20px rgba(0, 210, 255, 0.4);
    }

    .menu-toggle {
      display: none;
      background: none;
      border: none;
      color: var(--text-main);
      font-size: 1.5rem;
      cursor: pointer;
    }

    /* Hero Section */
    .hero {
      min-height: 100vh;
      display: flex;
      align-items: center;
      padding-top: 100px;
      position: relative;
    }

    .hero-content {
      display: grid;
      grid-template-columns: 1.2fr 0.8fr;
      gap: 60px;
      align-items: center;
    }

    .badge-experience {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 6px 16px;
      border-radius: 50px;
      background: rgba(0, 120, 212, 0.15);
      border: 1px solid rgba(0, 210, 255, 0.3);
      color: var(--accent-cyan);
      font-size: 0.85rem;
      font-weight: 600;
      margin-bottom: 20px;
    }

    .hero-title {
      font-size: 3.5rem;
      font-weight: 800;
      line-height: 1.15;
      margin-bottom: 16px;
      letter-spacing: -0.02em;
    }
    .hero-title .highlight {
      background: var(--gradient-accent);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .typing-container {
      font-family: 'Fira Code', monospace;
      font-size: 1.25rem;
      color: var(--accent-cyan);
      margin-bottom: 20px;
      min-height: 32px;
    }

    .hero-desc {
      font-size: 1.1rem;
      color: var(--text-muted);
      margin-bottom: 35px;
      max-width: 580px;
    }

    .hero-actions {
      display: flex;
      gap: 16px;
      flex-wrap: wrap;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      padding: 14px 26px;
      border-radius: var(--radius-sm);
      font-size: 1rem;
      font-weight: 600;
      text-decoration: none;
      cursor: pointer;
      transition: var(--transition);
      border: none;
    }
    .btn-primary {
      background: var(--gradient-accent);
      color: #fff;
      box-shadow: 0 4px 20px rgba(0, 120, 212, 0.35);
    }
    .btn-primary:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 25px rgba(0, 210, 255, 0.5);
    }
    .btn-whatsapp {
      background: #25D366;
      color: #fff;
      box-shadow: 0 4px 20px rgba(37, 211, 102, 0.3);
    }
    .btn-whatsapp:hover {
      background: #20ba5a;
      transform: translateY(-3px);
      box-shadow: 0 8px 25px rgba(37, 211, 102, 0.5);
    }

    .hero-card-visual {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-lg);
      padding: 30px;
      backdrop-filter: blur(20px);
      position: relative;
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4);
    }
    .hero-card-header {
      display: flex;
      align-items: center;
      gap: 8px;
      margin-bottom: 20px;
      padding-bottom: 15px;
      border-bottom: 1px solid var(--border-color);
    }
    .dot { width: 12px; height: 12px; border-radius: 50%; }
    .dot.red { background: #ff5f56; }
    .dot.yellow { background: #ffbd2e; }
    .dot.green { background: #27c93f; }
    
    .code-preview {
      font-family: 'Fira Code', monospace;
      font-size: 0.85rem;
      color: #a5b4fc;
      line-height: 1.6;
    }
    .code-keyword { color: #f472b6; }
    .code-func { color: #60a5fa; }
    .code-string { color: #34d399; }
    .code-comment { color: var(--text-dim); }

    /* Stats Banner */
    .stats-bar {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
      padding: 35px;
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-md);
      margin: 40px 0 100px;
    }
    .stat-item {
      text-align: center;
    }
    .stat-number {
      font-size: 2.3rem;
      font-weight: 800;
      color: #fff;
      background: var(--gradient-accent);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      margin-bottom: 4px;
    }
    .stat-label {
      font-size: 0.9rem;
      color: var(--text-muted);
    }

    /* Section Styles */
    section {
      padding: 80px 0;
    }

    .section-header {
      text-align: center;
      max-width: 650px;
      margin: 0 auto 60px;
    }
    .section-tag {
      font-size: 0.85rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 2px;
      color: var(--accent-cyan);
      margin-bottom: 12px;
      display: block;
    }
    .section-title {
      font-size: 2.4rem;
      font-weight: 800;
      color: #fff;
      margin-bottom: 16px;
    }
    .section-subtitle {
      font-size: 1.05rem;
      color: var(--text-muted);
    }

    /* Enterprise Domain Projects */
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
      gap: 30px;
    }

    .project-card {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-md);
      padding: 32px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      transition: var(--transition);
      position: relative;
      overflow: hidden;
    }
    .project-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 4px;
      background: var(--gradient-accent);
      opacity: 0;
      transition: var(--transition);
    }
    .project-card:hover {
      transform: translateY(-6px);
      border-color: rgba(0, 210, 255, 0.4);
      box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4);
    }
    .project-card:hover::before {
      opacity: 1;
    }

    .project-flagship-badge {
      position: absolute;
      top: 20px;
      right: 20px;
      background: rgba(0, 120, 212, 0.2);
      border: 1px solid rgba(0, 210, 255, 0.4);
      color: var(--accent-cyan);
      padding: 4px 12px;
      border-radius: 50px;
      font-size: 0.75rem;
      font-weight: 700;
      text-transform: uppercase;
    }

    .project-icon {
      font-size: 2.2rem;
      color: var(--accent-cyan);
      margin-bottom: 20px;
    }

    .project-title {
      font-size: 1.35rem;
      font-weight: 700;
      color: #fff;
      margin-bottom: 12px;
    }

    .project-desc {
      font-size: 0.95rem;
      color: var(--text-muted);
      margin-bottom: 20px;
      line-height: 1.6;
    }

    .project-features {
      list-style: none;
      margin-bottom: 24px;
    }
    .project-features li {
      font-size: 0.85rem;
      color: #d1d5db;
      margin-bottom: 8px;
      display: flex;
      align-items: center;
      gap: 8px;
    }
    .project-features li i {
      color: #34d399;
      font-size: 0.75rem;
    }

    .project-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-bottom: 20px;
    }
    .tag {
      font-size: 0.75rem;
      font-weight: 600;
      padding: 4px 10px;
      border-radius: 4px;
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid rgba(255, 255, 255, 0.08);
      color: #93c5fd;
    }

    .project-links {
      display: flex;
      gap: 15px;
    }
    .project-link {
      font-size: 0.88rem;
      font-weight: 600;
      color: var(--accent-cyan);
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      transition: var(--transition);
    }
    .project-link:hover {
      color: #fff;
      transform: translateX(3px);
    }

    /* Skills Grid */
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 24px;
    }

    .skill-card {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-md);
      padding: 28px;
      transition: var(--transition);
    }
    .skill-card:hover {
      border-color: rgba(0, 120, 212, 0.4);
      transform: translateY(-4px);
    }

    .skill-header {
      display: flex;
      align-items: center;
      gap: 14px;
      margin-bottom: 20px;
    }
    .skill-icon-wrapper {
      width: 46px;
      height: 46px;
      border-radius: 10px;
      background: rgba(0, 120, 212, 0.15);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.4rem;
      color: var(--accent-cyan);
    }
    .skill-title {
      font-size: 1.1rem;
      font-weight: 700;
      color: #fff;
    }

    .skill-pill-list {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
    }
    .skill-pill {
      font-size: 0.82rem;
      padding: 6px 12px;
      border-radius: 6px;
      background: rgba(255, 255, 255, 0.04);
      border: 1px solid var(--border-color);
      color: var(--text-main);
    }

    /* Experience / About Section */
    .about-box {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-lg);
      padding: 45px;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 50px;
      align-items: center;
    }
    .about-text h3 {
      font-size: 1.8rem;
      font-weight: 800;
      margin-bottom: 18px;
      color: #fff;
    }
    .about-text p {
      color: var(--text-muted);
      margin-bottom: 16px;
      font-size: 1.02rem;
    }

    .info-list {
      list-style: none;
      margin-top: 24px;
    }
    .info-list li {
      display: flex;
      align-items: center;
      gap: 12px;
      margin-bottom: 12px;
      font-size: 0.95rem;
      color: #d1d5db;
    }
    .info-list li i {
      color: var(--accent-cyan);
      width: 20px;
    }

    .experience-timeline {
      border-left: 2px solid var(--border-color);
      padding-left: 25px;
      position: relative;
    }
    .timeline-item {
      position: relative;
      margin-bottom: 30px;
    }
    .timeline-item:last-child {
      margin-bottom: 0;
    }
    .timeline-dot {
      position: absolute;
      left: -32px;
      top: 4px;
      width: 12px;
      height: 12px;
      border-radius: 50%;
      background: var(--accent-cyan);
      box-shadow: 0 0 10px var(--accent-cyan);
    }
    .timeline-period {
      font-size: 0.8rem;
      color: var(--accent-cyan);
      font-weight: 600;
      text-transform: uppercase;
      margin-bottom: 4px;
    }
    .timeline-role {
      font-size: 1.15rem;
      font-weight: 700;
      color: #fff;
    }
    .timeline-company {
      font-size: 0.95rem;
      color: var(--text-muted);
      margin-bottom: 8px;
    }

    /* "Let's Build Something Great Together" Banner */
    .cta-banner-card {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-lg);
      padding: 50px 40px;
      text-align: center;
      max-width: 900px;
      margin: 0 auto;
      box-shadow: 0 0 35px rgba(0, 120, 212, 0.2);
    }
    .cta-title {
      font-size: 2.2rem;
      font-weight: 800;
      color: #fff;
      margin-bottom: 16px;
    }
    .cta-desc {
      color: var(--text-muted);
      font-size: 1.05rem;
      max-width: 650px;
      margin: 0 auto 30px;
    }
    .cta-email-badge {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid var(--border-color);
      padding: 10px 22px;
      border-radius: 50px;
      margin-bottom: 30px;
      color: #fff;
      font-size: 0.98rem;
    }
    .cta-email-badge a {
      color: var(--accent-cyan);
      text-decoration: none;
      font-weight: 600;
    }
    .cta-email-badge a:hover {
      text-decoration: underline;
    }
    .cta-buttons {
      display: flex;
      justify-content: center;
      gap: 15px;
      flex-wrap: wrap;
    }
    .cta-btn-email {
      background: var(--gradient-accent);
      color: #fff;
      padding: 12px 24px;
      border-radius: var(--radius-sm);
      font-weight: 600;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: var(--transition);
      box-shadow: 0 4px 15px rgba(0, 120, 212, 0.35);
    }
    .cta-btn-email:hover {
      transform: translateY(-2px);
      box-shadow: 0 6px 20px rgba(0, 210, 255, 0.5);
    }
    .cta-btn-whatsapp {
      background: #25D366;
      color: #fff;
      padding: 12px 24px;
      border-radius: var(--radius-sm);
      font-weight: 600;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: var(--transition);
      box-shadow: 0 4px 15px rgba(37, 211, 102, 0.35);
    }
    .cta-btn-whatsapp:hover {
      background: #20ba5a;
      transform: translateY(-2px);
      box-shadow: 0 6px 20px rgba(37, 211, 102, 0.5);
    }
    .cta-btn-linkedin {
      background: #0077B5;
      color: #fff;
      padding: 12px 24px;
      border-radius: var(--radius-sm);
      font-weight: 600;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: var(--transition);
    }
    .cta-btn-linkedin:hover {
      transform: translateY(-2px);
      box-shadow: 0 6px 20px rgba(0, 119, 181, 0.4);
    }
    .cta-btn-github {
      background: rgba(255, 255, 255, 0.08);
      color: #fff;
      border: 1px solid var(--border-color);
      padding: 12px 24px;
      border-radius: var(--radius-sm);
      font-weight: 600;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: var(--transition);
    }
    .cta-btn-github:hover {
      background: rgba(255, 255, 255, 0.15);
      transform: translateY(-2px);
    }

    /* Interactive Contact Form Section */
    .contact-wrapper {
      display: grid;
      grid-template-columns: 1fr 1.3fr;
      gap: 40px;
      align-items: start;
    }

    .contact-info-card {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-lg);
      padding: 40px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    .contact-info-header h3 {
      font-size: 1.8rem;
      font-weight: 800;
      color: #fff;
      margin-bottom: 12px;
    }
    .contact-info-header p {
      color: var(--text-muted);
      margin-bottom: 30px;
      font-size: 1rem;
    }

    .direct-links {
      display: flex;
      flex-direction: column;
      gap: 16px;
      margin-bottom: 30px;
    }

    .direct-item {
      display: flex;
      align-items: center;
      gap: 16px;
      text-decoration: none;
      color: var(--text-main);
      padding: 14px 18px;
      border-radius: var(--radius-md);
      background: rgba(255, 255, 255, 0.03);
      border: 1px solid var(--border-color);
      transition: var(--transition);
    }
    .direct-item:hover {
      background: rgba(0, 120, 212, 0.15);
      border-color: var(--accent-cyan);
      transform: translateX(5px);
    }
    .direct-item.whatsapp-item:hover {
      background: rgba(37, 211, 102, 0.15);
      border-color: #25D366;
    }
    .direct-icon {
      width: 42px;
      height: 42px;
      border-radius: 10px;
      background: rgba(0, 210, 255, 0.1);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.25rem;
      color: var(--accent-cyan);
    }
    .direct-icon.whatsapp {
      background: rgba(37, 211, 102, 0.15);
      color: #25D366;
    }
    .direct-label {
      font-size: 0.8rem;
      color: var(--text-dim);
    }
    .direct-value {
      font-size: 0.95rem;
      font-weight: 600;
      color: #fff;
    }

    .contact-form-card {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-lg);
      padding: 40px;
      box-shadow: var(--shadow-glow);
    }

    .form-group {
      margin-bottom: 22px;
    }
    .form-row {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
    }

    .form-label {
      display: block;
      font-size: 0.88rem;
      font-weight: 600;
      color: #d1d5db;
      margin-bottom: 8px;
    }

    .form-control {
      width: 100%;
      padding: 14px 18px;
      background: rgba(255, 255, 255, 0.04);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-sm);
      color: #fff;
      font-family: inherit;
      font-size: 0.95rem;
      transition: var(--transition);
    }
    .form-control:focus {
      outline: none;
      border-color: var(--accent-cyan);
      background: rgba(255, 255, 255, 0.07);
      box-shadow: 0 0 15px rgba(0, 210, 255, 0.25);
    }

    textarea.form-control {
      resize: vertical;
      min-height: 120px;
    }

    .form-submit-btn {
      width: 100%;
      padding: 16px;
      border-radius: var(--radius-sm);
      background: var(--gradient-accent);
      color: #fff;
      font-size: 1.05rem;
      font-weight: 700;
      border: none;
      cursor: pointer;
      transition: var(--transition);
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      box-shadow: 0 4px 20px rgba(0, 120, 212, 0.35);
    }
    .form-submit-btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 25px rgba(0, 210, 255, 0.5);
    }

    .form-status {
      display: none;
      margin-top: 18px;
      padding: 14px;
      border-radius: var(--radius-sm);
      font-size: 0.92rem;
      text-align: center;
    }
    .form-status.success {
      display: block;
      background: rgba(39, 201, 63, 0.15);
      border: 1px solid rgba(39, 201, 63, 0.4);
      color: #34d399;
    }

    /* Floating WhatsApp Button */
    .floating-whatsapp {
      position: fixed;
      bottom: 30px;
      right: 30px;
      width: 60px;
      height: 60px;
      border-radius: 50%;
      background: #25D366;
      color: #fff;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 6px 20px rgba(37, 211, 102, 0.45);
      text-decoration: none;
      z-index: 999;
      transition: var(--transition);
      animation: pulseWhatsApp 2.5s infinite;
    }
    .floating-whatsapp:hover {
      transform: scale(1.12);
      box-shadow: 0 8px 30px rgba(37, 211, 102, 0.65);
    }

    @keyframes pulseWhatsApp {
      0% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0.6); }
      70% { box-shadow: 0 0 0 16px rgba(37, 211, 102, 0); }
      100% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0); }
    }

    /* Footer */
    footer {
      border-top: 1px solid var(--border-color);
      padding: 35px 0;
      text-align: center;
      color: var(--text-dim);
      font-size: 0.9rem;
      margin-top: 80px;
    }

    /* Responsive */
    @media (max-width: 900px) {
      .hero-content { grid-template-columns: 1fr; gap: 40px; text-align: center; }
      .hero-desc { margin-left: auto; margin-right: auto; }
      .hero-actions { justify-content: center; }
      .stats-bar { grid-template-columns: 1fr 1fr; gap: 25px; }
      .about-box { grid-template-columns: 1fr; gap: 35px; }
      .contact-wrapper { grid-template-columns: 1fr; }
      .form-row { grid-template-columns: 1fr; }
      .hero-title { font-size: 2.7rem; }
    }
    @media (max-width: 820px) {
      .nav-links {
        display: none;
        position: absolute;
        top: 75px;
        left: 0;
        width: 100%;
        background: rgba(11, 15, 25, 0.97);
        flex-direction: column;
        padding: 24px;
        border-bottom: 1px solid var(--border-color);
        gap: 18px;
      }
      .nav-links.active {
        display: flex;
      }
      .menu-toggle { display: block; }
      .hero-title { font-size: 2.2rem; }
      .stats-bar { grid-template-columns: 1fr; }
      .floating-whatsapp { bottom: 20px; right: 20px; width: 52px; height: 52px; }
    }
  </style>
</head>
<body>

  <!-- Ambient Glow Backgrounds -->
  <div class="glow-orb glow-1"></div>
  <div class="glow-orb glow-2"></div>

  <!-- Floating WhatsApp Quick-Chat Button -->
  <a href="https://wa.me/923044576934?text=Hi%20Waqar%2C%20I%20visited%20your%20portfolio%20and%20would%20like%20to%20discuss%20a%20project!" target="_blank" class="floating-whatsapp" title="Chat on WhatsApp">
    <svg width="34" height="34" viewBox="0 0 24 24" fill="#ffffff"><path d="M12.04 2c-5.46 0-9.91 4.45-9.91 9.91 0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91 0-2.65-1.03-5.14-2.9-7.01A9.816 9.816 0 0 0 12.04 2m.01 1.67c2.2 0 4.26.86 5.82 2.42a8.225 8.225 0 0 1 2.41 5.83c0 4.54-3.7 8.24-8.24 8.24-1.48 0-2.93-.4-4.2-1.15l-.3-.18-3.12.82.83-3.04-.2-.31a8.19 8.19 0 0 1-1.26-4.38c0-4.54 3.7-8.24 8.24-8.24M8.53 7.33c-.2-.43-.4-.44-.59-.45l-.5-.01c-.17 0-.45.07-.69.32-.24.26-.91.89-.91 2.17s.93 2.52 1.06 2.69c.13.17 1.81 2.89 4.46 3.94 2.21.87 2.66.7 3.14.65.48-.04 1.55-.63 1.77-1.25.22-.61.22-1.13.15-1.25-.07-.11-.25-.18-.53-.32s-1.55-.77-1.79-.86c-.24-.09-.41-.13-.59.13-.18.26-.69.86-.84 1.04-.16.17-.32.2-.6.06-.27-.13-1.16-.43-2.2-1.36-.82-.72-1.37-1.62-1.53-1.89-.16-.27-.02-.42.12-.56.13-.12.28-.32.42-.48.14-.16.19-.27.28-.45.09-.18.05-.34-.02-.48-.08-.14-.59-1.48-.82-2.02Z"/></svg>
  </a>

  <!-- Sticky Navigation Bar -->
  <header>
    <div class="container">
      <nav>
        <a href="#home" class="logo">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#00d2ff" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="16 18 22 12 16 6"></polyline><polyline points="8 6 2 12 8 18"></polyline></svg>
          <span>Waqar Hussain</span>
        </a>
        <ul class="nav-links" id="navLinks">
          <li><a href="#about">About</a></li>
          <li><a href="#skills">Tech Stack</a></li>
          <li><a href="#projects">Projects & Domains</a></li>
          <li><a href="#experience">Experience</a></li>
          
          <!-- LinkedIn -->
          <li>
            <a href="https://linkedin.com/in/waqarhussain786" target="_blank" title="LinkedIn" class="social-icon-link">
              <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M19 3a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h14m-.5 15.5v-5.3a3.26 3.26 0 0 0-3.26-3.26c-.85 0-1.84.52-2.28 1.3v-1.11h-2.79v8.37h2.79v-4.93c0-.77.62-1.4 1.39-1.4a1.4 1.4 0 0 1 1.4 1.4v4.93h2.75M6.46 10.9v8.37H9.2V10.9H6.46M7.83 6.45a1.64 1.64 0 1 0 0 3.28 1.64 1.64 0 0 0 0-3.28Z"/></svg>
            </a>
          </li>

          <!-- GitHub -->
          <li>
            <a href="https://github.com/waqarrasheed4444" target="_blank" title="GitHub" class="social-icon-link">
              <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34-.46-1.16-1.11-1.47-1.11-1.47-.91-.62.07-.6.07-.6 1 .07 1.53 1.03 1.53 1.03.87 1.52 2.34 1.07 2.91.83.1-.65.35-1.09.63-1.34-2.22-.25-4.55-1.11-4.55-4.92 0-1.11.38-2 1.03-2.71-.1-.25-.45-1.29.1-2.64 0 0 .84-.27 2.75 1.02.79-.22 1.65-.33 2.5-.33.85 0 1.71.11 2.5.33 1.91-1.29 2.75-1.02 2.75-1.02.55 1.35.2 2.39.1 2.64.65.71 1.03 1.6 1.03 2.71 0 3.82-2.34 4.66-4.57 4.91.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2Z"/></svg>
            </a>
          </li>

          <!-- WhatsApp Button Directly Before 'Get In Touch' -->
          <li>
            <a href="https://wa.me/923044576934?text=Hi%20Waqar%2C%20I%20visited%20your%20portfolio%20and%20would%20like%20to%20discuss%20a%20project!" target="_blank" class="nav-whatsapp-btn" title="Chat on WhatsApp">
              <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12.04 2c-5.46 0-9.91 4.45-9.91 9.91 0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91 0-2.65-1.03-5.14-2.9-7.01A9.816 9.816 0 0 0 12.04 2m.01 1.67c2.2 0 4.26.86 5.82 2.42a8.225 8.225 0 0 1 2.41 5.83c0 4.54-3.7 8.24-8.24 8.24-1.48 0-2.93-.4-4.2-1.15l-.3-.18-3.12.82.83-3.04-.2-.31a8.19 8.19 0 0 1-1.26-4.38c0-4.54 3.7-8.24 8.24-8.24M8.53 7.33c-.2-.43-.4-.44-.59-.45l-.5-.01c-.17 0-.45.07-.69.32-.24.26-.91.89-.91 2.17s.93 2.52 1.06 2.69c.13.17 1.81 2.89 4.46 3.94 2.21.87 2.66.7 3.14.65.48-.04 1.55-.63 1.77-1.25.22-.61.22-1.13.15-1.25-.07-.11-.25-.18-.53-.32s-1.55-.77-1.79-.86c-.24-.09-.41-.13-.59.13-.18.26-.69.86-.84 1.04-.16.17-.32.2-.6.06-.27-.13-1.16-.43-2.2-1.36-.82-.72-1.37-1.62-1.53-1.89-.16-.27-.02-.42.12-.56.13-.12.28-.32.42-.48.14-.16.19-.27.28-.45.09-.18.05-.34-.02-.48-.08-.14-.59-1.48-.82-2.02Z"/></svg>
              <span>WhatsApp</span>
            </a>
          </li>

          <!-- Get In Touch CTA -->
          <li><a href="#contact" class="nav-cta">Get In Touch</a></li>
        </ul>
        <button class="menu-toggle" id="menuToggle" aria-label="Toggle Menu">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="3" y1="12" x2="21" y2="12"></line><line x1="3" y1="6" x2="21" y2="6"></line><line x1="3" y1="18" x2="21" y2="18"></line></svg>
        </button>
      </nav>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="hero" id="home">
    <div class="container">
      <div class="hero-content">
        <div class="hero-text">
          <div class="badge-experience">
            <i class="fa-solid fa-award"></i> 6+ Years Industry Experience
          </div>
          <h1 class="hero-title">
            Hi, I'm <span class="highlight">Waqar Hussain</span>
          </h1>
          <div class="typing-container">
            <span id="typed-text"></span>
          </div>
          <p class="hero-desc">
            Senior Full Stack .NET Developer specializing in enterprise-grade <strong>ASP.NET Core 8 Web APIs</strong>, <strong>SQL Server</strong>, <strong>JWT Authentication & Security</strong>, and <strong>Angular</strong> architectures.
          </p>
          <div class="hero-actions">
            <a href="#projects" class="btn btn-primary">
              <i class="fa-solid fa-rocket"></i> View Enterprise Projects
            </a>
            <a href="https://wa.me/923044576934?text=Hi%20Waqar%2C%20I%20visited%20your%20portfolio%20and%20would%20like%20to%20discuss%20a%20project!" target="_blank" class="btn btn-whatsapp">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M12.04 2c-5.46 0-9.91 4.45-9.91 9.91 0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91 0-2.65-1.03-5.14-2.9-7.01A9.816 9.816 0 0 0 12.04 2m.01 1.67c2.2 0 4.26.86 5.82 2.42a8.225 8.225 0 0 1 2.41 5.83c0 4.54-3.7 8.24-8.24 8.24-1.48 0-2.93-.4-4.2-1.15l-.3-.18-3.12.82.83-3.04-.2-.31a8.19 8.19 0 0 1-1.26-4.38c0-4.54 3.7-8.24 8.24-8.24M8.53 7.33c-.2-.43-.4-.44-.59-.45l-.5-.01c-.17 0-.45.07-.69.32-.24.26-.91.89-.91 2.17s.93 2.52 1.06 2.69c.13.17 1.81 2.89 4.46 3.94 2.21.87 2.66.7 3.14.65.48-.04 1.55-.63 1.77-1.25.22-.61.22-1.13.15-1.25-.07-.11-.25-.18-.53-.32s-1.55-.77-1.79-.86c-.24-.09-.41-.13-.59.13-.18.26-.69.86-.84 1.04-.16.17-.32.2-.6.06-.27-.13-1.16-.43-2.2-1.36-.82-.72-1.37-1.62-1.53-1.89-.16-.27-.02-.42.12-.56.13-.12.28-.32.42-.48.14-.16.19-.27.28-.45.09-.18.05-.34-.02-.48-.08-.14-.59-1.48-.82-2.02Z"/></svg>
              <span>Chat on WhatsApp</span>
            </a>
          </div>
        </div>

        <div class="hero-card-visual">
          <div class="hero-card-header">
            <div class="dot red"></div>
            <div class="dot yellow"></div>
            <div class="dot green"></div>
            <span style="margin-left: 10px; font-size: 0.8rem; color: var(--text-dim);">ApplicationDbContext.cs</span>
          </div>
          <div class="code-preview">
            <span class="code-comment">// Architecting scalable .NET 8 Backends</span><br>
            <span class="code-keyword">public class</span> <span class="code-func">MediCoreContext</span> : <span class="code-func">DbContext</span><br>
            {<br>
            &nbsp;&nbsp;<span class="code-keyword">public</span> <span class="code-func">DbSet</span>&lt;<span class="code-func">PatientRecord</span>&gt; Patients { <span class="code-keyword">get; set;</span> }<br>
            &nbsp;&nbsp;<span class="code-keyword">public</span> <span class="code-func">DbSet</span>&lt;<span class="code-func">DoctorConsultation</span>&gt; Consultations { <span class="code-keyword">get; set;</span> }<br>
            &nbsp;&nbsp;<span class="code-keyword">public</span> <span class="code-func">DbSet</span>&lt;<span class="code-func">PharmacyPrescription</span>&gt; Prescriptions { <span class="code-keyword">get; set;</span> }<br>
            &nbsp;&nbsp;<span class="code-keyword">public</span> <span class="code-func">DbSet</span>&lt;<span class="code-func">TaskItem</span>&gt; Tasks { <span class="code-keyword">get; set;</span> }<br><br>
            &nbsp;&nbsp;<span class="code-comment">// Fluent API Mappings & Cascade Rules</span><br>
            &nbsp;&nbsp;<span class="code-keyword">protected override void</span> <span class="code-func">OnModelCreating</span>(...) { ... }<br>
            }
          </div>
        </div>
      </div>

      <!-- Stats Bar -->
      <div class="stats-bar">
        <div class="stat-item">
          <div class="stat-number">6+</div>
          <div class="stat-label">Years Experience</div>
        </div>
        <div class="stat-item">
          <div class="stat-number">15+</div>
          <div class="stat-label">Enterprise Solutions</div>
        </div>
        <div class="stat-item">
          <div class="stat-number">100%</div>
          <div class="stat-label">Client Satisfaction</div>
        </div>
        <div class="stat-item">
          <div class="stat-number">99.9%</div>
          <div class="stat-label">Uptime & Reliability</div>
        </div>
      </div>
    </div>
  </section>

  <!-- Featured Projects & Enterprise Domains -->
  <section id="projects">
    <div class="container">
      <div class="section-header">
        <span class="section-tag">Portfolio & Solutions</span>
        <h2 class="section-title">Enterprise Systems & Projects</h2>
        <p class="section-subtitle">Real-world enterprise platforms engineered across Healthcare, Retail, Fleet Logistics, and Core ERP domains.</p>
      </div>

      <div class="projects-grid">

        <!-- Project 1: MediCore Healthcare System -->
        <div class="project-card">
          <span class="project-flagship-badge">Flagship Project</span>
          <div>
            <div class="project-icon"><i class="fa-solid fa-hospital-user"></i></div>
            <h3 class="project-title">MediCore Healthcare ERP</h3>
            <p class="project-desc">Complete Hospital Management & Healthcare Platform designed for clinical governance, patient life cycles, and diagnostic workflows.</p>
            <ul class="project-features">
              <li><i class="fa-solid fa-check"></i> EMR/EHR electronic medical records</li>
              <li><i class="fa-solid fa-check"></i> Doctor scheduling & consultation queues</li>
              <li><i class="fa-solid fa-check"></i> Pharmacy inventory & prescription fulfillment</li>
              <li><i class="fa-solid fa-check"></i> Lab pathology test tracking & medical billing</li>
            </ul>
          </div>
          <div>
            <div class="project-tags">
              <span class="tag">ASP.NET Core</span>
              <span class="tag">SQL Server</span>
              <span class="tag">Angular</span>
              <span class="tag">EF Core</span>
              <span class="tag">JWT / RBAC</span>
            </div>
            <div class="project-links">
              <span class="project-link" style="color: #9ca3af;"><i class="fa-solid fa-shield-halved"></i> Enterprise Platform</span>
            </div>
          </div>
        </div>

        <!-- Project 2: PaperSource Retail Integration -->
        <div class="project-card">
          <div>
            <div class="project-icon"><i class="fa-solid fa-store"></i></div>
            <h3 class="project-title">PaperSource Retail Integration</h3>
            <p class="project-desc">Automated multi-channel retail platform synchronizing store inventory, product catalogs, order processing, and payment pipelines.</p>
            <ul class="project-features">
              <li><i class="fa-solid fa-check"></i> Multi-channel real-time inventory sync</li>
              <li><i class="fa-solid fa-check"></i> Automated product catalog pipelines</li>
              <li><i class="fa-solid fa-check"></i> Payment gateway & invoice integrations</li>
            </ul>
          </div>
          <div>
            <div class="project-tags">
              <span class="tag">ASP.NET Core</span>
              <span class="tag">REST APIs</span>
              <span class="tag">JavaScript</span>
              <span class="tag">SQL Server</span>
            </div>
            <div class="project-links">
              <a href="https://github.com/waqarrasheed4444/Papersource-Integration" target="_blank" class="project-link">
                <i class="fa-brands fa-github"></i> View Repository <i class="fa-solid fa-arrow-right"></i>
              </a>
            </div>
          </div>
        </div>

        <!-- Project 3: Fleet Management System -->
        <div class="project-card">
          <div>
            <div class="project-icon"><i class="fa-solid fa-truck-fast"></i></div>
            <h3 class="project-title">Fleet & Logistics Management</h3>
            <p class="project-desc">Logistics & vehicle dispatch system providing real-time fleet tracking, preventive maintenance schedules, driver management, and route planning.</p>
            <ul class="project-features">
              <li><i class="fa-solid fa-check"></i> Vehicle tracking & route optimization</li>
              <li><i class="fa-solid fa-check"></i> Automated maintenance schedules</li>
              <li><i class="fa-solid fa-check"></i> Driver dispatch & fuel tracking</li>
            </ul>
          </div>
          <div>
            <div class="project-tags">
              <span class="tag">C# / .NET</span>
              <span class="tag">ASP.NET Core</span>
              <span class="tag">SQL Server</span>
              <span class="tag">Angular</span>
            </div>
            <div class="project-links">
              <span class="project-link" style="color: #9ca3af;"><i class="fa-solid fa-truck"></i> Logistics Core</span>
            </div>
          </div>
        </div>

        <!-- Project 4: Enterprise CMS & ERP -->
        <div class="project-card">
          <div>
            <div class="project-icon"><i class="fa-solid fa-cubes"></i></div>
            <h3 class="project-title">Enterprise CMS & ERP System</h3>
            <p class="project-desc">Comprehensive Enterprise Resource Planning system automating financial ledger tracking, multi-role approval workflows, and content delivery.</p>
            <ul class="project-features">
              <li><i class="fa-solid fa-check"></i> Business process automation & workflows</li>
              <li><i class="fa-solid fa-check"></i> Multi-tier role permissions & audit logs</li>
              <li><i class="fa-solid fa-check"></i> Financial reports & inventory modules</li>
            </ul>
          </div>
          <div>
            <div class="project-tags">
              <span class="tag">ASP.NET Core</span>
              <span class="tag">Angular</span>
              <span class="tag">SQL Server</span>
              <span class="tag">Clean Architecture</span>
            </div>
            <div class="project-links">
              <a href="https://github.com/waqarrasheed4444/CMSMANAGMENT" target="_blank" class="project-link">
                <i class="fa-brands fa-github"></i> View Repository <i class="fa-solid fa-arrow-right"></i>
              </a>
            </div>
          </div>
        </div>

        <!-- Project 5: Task Manager Web API (.NET 8) -->
        <div class="project-card">
          <div>
            <div class="project-icon"><i class="fa-solid fa-list-check"></i></div>
            <h3 class="project-title">Task Manager Web API (.NET 8)</h3>
            <p class="project-desc">Production-grade ASP.NET Core 8 Web API with JWT Authentication, cryptographic Refresh Token rotation, Task CRUD, and Swagger documentation.</p>
            <ul class="project-features">
              <li><i class="fa-solid fa-check"></i> JWT Access Token & Refresh Token rotation</li>
              <li><i class="fa-solid fa-check"></i> Strict user data isolation (403 Forbidden)</li>
              <li><i class="fa-solid fa-check"></i> 18/18 integration automated tests passing</li>
            </ul>
          </div>
          <div>
            <div class="project-tags">
              <span class="tag">.NET 8</span>
              <span class="tag">EF Core 8</span>
              <span class="tag">SQL Server</span>
              <span class="tag">JWT Bearer</span>
              <span class="tag">Swagger</span>
            </div>
            <div class="project-links">
              <a href="https://github.com/waqarrasheed4444/task-manager-api-net8" target="_blank" class="project-link">
                <i class="fa-brands fa-github"></i> View Repository <i class="fa-solid fa-arrow-right"></i>
              </a>
            </div>
          </div>
        </div>

        <!-- Project 6: Clean Architecture API -->
        <div class="project-card">
          <div>
            <div class="project-icon"><i class="fa-solid fa-layer-group"></i></div>
            <h3 class="project-title">dotnet-clean-architecture-api</h3>
            <p class="project-desc">Demonstration of Clean Architecture & Domain-Driven Design principles using ASP.NET Core, repository pattern, CQRS, and dependency injection.</p>
            <ul class="project-features">
              <li><i class="fa-solid fa-check"></i> Decoupled domain & persistence layers</li>
              <li><i class="fa-solid fa-check"></i> Repository & Unit of Work patterns</li>
              <li><i class="fa-solid fa-check"></i> Centralized exception interception</li>
            </ul>
          </div>
          <div>
            <div class="project-tags">
              <span class="tag">C#</span>
              <span class="tag">.NET 8</span>
              <span class="tag">Clean Architecture</span>
              <span class="tag">SOLID</span>
            </div>
            <div class="project-links">
              <a href="https://github.com/waqarrasheed4444/dotnet-clean-architecture-api" target="_blank" class="project-link">
                <i class="fa-brands fa-github"></i> View Repository <i class="fa-solid fa-arrow-right"></i>
              </a>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- Technical Skills Matrix -->
  <section id="skills" style="background: rgba(17, 24, 39, 0.4);">
    <div class="container">
      <div class="section-header">
        <span class="section-tag">Technical Competencies</span>
        <h2 class="section-title">Skills & Technologies</h2>
        <p class="section-subtitle">A comprehensive toolkit honed over 6+ years of building enterprise software.</p>
      </div>

      <div class="skills-grid">
        <!-- Backend -->
        <div class="skill-card">
          <div class="skill-header">
            <div class="skill-icon-wrapper"><i class="fa-solid fa-server"></i></div>
            <h3 class="skill-title">Backend & Core</h3>
          </div>
          <div class="skill-pill-list">
            <span class="skill-pill">C# 12</span>
            <span class="skill-pill">.NET 8.0</span>
            <span class="skill-pill">ASP.NET Core Web API</span>
            <span class="skill-pill">Minimal APIs</span>
            <span class="skill-pill">LINQ</span>
            <span class="skill-pill">RESTful Architecture</span>
          </div>
        </div>

        <!-- Database & ORM -->
        <div class="skill-card">
          <div class="skill-header">
            <div class="skill-icon-wrapper"><i class="fa-solid fa-database"></i></div>
            <h3 class="skill-title">Database & ORM</h3>
          </div>
          <div class="skill-pill-list">
            <span class="skill-pill">Microsoft SQL Server</span>
            <span class="skill-pill">Entity Framework Core 8</span>
            <span class="skill-pill">Code-First Migrations</span>
            <span class="skill-pill">Fluent API</span>
            <span class="skill-pill">Query Optimization</span>
            <span class="skill-pill">SSMS</span>
          </div>
        </div>

        <!-- Security & Auth -->
        <div class="skill-card">
          <div class="skill-header">
            <div class="skill-icon-wrapper"><i class="fa-solid fa-lock"></i></div>
            <h3 class="skill-title">Security & Auth</h3>
          </div>
          <div class="skill-pill-list">
            <span class="skill-pill">JWT Bearer Tokens</span>
            <span class="skill-pill">Refresh Token Rotation</span>
            <span class="skill-pill">Role-Based Access Control</span>
            <span class="skill-pill">BCrypt Password Hashing</span>
            <span class="skill-pill">Claims-Based Identity</span>
            <span class="skill-pill">HIPAA Data Safety</span>
          </div>
        </div>

        <!-- Frontend -->
        <div class="skill-card">
          <div class="skill-header">
            <div class="skill-icon-wrapper"><i class="fa-brands fa-angular"></i></div>
            <h3 class="skill-title">Frontend & Web</h3>
          </div>
          <div class="skill-pill-list">
            <span class="skill-pill">Angular</span>
            <span class="skill-pill">TypeScript</span>
            <span class="skill-pill">JavaScript (ES6+)</span>
            <span class="skill-pill">RxJS</span>
            <span class="skill-pill">HTML5 & CSS3</span>
            <span class="skill-pill">Responsive Design</span>
          </div>
        </div>

        <!-- Architecture -->
        <div class="skill-card">
          <div class="skill-header">
            <div class="skill-icon-wrapper"><i class="fa-solid fa-sitemap"></i></div>
            <h3 class="skill-title">Architecture</h3>
          </div>
          <div class="skill-pill-list">
            <span class="skill-pill">Clean Architecture</span>
            <span class="skill-pill">SOLID Principles</span>
            <span class="skill-pill">Repository Pattern</span>
            <span class="skill-pill">Global Exception Handlers</span>
            <span class="skill-pill">DTO / ViewModel Mapping</span>
          </div>
        </div>

        <!-- DevOps & Tools -->
        <div class="skill-card">
          <div class="skill-header">
            <div class="skill-icon-wrapper"><i class="fa-solid fa-screwdriver-wrench"></i></div>
            <h3 class="skill-title">DevOps & Tools</h3>
          </div>
          <div class="skill-pill-list">
            <span class="skill-pill">Visual Studio 2022</span>
            <span class="skill-pill">VS Code</span>
            <span class="skill-pill">Git & GitHub</span>
            <span class="skill-pill">Postman / Swagger</span>
            <span class="skill-pill">Docker Containers</span>
            <span class="skill-pill">Microsoft Azure</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- About & Experience Section -->
  <section id="experience">
    <div class="container">
      <div class="about-box">
        <div class="about-text">
          <span class="section-tag">Career & Background</span>
          <h3>Engineering Robust, Scalable Backend Systems</h3>
          <p>
            With over <strong>6+ years of specialized experience</strong>, I focus on solving complex business challenges by building robust backend services and seamless web interfaces.
          </p>
          <p>
            Whether designing high-volume retail synchronizers, healthcare EMR architectures, or secure financial modules, I ensure every system is maintainable, performant, and secure.
          </p>
          <ul class="info-list">
            <li><i class="fa-solid fa-location-dot"></i> Lahore, Pakistan</li>
            <li><i class="fa-solid fa-building"></i> Senior Full Stack Engineer @ Berks Technologies</li>
            <li><i class="fa-solid fa-envelope"></i> Open to enterprise consulting & contracts</li>
          </ul>
        </div>

        <div class="experience-timeline">
          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <div class="timeline-period">Present (6+ Years Experience)</div>
            <div class="timeline-role">Senior Full Stack .NET Developer</div>
            <div class="timeline-company">Berks Technologies</div>
            <p style="font-size: 0.9rem; color: var(--text-muted);">
              Lead architect for enterprise Healthcare (MediCore), Retail (PaperSource), Fleet Management, and custom ERP/CMS platforms. Specializing in ASP.NET Core 8 Web APIs and SQL Server.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- "Let's Build Something Great Together" Banner Section -->
  <section id="connect-banner">
    <div class="container">
      <div class="cta-banner-card">
        <h2 class="cta-title">Let's Build Something Great Together</h2>
        <p class="cta-desc">
          Looking for a Senior .NET Developer to architect your Web API, build a high-performance backend, or engineer a full-stack solution? Let's connect!
        </p>

        <!-- Direct Email Pill Badge -->
        <div class="cta-email-badge">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#00d2ff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
          Direct Email: <a href="mailto:waqarhussain.dev12@gmail.com">waqarhussain.dev12@gmail.com</a>
        </div>

        <!-- Action Buttons -->
        <div class="cta-buttons">
          <!-- Email Button -->
          <a href="mailto:waqarhussain.dev12@gmail.com?subject=Project%20Inquiry%20from%20Portfolio" class="cta-btn-email">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
            Send Email
          </a>

          <!-- WhatsApp Button -->
          <a href="https://wa.me/923044576934?text=Hi%20Waqar%2C%20I%20visited%20your%20portfolio%20and%20would%20like%20to%20discuss%20a%20project!" target="_blank" class="cta-btn-whatsapp">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12.04 2c-5.46 0-9.91 4.45-9.91 9.91 0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91 0-2.65-1.03-5.14-2.9-7.01A9.816 9.816 0 0 0 12.04 2m.01 1.67c2.2 0 4.26.86 5.82 2.42a8.225 8.225 0 0 1 2.41 5.83c0 4.54-3.7 8.24-8.24 8.24-1.48 0-2.93-.4-4.2-1.15l-.3-.18-3.12.82.83-3.04-.2-.31a8.19 8.19 0 0 1-1.26-4.38c0-4.54 3.7-8.24 8.24-8.24M8.53 7.33c-.2-.43-.4-.44-.59-.45l-.5-.01c-.17 0-.45.07-.69.32-.24.26-.91.89-.91 2.17s.93 2.52 1.06 2.69c.13.17 1.81 2.89 4.46 3.94 2.21.87 2.66.7 3.14.65.48-.04 1.55-.63 1.77-1.25.22-.61.22-1.13.15-1.25-.07-.11-.25-.18-.53-.32s-1.55-.77-1.79-.86c-.24-.09-.41-.13-.59.13-.18.26-.69.86-.84 1.04-.16.17-.32.2-.6.06-.27-.13-1.16-.43-2.2-1.36-.82-.72-1.37-1.62-1.53-1.89-.16-.27-.02-.42.12-.56.13-.12.28-.32.42-.48.14-.16.19-.27.28-.45.09-.18.05-.34-.02-.48-.08-.14-.59-1.48-.82-2.02Z"/></svg>
            WhatsApp
          </a>

          <!-- LinkedIn Button -->
          <a href="https://linkedin.com/in/waqarhussain786" target="_blank" class="cta-btn-linkedin">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M19 3a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h14m-.5 15.5v-5.3a3.26 3.26 0 0 0-3.26-3.26c-.85 0-1.84.52-2.28 1.3v-1.11h-2.79v8.37h2.79v-4.93c0-.77.62-1.4 1.39-1.4a1.4 1.4 0 0 1 1.4 1.4v4.93h2.75M6.46 10.9v8.37H9.2V10.9H6.46M7.83 6.45a1.64 1.64 0 1 0 0 3.28 1.64 1.64 0 0 0 0-3.28Z"/></svg>
            Connect on LinkedIn
          </a>

          <!-- GitHub Button -->
          <a href="https://github.com/waqarrasheed4444" target="_blank" class="cta-btn-github">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34-.46-1.16-1.11-1.47-1.11-1.47-.91-.62.07-.6.07-.6 1 .07 1.53 1.03 1.53 1.03.87 1.52 2.34 1.07 2.91.83.1-.65.35-1.09.63-1.34-2.22-.25-4.55-1.11-4.55-4.92 0-1.11.38-2 1.03-2.71-.1-.25-.45-1.29.1-2.64 0 0 .84-.27 2.75 1.02.79-.22 1.65-.33 2.5-.33.85 0 1.71.11 2.5.33 1.91-1.29 2.75-1.02 2.75-1.02.55 1.35.2 2.39.1 2.64.65.71 1.03 1.6 1.03 2.71 0 3.82-2.34 4.66-4.57 4.91.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2Z"/></svg>
            Explore GitHub
          </a>
        </div>
      </div>
    </div>
  </section>

  <!-- Interactive Contact Form Section -->
  <section id="contact">
    <div class="container">
      <div class="section-header">
        <span class="section-tag">Get In Touch</span>
        <h2 class="section-title">Start a Project or Consultation</h2>
        <p class="section-subtitle">Have an enterprise project, .NET backend requirement, or architecture consulting need? Send a message directly.</p>
      </div>

      <div class="contact-wrapper">
        <!-- Direct Contact Cards -->
        <div class="contact-info-card">
          <div class="contact-info-header">
            <h3>Let's Connect</h3>
            <p>I'm available for full-stack .NET contracts, architecture design, and enterprise software consulting.</p>
          </div>

          <div class="direct-links">
            <a href="https://wa.me/923044576934?text=Hi%20Waqar%2C%20I%20visited%20your%20portfolio%20and%20would%20like%20to%20discuss%20a%20project!" target="_blank" class="direct-item whatsapp-item">
              <div class="direct-icon whatsapp">
                <svg width="22" height="22" viewBox="0 0 24 24" fill="currentColor"><path d="M12.04 2c-5.46 0-9.91 4.45-9.91 9.91 0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91 0-2.65-1.03-5.14-2.9-7.01A9.816 9.816 0 0 0 12.04 2m.01 1.67c2.2 0 4.26.86 5.82 2.42a8.225 8.225 0 0 1 2.41 5.83c0 4.54-3.7 8.24-8.24 8.24-1.48 0-2.93-.4-4.2-1.15l-.3-.18-3.12.82.83-3.04-.2-.31a8.19 8.19 0 0 1-1.26-4.38c0-4.54 3.7-8.24 8.24-8.24M8.53 7.33c-.2-.43-.4-.44-.59-.45l-.5-.01c-.17 0-.45.07-.69.32-.24.26-.91.89-.91 2.17s.93 2.52 1.06 2.69c.13.17 1.81 2.89 4.46 3.94 2.21.87 2.66.7 3.14.65.48-.04 1.55-.63 1.77-1.25.22-.61.22-1.13.15-1.25-.07-.11-.25-.18-.53-.32s-1.55-.77-1.79-.86c-.24-.09-.41-.13-.59.13-.18.26-.69.86-.84 1.04-.16.17-.32.2-.6.06-.27-.13-1.16-.43-2.2-1.36-.82-.72-1.37-1.62-1.53-1.89-.16-.27-.02-.42.12-.56.13-.12.28-.32.42-.48.14-.16.19-.27.28-.45.09-.18.05-.34-.02-.48-.08-.14-.59-1.48-.82-2.02Z"/></svg>
              </div>
              <div>
                <div class="direct-label">WhatsApp (Direct Chat)</div>
                <div class="direct-value">+92 304 4576934</div>
              </div>
            </a>

            <!-- Direct Email Link -->
            <a href="mailto:waqarhussain.dev12@gmail.com?subject=Enterprise%20Consultation" class="direct-item">
              <div class="direct-icon">
                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#00d2ff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
              </div>
              <div>
                <div class="direct-label">Direct Email</div>
                <div class="direct-value">waqarhussain.dev12@gmail.com</div>
              </div>
            </a>

            <a href="https://linkedin.com/in/waqarhussain786" target="_blank" class="direct-item">
              <div class="direct-icon">
                <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M19 3a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h14m-.5 15.5v-5.3a3.26 3.26 0 0 0-3.26-3.26c-.85 0-1.84.52-2.28 1.3v-1.11h-2.79v8.37h2.79v-4.93c0-.77.62-1.4 1.39-1.4a1.4 1.4 0 0 1 1.4 1.4v4.93h2.75M6.46 10.9v8.37H9.2V10.9H6.46M7.83 6.45a1.64 1.64 0 1 0 0 3.28 1.64 1.64 0 0 0 0-3.28Z"/></svg>
              </div>
              <div>
                <div class="direct-label">LinkedIn Profile</div>
                <div class="direct-value">in/waqarhussain786</div>
              </div>
            </a>

            <a href="https://github.com/waqarrasheed4444" target="_blank" class="direct-item">
              <div class="direct-icon">
                <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34-.46-1.16-1.11-1.47-1.11-1.47-.91-.62.07-.6.07-.6 1 .07 1.53 1.03 1.53 1.03.87 1.52 2.34 1.07 2.91.83.1-.65.35-1.09.63-1.34-2.22-.25-4.55-1.11-4.55-4.92 0-1.11.38-2 1.03-2.71-.1-.25-.45-1.29.1-2.64 0 0 .84-.27 2.75 1.02.79-.22 1.65-.33 2.5-.33.85 0 1.71.11 2.5.33 1.91-1.29 2.75-1.02 2.75-1.02.55 1.35.2 2.39.1 2.64.65.71 1.03 1.6 1.03 2.71 0 3.82-2.34 4.66-4.57 4.91.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2Z"/></svg>
              </div>
              <div>
                <div class="direct-label">GitHub Profile</div>
                <div class="direct-value">waqarrasheed4444</div>
              </div>
            </a>

            <div class="direct-item">
              <div class="direct-icon">
                <i class="fa-solid fa-location-dot"></i>
              </div>
              <div>
                <div class="direct-label">Location</div>
                <div class="direct-value">Lahore, Pakistan (PKT / UTC+5)</div>
              </div>
            </div>
          </div>

          <div style="font-size: 0.88rem; color: var(--text-dim);">
            <i class="fa-solid fa-bolt" style="color: #ffbd2e; margin-right: 6px;"></i> Average response time: Under 24 hours
          </div>
        </div>

        <!-- Interactive Contact Form -->
        <div class="contact-form-card">
          <form id="portfolioContactForm" onsubmit="handleFormSubmit(event)">
            <div class="form-row">
              <div class="form-group">
                <label class="form-label" for="senderName">Your Name *</label>
                <input type="text" id="senderName" class="form-control" placeholder="John Doe" required>
              </div>
              <div class="form-group">
                <label class="form-label" for="senderEmail">Your Email *</label>
                <input type="email" id="senderEmail" class="form-control" placeholder="john@example.com" required>
              </div>
            </div>

            <div class="form-group">
              <label class="form-label" for="projectType">Service / Project Type</label>
              <select id="projectType" class="form-control" style="background: #1a2234;">
                <option value="ASP.NET Core 8 Web API Backend">ASP.NET Core 8 Web API & REST Backend</option>
                <option value="Healthcare ERP / MediCore Platform">Healthcare / Medical ERP Solution</option>
                <option value="Full Stack Angular & .NET App">Full Stack App (Angular + .NET Core)</option>
                <option value="SQL Server & Database Optimization">SQL Server Database & Query Tuning</option>
                <option value="Architecture Review & Clean Code Consultation">Architecture Review & Clean Code Consultation</option>
                <option value="Other Inquiries">Other Inquiries</option>
              </select>
            </div>

            <div class="form-group">
              <label class="form-label" for="senderMessage">Project Details / Message *</label>
              <textarea id="senderMessage" class="form-control" placeholder="Tell me about your project scope, timeline, and requirements..." required></textarea>
            </div>

            <button type="submit" class="form-submit-btn" id="submitBtn">
              <i class="fa-solid fa-paper-plane"></i> Send Message
            </button>

            <div class="form-status success" id="formStatus">
              <i class="fa-solid fa-circle-check"></i> Thank you! Your message has been prepared. Opening your email client to send...
            </div>
          </form>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container">
      <p>© 2026 Waqar Hussain. Senior Full Stack .NET Developer. Built with precision & modern web standards.</p>
    </div>
  </footer>

  <!-- Interactive Scripts -->
  <script>
    // Typing animation
    const phrases = [
      "Senior Full Stack .NET Developer",
      "ASP.NET Core 8 Web API Specialist",
      "MediCore Healthcare ERP Architect",
      "JWT Security & SQL Server Expert",
      "Angular & Full Stack Engineer"
    ];
    let phraseIndex = 0;
    let charIndex = 0;
    let isDeleting = false;
    const typedTextSpan = document.getElementById("typed-text");

    function typeEffect() {
      const currentPhrase = phrases[phraseIndex];
      if (isDeleting) {
        typedTextSpan.textContent = currentPhrase.substring(0, charIndex - 1);
        charIndex--;
      } else {
        typedTextSpan.textContent = currentPhrase.substring(0, charIndex + 1);
        charIndex++;
      }

      let typeSpeed = isDeleting ? 40 : 80;

      if (!isDeleting && charIndex === currentPhrase.length) {
        typeSpeed = 1800;
        isDeleting = true;
      } else if (isDeleting && charIndex === 0) {
        isDeleting = false;
        phraseIndex = (phraseIndex + 1) % phrases.length;
        typeSpeed = 300;
      }

      setTimeout(typeEffect, typeSpeed);
    }

    // Mobile Navbar Toggle
    const menuToggle = document.getElementById('menuToggle');
    const navLinks = document.getElementById('navLinks');
    if (menuToggle && navLinks) {
      menuToggle.addEventListener('click', () => {
        navLinks.classList.toggle('active');
      });
      navLinks.querySelectorAll('a').forEach(link => {
        link.addEventListener('click', () => {
          navLinks.classList.remove('active');
        });
      });
    }

    // Form Submission Handler with waqarhussain.dev12@gmail.com
    function handleFormSubmit(e) {
      e.preventDefault();
      const name = document.getElementById('senderName').value;
      const email = document.getElementById('senderEmail').value;
      const type = document.getElementById('projectType').value;
      const message = document.getElementById('senderMessage').value;
      const statusDiv = document.getElementById('formStatus');
      const submitBtn = document.getElementById('submitBtn');

      submitBtn.innerHTML = '<i class="fa-solid fa-spinner fa-spin"></i> Processing...';
      
      setTimeout(() => {
        statusDiv.style.display = 'block';
        submitBtn.innerHTML = '<i class="fa-solid fa-check"></i> Sent!';
        
        // Trigger mailto link to waqarhussain.dev12@gmail.com
        const subject = encodeURIComponent(`[Project Inquiry: ${type}] from ${name}`);
        const body = encodeURIComponent(`Hi Waqar,\n\nName: ${name}\nEmail: ${email}\nProject Type: ${type}\n\nMessage:\n${message}`);
        window.location.href = `mailto:waqarhussain.dev12@gmail.com?subject=${subject}&body=${body}`;

        setTimeout(() => {
          submitBtn.innerHTML = '<i class="fa-solid fa-paper-plane"></i> Send Another Message';
        }, 3000);
      }, 600);
    }

    document.addEventListener("DOMContentLoaded", () => {
      setTimeout(typeEffect, 400);
    });
  </script>
</body>
</html>
```
