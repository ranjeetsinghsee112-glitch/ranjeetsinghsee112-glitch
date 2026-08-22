<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ranjeet Kumar Singh | Azure DevOps Engineer & Cloud Architect</title>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Fira+Code:wght@400;600&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --bg-color: #0b0f19;
            --card-bg: rgba(17, 24, 39, 0.7);
            --card-border: rgba(255, 255, 255, 0.08);
            --text-main: #f3f4f6;
            --text-muted: #9ca3af;
            --accent-blue: #0078d4;
            --accent-cyan: #00b4d8;
            --accent-purple: #844fba;
            --accent-glow: rgba(0, 120, 212, 0.25);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
            overflow-x: hidden;
            background-image: 
                radial-gradient(circle at 10% 20%, rgba(0, 120, 212, 0.08) 0%, transparent 40%),
                radial-gradient(circle at 90% 80%, rgba(132, 79, 186, 0.08) 0%, transparent 40%);
            background-attachment: fixed;
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        /* Header Section */
        header {
            text-align: center;
            padding: 50px 20px;
            background: var(--card-bg);
            border: 1px solid var(--card-border);
            border-radius: 20px;
            backdrop-filter: blur(12px);
            margin-bottom: 40px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
        }

        header h1 {
            font-size: 2.5rem;
            font-weight: 800;
            margin-bottom: 15px;
            background: linear-gradient(135deg, #fff 30%, var(--accent-cyan));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .badges-row {
            display: flex;
            justify-content: center;
            gap: 12px;
            margin: 20px 0;
            flex-wrap: wrap;
        }

        .badges-row img {
            height: 28px;
            /* Animated Logo Effect */
            transition: transform 0.3s ease, filter 0.3s ease;
        }
        .badges-row img:hover {
            transform: translateY(-4px) scale(1.05);
            filter: drop-shadow(0 5px 10px var(--accent-glow));
        }

        .tagline {
            font-size: 1.2rem;
            color: var(--text-muted);
            font-weight: 500;
            margin-top: 10px;
        }

        /* Section Styling */
        section {
            background: var(--card-bg);
            border: 1px solid var(--card-border);
            border-radius: 16px;
            padding: 35px;
            margin-bottom: 30px;
            backdrop-filter: blur(10px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.3);
            transition: border-color 0.3s ease;
        }

        section:hover {
            border-color: rgba(0, 120, 212, 0.3);
        }

        h2 {
            font-size: 1.6rem;
            margin-bottom: 25px;
            display: flex;
            align-items: center;
            gap: 12px;
            color: #fff;
            border-bottom: 1px solid var(--card-border);
            padding-bottom: 12px;
        }

        /* About Grid */
        .about-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 15px;
            list-style: none;
        }

        .about-grid li {
            background: rgba(255, 255, 255, 0.02);
            border: 1px solid var(--card-border);
            padding: 15px 20px;
            border-radius: 10px;
            font-size: 0.95krem;
            color: var(--text-muted);
            display: flex;
            align-items: center;
            gap: 12px;
            transition: all 0.3s ease;
        }

        .about-grid li:hover {
            background: rgba(255, 255, 255, 0.05);
            color: var(--text-main);
            transform: translateX(5px);
        }

        /* Skill Icons Grid */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
            gap: 20px;
            text-align: center;
        }

        .skill-card {
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid var(--card-border);
            padding: 20px 10px;
            border-radius: 12px;
            transition: all 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        .skill-card img {
            width: 45px;
            height: 45px;
            margin-bottom: 10px;
            transition: transform 0.3s ease;
        }

        .skill-card:hover {
            transform: translateY(-8px);
            background: rgba(0, 120, 212, 0.08);
            border-color: var(--accent-blue);
            box-shadow: 0 10px 20px var(--accent-glow);
        }

        .skill-card:hover img {
            transform: scale(1.15) rotate(5deg);
        }

        .skill-card b {
            font-size: 0.85rem;
            color: var(--text-main);
            display: block;
        }

        /* Tags Container */
        .tags-container {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 15px;
        }

        .tag {
            background: rgba(0, 120, 212, 0.1);
            color: var(--accent-cyan);
            border: 1px solid rgba(0, 120, 212, 0.2);
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-family: 'Fira Code', monospace;
            transition: all 0.3s ease;
        }

        .tag:hover {
            background: var(--accent-blue);
            color: #fff;
            transform: scale(1.05);
        }

        /* Table Styling */
        .custom-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
            overflow: hidden;
            border-radius: 10px;
            border: 1px solid var(--card-border);
        }

        .custom-table th, .custom-table td {
            padding: 14px 18px;
            text-align: left;
            border-bottom: 1px solid var(--card-border);
        }

        .custom-table th {
            background: rgba(255, 255, 255, 0.05);
            color: #fff;
            font-weight: 600;
        }

        .custom-table tr:hover {
            background: rgba(255, 255, 255, 0.02);
        }

        /* Marquee Effect for Tech Lists / Sub-stacks */
        .marquee-wrapper {
            overflow: hidden;
            white-space: nowrap;
            width: 100%;
            margin: 15px 0;
            position: relative;
        }

        .marquee-content {
            display: inline-block;
            animation: marquee 25s linear infinite;
        }

        .marquee-content span {
            display: inline-block;
            background: rgba(255, 255, 255, 0.04);
            border: 1px solid var(--card-border);
            padding: 8px 16px;
            border-radius: 8px;
            margin-right: 10px;
            font-family: 'Fira Code', monospace;
            font-size: 0.85rem;
            color: var(--text-muted);
        }

        @keyframes marquee {
            0% { transform: translateX(0); }
            100% { transform: translateX(-50%); }
        }

        /* Project & Code Block */
        .featured-box {
            background: linear-gradient(145deg, rgba(132, 79, 186, 0.05), rgba(0, 120, 212, 0.05));
            border: 1px solid rgba(132, 79, 186, 0.2);
            border-radius: 14px;
            padding: 25px;
        }

        .code-block {
            background: #05070b;
            border: 1px solid var(--card-border);
            border-radius: 10px;
            padding: 20px;
            font-family: 'Fira Code', monospace;
            font-size: 0.85rem;
            color: #34d399;
            white-space: pre-wrap;
            line-height: 1.7;
        }

        /* Activity & Connect */
        .activity-box {
            text-align: center;
        }

        .activity-box img {
            max-width: 100%;
            border-radius: 10px;
            filter: invert(0.85) hue-rotate(180deg);
        }

        .connect-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin-top: 20px;
        }

        .btn-connect {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 12px 24px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.95rem;
            transition: all 0.3s ease;
            border: 1px solid transparent;
        }

        .btn-linkedin { background: #0a66c2; color: #fff; }
        .btn-gmail { background: #d14836; color: #fff; }
        .btn-github { background: #181717; color: #fff; border-color: var(--card-border); }

        .btn-connect:hover {
            transform: translateY(-4px);
            filter: brightness(1.1);
            box-shadow: 0 8px 20px rgba(0,0,0,0.4);
        }

        footer {
            text-align: center;
            padding: 30px;
            color: var(--text-muted);
            font-size: 0.9rem;
            border-top: 1px solid var(--card-border);
            margin-top: 40px;
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- Header Section -->
        <header>
            <h1>👋 Hi, I'm Ranjeet Kumar Singh</h1>
            <p class="tagline">🚀 Azure DevOps Engineer | Cloud Infrastructure | Kubernetes | Terraform</p>
            <div class="badges-row">
                <img src="https://komarev.com/ghpvc/?username=ranjeet-112&label=Profile%20Views&color=0e75b6&style=flat" alt="Profile Views" />
                <img src="https://img.shields.io/github/followers/ranjeet-112?label=Followers&style=flat" alt="GitHub Followers" />
            </div>
            <p style="color: var(--text-muted); font-weight: 600; margin-top: 10px;">☁️ Building Scalable • Secure • Automated Cloud Infrastructure</p>
        </header>

        <!-- About Me Section -->
        <section>
            <h2><i class="fa-solid fa-user-astronaut"></i> About Me</h2>
            <ul class="about-grid">
                <li><i class="fa-solid fa-briefcase" style="color:var(--accent-cyan)"></i> <strong>10+ years</strong> of IT experience (6+ years in Azure)</li>
                <li><i class="fa-solid fa-cloud" style="color:var(--accent-blue)"></i> Specialized in Azure Cloud Infrastructure & DevOps</li>
                <li><i class="fa-solid fa-file-code" style="color:var(--accent-purple)"></i> IaC expert using Terraform</li>
                <li><i class="fa-solid fa-dharmachakra" style="color:#326ce5"></i> Working with Kubernetes, AKS, Helm & Argo CD</li>
                <li><i class="fa-solid fa-rotate" style="color:#2088ff"></i> Optimizing CI/CD with Azure DevOps & GitHub Actions</li>
                <li><i class="fa-solid fa-shield-halved" style="color:#34d399"></i> Implementing DevSecOps (SonarQube, Trivy, Checkov)</li>
                <li><i class="fa-solid fa-chart-line" style="color:#f46800"></i> Observability via Prometheus, Grafana & Azure Monitor</li>
                <li><i class="fa-solid fa-key" style="color:#ffd700"></i> Identity & Access Management (Entra ID, RBAC, OIDC)</li>
                <li><i class="fa-solid fa-brain" style="color:#ec4899"></i> Exploring AI-assisted DevOps automation & LLM workflows</li>
                <li><i class="fa-solid fa-envelope" style="color:#d14836"></i> <strong>Email:</strong> ranjeetsee112@gmail.com</li>
                <li><i class="fa-solid fa-location-dot" style="color:#ef7b4d"></i> <strong>Location:</strong> Jharkhand, India</li>
            </ul>
        </section>

        <!-- Core DevOps & Cloud Skills -->
        <section>
            <h2><i class="fa-solid fa-toolbox"></i> Core DevOps & Cloud Skills</h2>
            <div class="skills-grid">
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=azure" alt="Azure"/><b>Azure</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=terraform" alt="Terraform"/><b>Terraform</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=docker" alt="Docker"/><b>Docker</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=kubernetes" alt="Kubernetes"/><b>Kubernetes</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=helm" alt="Helm"/><b>Helm</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=git" alt="Git"/><b>Git</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=github" alt="GitHub"/><b>GitHub</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=jenkins" alt="Jenkins"/><b>Jenkins</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=python" alt="Python"/><b>Python</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=bash" alt="Bash"/><b>Bash</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=prometheus" alt="Prometheus"/><b>Prometheus</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=grafana" alt="Grafana"/><b>Grafana</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=javascript" alt="JavaScript"/><b>JavaScript</b></div>
                <div class="skill-card"><img src="https://skillicons.dev/icons?i=html" alt="HTML5"/><b>HTML5</b></div>
            </div>
        </section>

        <!-- Cloud Platforms -->
        <section>
            <h2><i class="fa-solid fa-cloud-arrow-up"></i> Cloud Platforms</h2>
            <div style="display: flex; gap: 15px; margin-bottom: 20px;">
                <img src="https://img.shields.io/badge/Microsoft%20Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" alt="Azure" style="border-radius:6px;">
                <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS" style="border-radius:6px;">
            </div>
            <h3 style="font-size: 1.1rem; color: #fff; margin-bottom: 10px;">Azure Ecosystem Expertise</h3>
            <div class="marquee-wrapper">
                <div class="marquee-content">
                    <span>Azure VNet</span><span>Subnets</span><span>NSG</span><span>Route Tables</span><span>VNet Peering</span><span>Private Endpoints</span><span>Load Balancer</span><span>Application Gateway/WAF</span><span>AKS</span><span>ACR</span><span>Azure Monitor</span><span>Log Analytics</span><span>Application Insights</span><span>Key Vault</span><span>Entra ID</span><span>RBAC</span><span>Managed Identity</span><span>Azure Policy</span>
                    <!-- Duplicate for infinite smooth loop effect -->
                    <span>Azure VNet</span><span>Subnets</span><span>NSG</span><span>Route Tables</span><span>VNet Peering</span><span>Private Endpoints</span><span>Load Balancer</span><span>Application Gateway/WAF</span><span>AKS</span><span>ACR</span><span>Azure Monitor</span><span>Log Analytics</span><span>Application Insights</span><span>Key Vault</span><span>Entra ID</span><span>RBAC</span><span>Managed Identity</span><span>Azure Policy</span>
                </div>
            </div>
        </section>

        <!-- Infrastructure as Code -->
        <section>
            <h2><i class="fa-solid fa-code"></i> Infrastructure as Code</h2>
            <img src="https://img.shields.io/badge/Terraform-844FBA?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform" style="border-radius:6px; margin-bottom: 15px;">
            <div class="tags-container">
                <span class="tag">Terraform</span>
                <span class="tag">Reusable Terraform Modules</span>
                <span class="tag">Remote State Management</span>
                <span class="tag">Bicep</span>
                <span class="tag">ARM Templates</span>
                <span class="tag">Infrastructure Standardization</span>
                <span class="tag">Cloud Provisioning & Automation</span>
            </div>
        </section>

        <!-- CI/CD & DevOps -->
        <section>
            <h2><i class="fa-solid fa-infinity"></i> CI/CD & DevOps</h2>
            <div style="display: flex; gap: 15px; margin-bottom: 20px; flex-wrap: wrap;">
                <img src="https://img.shields.io/badge/Azure%20DevOps-0078D7?style=for-the-badge&logo=azuredevops&logoColor=white" alt="Azure DevOps" style="border-radius:6px;">
                <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions" style="border-radius:6px;">
                <img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white" alt="Jenkins" style="border-radius:6px;">
            </div>
            <div class="tags-container">
                <span class="tag">Azure DevOps Pipelines</span>
                <span class="tag">GitHub Actions</span>
                <span class="tag">Azure Repos</span>
                <span class="tag">YAML Pipelines</span>
                <span class="tag">Build & Release Automation</span>
                <span class="tag">Deployment Automation</span>
                <span class="tag">Rollback Strategies</span>
                <span class="tag">CI/CD Security Integration</span>
            </div>
        </section>

        <!-- Containers, Kubernetes & GitOps -->
        <section>
            <h2><i class="fa-solid fa-server"></i> Containers, Kubernetes & GitOps</h2>
            <div style="display: flex; gap: 15px; margin-bottom: 20px; flex-wrap: wrap;">
                <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" style="border-radius:6px;">
                <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes" style="border-radius:6px;">
                <img src="https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white" alt="Helm" style="border-radius:6px;">
                <img src="https://img.shields.io/badge/ArgoCD-EF7B4D?style=for-the-badge&logo=argo&logoColor=white" alt="ArgoCD" style="border-radius:6px;">
            </div>
            <div class="tags-container">
                <span class="tag">Docker Containerization</span>
                <span class="tag">Kubernetes</span>
                <span class="tag">Azure Kubernetes Service (AKS)</span>
                <span class="tag">Amazon EKS</span>
                <span class="tag">Kubernetes Namespaces</span>
                <span class="tag">Ingress Controllers</span>
                <span class="tag">Autoscaling</span>
                <span class="tag">Helm Charts</span>
                <span class="tag">Argo CD</span>
                <span class="tag">GitOps-based Deployment</span>
            </div>
        </section>

        <!-- DevSecOps & Cloud Security -->
        <section>
            <h2><i class="fa-solid fa-shield-cat"></i> DevSecOps & Cloud Security</h2>
            <div style="display: flex; gap: 15px; margin-bottom: 20px; flex-wrap: wrap;">
                <img src="https://img.shields.io/badge/SonarQube-4E9BCD?style=for-the-badge&logo=sonarqube&logoColor=white" alt="SonarQube" style="border-radius:6px;">
                <img src="https://img.shields.io/badge/Trivy-1904DA?style=for-the-badge&logo=aquasec&logoColor=white" alt="Trivy" style="border-radius:6px;">
            </div>
            <table class="custom-table">
                <tr>
                    <th>Area</th>
                    <th>Technologies</th>
                </tr>
                <tr>
                    <td>🔍 Code Security</td>
                    <td>SonarQube, SAST, DAST</td>
                </tr>
                <tr>
                    <td>🐳 Container Security</td>
                    <td>Trivy</td>
                </tr>
                <tr>
                    <td>🏗️ IaC Security</td>
                    <td>Checkov, tfsec</td>
                </tr>
                <tr>
                    <td>🔐 Identity</td>
                    <td>Entra ID, RBAC, Managed Identity</td>
                </tr>
                <tr>
                    <td>🔑 Secrets</td>
                    <td>Azure Key Vault</td>
                </tr>
                <tr>
                    <td>🔗 Authentication</td>
                    <td>OIDC</td>
                </tr>
                <tr>
                    <td>🛡️ Cloud Security</td>
                    <td>Microsoft Defender for Cloud, Azure Policy</td>
                </tr>
            </table>
        </section>

        <!-- Monitoring & Observability -->
        <section>
            <h2><i class="fa-solid fa-chart-pie"></i> Monitoring & Observability</h2>
            <div style="display: flex; gap: 15px; margin-bottom: 20px; flex-wrap: wrap;">
                <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white" alt="Prometheus" style="border-radius:6px;">
                <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white" alt="Grafana" style="border-radius:6px;">
            </div>
            <div class="tags-container">
                <span class="tag">Azure Monitor</span>
                <span class="tag">Log Analytics</span>
                <span class="tag">Application Insights</span>
                <span class="tag">Prometheus</span>
                <span class="tag">Grafana</span>
                <span class="tag">Alert Management</span>
                <span class="tag">System Monitoring</span>
                <span class="tag">Performance Visibility</span>
                <span class="tag">Root Cause Analysis (RCA)</span>
            </div>
        </section>

        <!-- Featured Project -->
        <section class="featured-box">
            <h2><i class="fa-solid fa-rocket"></i> Featured Project: Cloud-Native Application Deployment on Azure</h2>
            <p style="color: var(--text-muted); margin-bottom: 15px;"><strong>Tech Stack:</strong> Azure | AKS | Docker | ACR | Helm | Argo CD | Azure DevOps | GitHub Actions | Terraform</p>
            <ul class="about-grid">
                <li>🐳 Containerized applications using Docker</li>
                <li>📦 Published container images to Azure Container Registry (ACR)</li>
                <li>🔄 Built robust CI/CD pipelines via Azure DevOps & GitHub Actions</li>
                <li>☸️ Deployed scalable workloads on Azure Kubernetes Service (AKS)</li>
                <li>⛵ Used Kubernetes manifests & Helm charts for deployments</li>
                <li>🚀 Implemented GitOps-based CD workflows using Argo CD</li>
                <li>🏗️ Provisioned complete Azure infrastructure using Terraform</li>
                <li>📊 Configured advanced monitoring via Azure Monitor, Prometheus & Grafana</li>
            </ul>
        </section>

        <!-- Operating Systems -->
        <section>
            <h2><i class="fa-solid fa-computer"></i> Operating Systems</h2>
            <div style="display: flex; gap: 15px;">
                <img src="https://img.shields.io/badge/Windows-0078D6.svg?style=for-the-badge&logo=windows&logoColor=white" alt="Windows" style="border-radius:6px;">
                <img src="https://img.shields.io/badge/Linux-FCC624.svg?style=for-the-badge&logo=linux&logoColor=black" alt="Linux" style="border-radius:6px;">
            </div>
        </section>

        <!-- Currently Exploring -->
        <section>
            <h2><i class="fa-solid fa-brain"></i> Currently Exploring</h2>
            <div class="code-block">Kubernetes         ███████████████████░  Advanced
Terraform          ███████████████████░  Advanced
Azure              ████████████████████  Advanced
Docker             ███████████████████░  Advanced
CI/CD              ████████████████████  Advanced
GitOps             █████████████████░░░  Advanced
Observability      ████████████████░░░░  Learning
AI-assisted DevOps ██████████████░░░░░░  Exploring</div>
        </section>

        <!-- GitHub Activity -->
        <section class="activity-box">
            <h2><i class="fa-solid fa-chart-bar"></i> GitHub Activity</h2>
            <img src="https://github-readme-activity-graph.vercel.app/graph?username=ranjeet-112&theme=github-compact&hide_border=true" alt="GitHub Activity Graph" />
        </section>

        <!-- Connect Section -->
        <section style="text-align: center;">
            <h2><i class="fa-solid fa-handshake"></i> Let's Connect</h2>
            <div class="connect-buttons">
                <a href="https://www.linkedin.com/in/ranjeet-singh-42508b158/" class="btn-connect btn-linkedin" target="_blank">
                    <i class="fa-brands fa-linkedin"></i> LinkedIn
                </a>
                <a href="mailto:ranjeetsee112@gmail.com" class="btn-connect btn-gmail">
                    <i class="fa-solid fa-envelope"></i> Gmail
                </a>
                <a href="https://github.com/ranjeet-112" class="btn-connect btn-github" target="_blank">
                    <i class="fa-brands fa-github"></i> GitHub
                </a>
            </div>
        </section>

        <!-- Footer -->
        <footer>
            <p>⚡ <em>Automate • Secure • Deploy • Monitor</em></p>
            <p style="margin-top: 10px;">Thanks for visiting my portfolio! 🚀 &copy; 2026 Ranjeet Kumar Singh</p>
        </footer>
    </div>

</body>
</html>
