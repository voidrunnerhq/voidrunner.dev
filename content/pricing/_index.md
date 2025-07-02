---
title: "Pricing"
description: "Transparent, usage-based pricing that scales with your success. Start free, pay only for what you use."
draft: false
layout: "pricing"

# Hero section
hero:
  enable: true
  title: "**Transparent Pricing** That Scales With You"
  subtitle: "Start free, pay only for what you use. No hidden fees, no vendor lock-in, no surprises."

# Pricing tiers
pricing_tiers:
  enable: true

  tiers:
    - name: "Developer"
      price: "Free"
      price_period: "forever"
      description: "Perfect for learning, prototyping, and personal projects"
      color: "blue"
      features:
        - text: "1,000 function executions/month"
          included: true
        - text: "10 GB-hours compute time"
          included: true
        - text: "5GB bandwidth"
          included: true
        - text: "Community support"
          included: true
        - text: "Basic monitoring"
          included: true
        - text: "Public GitHub repos"
          included: true
        - text: "Standard security"
          included: true
        - text: "Priority support"
          included: false
        - text: "Private repositories"
          included: false
        - text: "Advanced monitoring"
          included: false
        - text: "Team collaboration"
          included: false
        - text: "Custom domains"
          included: false
      button:
        label: "Start Free"
        link: "https://app.voidrunner.dev/signup"

    - name: "Pro"
      price: "$29"
      price_period: "/month"
      description: "For professional developers and growing applications"
      color: "purple"
      popular: true
      features:
        - text: "50,000 executions included"
          included: true
        - text: "100 GB-hours compute included"
          included: true
        - text: "100GB bandwidth included"
          included: true
        - text: "Email support (24h response)"
          included: true
        - text: "Advanced monitoring & logs"
          included: true
        - text: "Private repositories"
          included: true
        - text: "Custom domains"
          included: true
        - text: "Enhanced security"
          included: true
        - text: "Team collaboration (5 seats)"
          included: true
        - text: "API access"
          included: true
        - text: "Deployment webhooks"
          included: true
        - text: "Environment variables"
          included: true
      overages:
        - text: "$0.20 per 1,000 additional executions"
        - text: "$0.50 per additional GB-hour"
        - text: "$0.10 per additional GB bandwidth"
      button:
        label: "Start Pro Trial"
        link: "https://app.voidrunner.dev/signup?plan=pro"

    - name: "Team"
      price: "$99"
      price_period: "/month"
      description: "For teams building production applications"
      color: "green"
      features:
        - text: "500,000 executions included"
          included: true
        - text: "1,000 GB-hours compute included"
          included: true
        - text: "1TB bandwidth included"
          included: true
        - text: "Priority support (4h response)"
          included: true
        - text: "Advanced monitoring & alerting"
          included: true
        - text: "Unlimited private repos"
          included: true
        - text: "Custom domains & SSL"
          included: true
        - text: "Enhanced security & compliance"
          included: true
        - text: "Team collaboration (25 seats)"
          included: true
        - text: "Advanced API features"
          included: true
        - text: "CI/CD integrations"
          included: true
        - text: "Environment management"
          included: true
      overages:
        - text: "$0.15 per 1,000 additional executions"
        - text: "$0.40 per additional GB-hour"
        - text: "$0.08 per additional GB bandwidth"
      button:
        label: "Start Team Trial"
        link: "https://app.voidrunner.dev/signup?plan=team"

    - name: "Enterprise"
      price: "Custom"
      price_period: ""
      description: "For large teams and mission-critical applications"
      color: "gray"
      features:
        - text: "Custom execution limits"
          included: true
        - text: "Dedicated compute resources"
          included: true
        - text: "Unlimited bandwidth"
          included: true
        - text: "24/7 dedicated support"
          included: true
        - text: "Custom SLAs (99.95%+ uptime)"
          included: true
        - text: "Advanced security features"
          included: true
        - text: "SSO/SCIM integration"
          included: true
        - text: "Compliance certifications"
          included: true
        - text: "Unlimited team members"
          included: true
        - text: "Premium API features"
          included: true
        - text: "Custom integrations"
          included: true
        - text: "Dedicated account manager"
          included: true
      button:
        label: "Contact Sales"
        link: "/contact/"

# Usage calculator
usage_calculator:
  enable: true
  title: "**Calculate Your Costs**"
  subtitle: "Estimate your monthly bill based on your usage patterns"

# Feature comparison
feature_comparison:
  enable: true
  title: "**Feature Comparison**"
  subtitle: "Compare plans and find the perfect fit for your needs"

  categories:
    - name: "Compute Resources"
      features:
        - name: "Function Executions"
          developer: "1,000/month"
          pro: "50,000/month"
          team: "500,000/month"
          enterprise: "Unlimited"
        - name: "Compute Time"
          developer: "10 GB-hours"
          pro: "100 GB-hours"
          team: "1,000 GB-hours"
          enterprise: "Unlimited"
        - name: "Memory per Function"
          developer: "512MB - 1GB"
          pro: "512MB - 4GB"
          team: "512MB - 8GB"
          enterprise: "Custom"
        - name: "Execution Timeout"
          developer: "15 minutes"
          pro: "30 minutes"
          team: "60 minutes"
          enterprise: "Custom"

    - name: "Development Features"
      features:
        - name: "Private Repositories"
          developer: false
          pro: true
          team: true
          enterprise: true
        - name: "Custom Domains"
          developer: false
          pro: true
          team: true
          enterprise: true
        - name: "Environment Variables"
          developer: "Limited"
          pro: "Unlimited"
          team: "Unlimited"
          enterprise: "Unlimited"
        - name: "Deployment Rollbacks"
          developer: "3 versions"
          pro: "10 versions"
          team: "50 versions"
          enterprise: "Unlimited"

    - name: "Monitoring & Support"
      features:
        - name: "Basic Monitoring"
          developer: true
          pro: true
          team: true
          enterprise: true
        - name: "Advanced Analytics"
          developer: false
          pro: true
          team: true
          enterprise: true
        - name: "Custom Alerts"
          developer: false
          pro: "Basic"
          team: "Advanced"
          enterprise: "Custom"
        - name: "Support Response Time"
          developer: "Community"
          pro: "24 hours"
          team: "4 hours"
          enterprise: "1 hour"

# FAQ section
faq:
  enable: true
  title: "**Frequently Asked Questions**"

  questions:
    - question: "How does usage-based pricing work?"
      answer: "You're charged based on three main metrics: function executions (each time your code runs), compute time (GB-hours of actual processing), and bandwidth (data transfer). Each plan includes generous limits, and you only pay for usage beyond those limits."

    - question: "What happens if I exceed my plan limits?"
      answer: "Your applications continue running without interruption. You'll be charged the overage rates shown for each plan. You can set spending limits and alerts to avoid unexpected charges."

    - question: "Can I change plans anytime?"
      answer: "Yes! You can upgrade or downgrade your plan at any time. Changes take effect immediately, and billing is prorated based on usage."

    - question: "Is there a free tier forever?"
      answer: "Absolutely. Our Developer plan is free forever with generous limits perfect for learning, prototyping, and personal projects. No credit card required to get started."

    - question: "What's included in compute time?"
      answer: "Compute time is measured in GB-hours: the amount of memory allocated to your function multiplied by execution time. A function using 1GB of memory running for 1 hour equals 1 GB-hour."

    - question: "Do you offer academic discounts?"
      answer: "Yes! We provide special pricing for educational institutions and students. Contact our sales team with your academic email for details."

    - question: "What payment methods do you accept?"
      answer: "We accept all major credit cards (Visa, MasterCard, American Express) and ACH transfers for Enterprise customers. All payments are processed securely through Stripe."

    - question: "Is there a long-term contract requirement?"
      answer: "No contracts required. All plans are month-to-month. Enterprise customers can opt for annual contracts with additional discounts."

# Enterprise features
enterprise_features:
  enable: true
  title: "**Enterprise Features**"
  subtitle: "Advanced capabilities for mission-critical applications"

  features:
    - title: "Dedicated Infrastructure"
      description: "Isolated compute resources with guaranteed performance and enhanced security for your applications."
      icon: "fas fa-server"

    - title: "Advanced Security"
      description: "SOC 2 Type II compliance, custom security policies, audit logging, and enterprise-grade encryption."
      icon: "fas fa-shield-alt"

    - title: "Custom SLAs"
      description: "Tailored service level agreements with 99.95%+ uptime guarantees and priority incident response."
      icon: "fas fa-handshake"

    - title: "SSO Integration"
      description: "Single sign-on with SAML, OAuth, and SCIM support for seamless identity management."
      icon: "fas fa-users-cog"

# Cost comparison
cost_comparison:
  enable: true
  title: "**Compare With Alternatives**"
  subtitle: "See how VoidRunner's transparent pricing stacks up against traditional cloud providers"

  scenarios:
    - name: "Small Application"
      description: "10,000 requests/month, 1GB memory, 100ms average execution"
      voidrunner: "$3.20"
      aws_lambda: "$4.20"
      google_cloud: "$4.50"
      azure: "$4.80"

    - name: "Medium Application"
      description: "100,000 requests/month, 2GB memory, 250ms average execution"
      voidrunner: "$24.50"
      aws_lambda: "$31.20"
      google_cloud: "$33.80"
      azure: "$35.20"

    - name: "Large Application"
      description: "1M requests/month, 4GB memory, 500ms average execution"
      voidrunner: "$189.00"
      aws_lambda: "$247.50"
      google_cloud: "$264.30"
      azure: "$278.90"

# CTA section
cta:
  enable: true
  title: "Ready to **Start Building**?"
  subtitle: "Join thousands of developers who've eliminated infrastructure complexity with transparent, predictable pricing."
  button:
    label: "Start Free Trial"
    link: "https://app.voidrunner.dev/signup"
  button_alt:
    label: "Contact Sales"
    link: "/contact/"
---

## Fair, Transparent Pricing

VoidRunner's usage-based pricing ensures you only pay for what you actually use. No hidden fees, no surprise bills, and no vendor lock-in. Our pricing scales with your success, making it perfect for everything from personal projects to enterprise applications.

### Why Usage-Based Pricing?

Traditional cloud providers charge for reserved capacity whether you use it or not. VoidRunner charges based on actual resource consumption:

- **Function Executions**: Pay per request, not per hour
- **Compute Time**: Charged only while your code is running
- **Bandwidth**: Fair pricing for data transfer
- **Storage**: Optional persistent storage at competitive rates

### Enterprise Volume Discounts

Large-scale deployments qualify for significant volume discounts:

- **1M+ executions/month**: Up to 25% discount
- **Annual commitments**: Additional 15% savings
- **Multi-region deployments**: Custom pricing available

Ready to see how much you could save? Use our cost calculator above or contact our sales team for a personalized quote.
