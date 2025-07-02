---
title: "Deploy AI Applications in Minutes, Not Hours"
description: "VoidRunner's AI-powered platform automatically detects and sets up runtime environments from just your code. Skip the infrastructure complexity and focus on building."
draft: false
layout: "home"

# Hero section
hero:
  enable: true
  title: "Deploy AI Applications in **Minutes, Not Hours**"
  subtitle: "VoidRunner's AI-powered platform automatically detects and sets up runtime environments from just your code. Skip the infrastructure complexity and focus on building."
  button:
    enable: true
    label: "Start Free"
    link: "https://app.voidrunner.dev/signup"
  button_alt:
    enable: true
    label: "View Demo"
    link: "#demo"
  image: "/images/hero-dashboard.png"
  video:
    enable: true
    youtube_id: "dQw4w9WgXcQ"

# Code example section
code_demo:
  enable: true
  title: "From Code to Production in **3 Simple Steps**"
  subtitle: "Just provide your code and description. Our AI does the rest."
  steps:
    - title: "1. Submit Your Code"
      description: "Upload your application code with a simple description"
      code: |
        ```json
        {
          "name": "ML Image Classifier",
          "description": "TensorFlow model for image classification with REST API",
          "code": "from flask import Flask, request\nimport tensorflow as tf\n\napp = Flask(__name__)\nmodel = tf.keras.models.load_model('model.h5')\n\n@app.route('/predict', methods=['POST'])\ndef predict():\n    # Your ML code here\n    return {'prediction': result}"
        }
        ```
    - title: "2. AI Environment Detection"
      description: "Our AI analyzes dependencies and creates optimal container environment"
      code: |
        ```dockerfile
        FROM python:3.9-slim
        WORKDIR /app

        # AI-detected dependencies
        COPY requirements.txt .
        RUN pip install tensorflow==2.13.0 flask==2.3.2

        COPY . .
        EXPOSE 5000
        CMD ["python", "app.py"]
        ```
    - title: "3. Deploy & Scale"
      description: "Instant deployment with automatic scaling and monitoring"
      code: |
        ```bash
        ✅ Environment detected: Python 3.9 + TensorFlow
        ✅ Container built: ml-classifier-a4f2x:rev-1
        ✅ Deployed: https://ml-classifier.voidrunner.app
        ✅ Scaling: 0→3 instances (auto)

        📊 Status: Ready (99.9% uptime)
        🚀 Cold start: <800ms
        💰 Cost: $0.12/hour
        ```

# Features section
features:
  enable: true
  title: "**Intelligent Infrastructure** That Thinks Like You"
  subtitle: "Stop wrestling with Docker, Kubernetes, and cloud complexity. VoidRunner's AI understands your code and sets up everything automatically."

  feature_list:
    - icon: "fas fa-brain"
      title: "AI-Powered Environment Detection"
      description: "Advanced language models analyze your code to detect dependencies, frameworks, and optimal runtime configurations automatically."

    - icon: "fas fa-rocket"
      title: "Sub-Second Cold Starts"
      description: "Pre-warmed containers and intelligent caching deliver blazing-fast performance with minimal latency."

    - icon: "fas fa-shield-alt"
      title: "Enterprise-Grade Security"
      description: "gVisor sandboxing, container isolation, and SOC 2 compliance keep your code and data secure."

    - icon: "fas fa-chart-line"
      title: "Usage-Based Scaling"
      description: "Pay only for what you use with transparent pricing and automatic scaling that grows with your needs."

    - icon: "fas fa-code"
      title: "Multi-Language Support"
      description: "Python, Node.js, Go, Java, Rust, and more. If you can code it, we can run it."

    - icon: "fas fa-cogs"
      title: "Developer-First API"
      description: "RESTful APIs, comprehensive SDKs, and detailed documentation designed by developers, for developers."

# Social proof section
testimonials:
  enable: true
  title: "Trusted by **Developers Worldwide**"
  subtitle: "Join thousands of developers who've eliminated infrastructure headaches"

  testimonial_list:
    - name: "Sarah Chen"
      designation: "Senior ML Engineer @ TechFlow"
      avatar: "/images/testimonials/sarah.jpg"
      content: "VoidRunner cut our deployment time from 4 hours to 3 minutes. The AI environment detection is incredibly accurate - it understood our complex ML pipeline instantly."

    - name: "Marcus Rodriguez"
      designation: "Lead DevOps @ StartupX"
      avatar: "/images/testimonials/marcus.jpg"
      content: "Finally, a platform that just works. No more Dockerfile debugging or Kubernetes YAML wrestling. Our team can focus on shipping features, not infrastructure."

    - name: "Dr. Emily Watson"
      designation: "Research Scientist @ AI Labs"
      avatar: "/images/testimonials/emily.jpg"
      content: "The automatic dependency resolution saved us weeks of environment setup. VoidRunner handles our research workloads seamlessly."

# Stats section
stats:
  enable: true
  title: "**Proven Performance** at Scale"

  stat_list:
    - number: "1M+"
      title: "Functions Deployed"

    - number: "99.9%"
      title: "Uptime SLA"

    - number: "<800ms"
      title: "Average Cold Start"

    - number: "50+"
      title: "Languages Supported"

# Pricing preview
pricing_preview:
  enable: true
  title: "**Transparent Pricing** That Scales With You"
  subtitle: "Start free, pay only for what you use. No hidden fees, no surprises."

  plans:
    - name: "Developer"
      price: "Free"
      description: "Perfect for learning and small projects"
      features:
        - "1,000 function executions/month"
        - "10 GB-hours compute time"
        - "5GB bandwidth"
        - "Community support"
      button:
        label: "Start Free"
        link: "https://app.voidrunner.dev/signup"

    - name: "Pro"
      price: "$29"
      price_period: "/month"
      description: "For professional developers and growing projects"
      features:
        - "50,000 executions included"
        - "100 GB-hours compute"
        - "100GB bandwidth"
        - "Email support"
        - "Advanced monitoring"
      button:
        label: "Start Pro Trial"
        link: "https://app.voidrunner.dev/signup?plan=pro"
      popular: true

    - name: "Enterprise"
      price: "Custom"
      description: "For teams and large-scale applications"
      features:
        - "Unlimited executions"
        - "Custom SLAs"
        - "Dedicated support"
        - "Advanced security"
        - "Volume discounts"
      button:
        label: "Contact Sales"
        link: "/contact/"

# CTA section
cta:
  enable: true
  title: "Ready to **Deploy Smarter**?"
  subtitle: "Join thousands of developers who've eliminated infrastructure complexity with VoidRunner."
  button:
    label: "Start Building for Free"
    link: "https://app.voidrunner.dev/signup"
  button_alt:
    label: "Schedule Demo"
    link: "/contact/"
---

<!-- Custom sections can be added here -->

## Why Developers Choose VoidRunner

Traditional deployment workflows are broken. You spend more time configuring environments than building features. VoidRunner fixes this with AI-powered automation that understands your code and sets up everything perfectly, every time.

### The Old Way: Infrastructure Hell

- Manual Dockerfile creation and debugging
- Complex Kubernetes YAML configurations
- Hours of environment troubleshooting
- Unpredictable deployment failures
- Expensive DevOps overhead

### The VoidRunner Way: AI-Powered Simplicity

- Submit code + description → Instant deployment
- Automatic dependency detection and resolution
- Zero-config container optimization
- Predictable, usage-based pricing
- Focus on features, not infrastructure
