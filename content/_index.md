---
title: "Execute Distributed Tasks in Minutes, Not Hours"
description: "VoidRunner's AI-powered platform automatically detects optimal runtime environments and orchestrates computational workloads. Skip the distributed computing complexity and focus on your tasks."
draft: false
layout: "home"

# Hero section
hero:
  enable: true
  title: "Execute Distributed Tasks in **Minutes, Not Hours**"
  subtitle: "VoidRunner's AI-powered platform automatically detects optimal runtime environments and orchestrates computational workloads across distributed infrastructure. Skip the complexity and focus on your tasks."
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
  title: "From Code to Execution in **3 Simple Steps**"
  subtitle: "Just provide your task code and description. Our AI orchestrates the execution."
  steps:
    - title: "1. Submit Your Task"
      description: "Upload your computational task code with a simple description"
      code: |
        ```json
        {
          "name": "Fibonacci Calculator",
          "description": "Calculate Fibonacci numbers using recursive algorithm",
          "code": "import math\n\ndef calculate_fibonacci(n):\n    \"\"\"Calculate the nth Fibonacci number\"\"\"\n    if n <= 1:\n        return n\n    return calculate_fibonacci(n-1) + calculate_fibonacci(n-2)\n\n# Calculate and display result\nresult = calculate_fibonacci(20)\nprint(f\"20th Fibonacci number: {result}\")"
        }
        ```
    - title: "2. AI Runtime Optimization"
      description: "Our AI analyzes dependencies and creates optimal execution environment"
      code: |
        ```dockerfile
        FROM python:3.9-slim
        WORKDIR /app

        # AI-optimized for computational tasks
        COPY requirements.txt .
        RUN pip install numpy==1.24.0

        COPY . .
        # Optimized for mathematical computation
        CMD ["python", "fibonacci_calculator.py"]
        ```
    - title: "3. Execute & Scale"
      description: "Instant task execution with automatic resource scaling and monitoring"
      code: |
        ```bash
        ✅ Runtime optimized: Python 3.9 + NumPy
        ✅ Task environment: fibonacci-calc-a4f2x:v1
        ✅ Executing: Task #12847 (Fibonacci sequence)
        ✅ Scaling: 1→4 workers (auto)

        📊 Status: Complete (runtime: 1.2s)
        🚀 Task startup: <300ms
        💰 Cost: $0.02/task
        ```

# Features section
features:
  enable: true
  title: "**Intelligent Task Orchestration** That Thinks Like You"
  subtitle: "Stop wrestling with distributed computing complexity. VoidRunner's AI understands your tasks and orchestrates optimal execution automatically."

  feature_list:
    - icon: "fas fa-brain"
      title: "AI-Powered Task Analysis"
      description: "Advanced language models analyze your computational tasks to detect dependencies, frameworks, and optimal execution strategies automatically."

    - icon: "fas fa-rocket"
      title: "Sub-Second Task Initialization"
      description: "Pre-warmed execution environments and intelligent resource allocation deliver blazing-fast task startup with minimal latency."

    - icon: "fas fa-shield-alt"
      title: "Enterprise-Grade Security"
      description: "gVisor sandboxing, container isolation, and SOC 2 compliance keep your code and data secure."

    - icon: "fas fa-chart-line"
      title: "Dynamic Resource Scaling"
      description: "Pay only for computational resources consumed with transparent pricing and automatic scaling that adapts to task demands."

    - icon: "fas fa-code"
      title: "Multi-Language Task Support"
      description: "Python, Node.js, Go, Java, Rust, and more. If you can code it, we can execute it at scale."

    - icon: "fas fa-cogs"
      title: "Task-Oriented APIs"
      description: "RESTful APIs optimized for task submission, monitoring, and result retrieval with comprehensive SDKs and documentation."

# Social proof section
testimonials:
  enable: true
  title: "Trusted by **Researchers & Engineers Worldwide**"
  subtitle: "Join thousands of researchers and engineers who've eliminated distributed computing headaches"

  testimonial_list:
    - name: "Sarah Chen"
      designation: "Senior ML Engineer @ TechFlow"
      avatar: "/images/testimonials/sarah.svg"
      content: "VoidRunner cut our batch processing setup from 4 hours to 3 minutes. The AI runtime optimization is incredibly accurate - it understood our complex ML workload instantly."

    - name: "Marcus Rodriguez"
      designation: "Principal Engineer @ StartupX"
      avatar: "/images/testimonials/marcus.svg"
      content: "Finally, a platform that just works. No more distributed computing setup or resource management wrestling. Our team can focus on research algorithms, not infrastructure."

    - name: "Dr. Emily Watson"
      designation: "Research Scientist @ AI Labs"
      avatar: "/images/testimonials/emily.svg"
      content: "The automatic dependency resolution saved us weeks of environment setup. VoidRunner handles our computational research tasks seamlessly."

# Stats section
stats:
  enable: true
  title: "**Proven Performance** at Scale"

  stat_list:
    - number: "1M+"
      title: "Tasks Executed"

    - number: "99.9%"
      title: "Uptime SLA"

    - number: "<800ms"
      title: "Average Task Startup"

    - number: "50+"
      title: "Languages & Frameworks"

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
        - "1,000 task executions/month"
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
        - "50,000 task executions included"
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
        - "Unlimited task executions"
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
  title: "Ready to **Execute Smarter**?"
  subtitle: "Join thousands of researchers and engineers who've eliminated distributed computing complexity with VoidRunner."
  button:
    label: "Start Executing for Free"
    link: "https://app.voidrunner.dev/signup"
  button_alt:
    label: "Schedule Demo"
    link: "/contact/"
---

<!-- Custom sections can be added here -->

## Why Researchers & Engineers Choose VoidRunner

Traditional distributed computing workflows are broken. You spend more time configuring environments than running computational tasks. VoidRunner fixes this with AI-powered automation that understands your tasks and orchestrates execution perfectly, every time.

### The Old Way: Distributed Computing Hell

- Manual environment setup and debugging
- Complex cluster configuration and management
- Hours of distributed system troubleshooting
- Unpredictable task execution failures
- Expensive infrastructure overhead

### The VoidRunner Way: AI-Powered Task Execution

- Submit task + description → Instant execution
- Automatic dependency detection and optimization
- Zero-config execution environment optimization
- Predictable, task-based pricing
- Focus on computation, not infrastructure
