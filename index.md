---
layout: page
title: Home
---

# Aripravina S

## Cybersecurity Learning Journal

**Documenting my journey from cybersecurity fundamentals to practical SOC analysis — one concept, one lab, and one lesson at a time.**

[ **Read the Blog →** ]({{ '/archives/' | relative_url }})

---

## 👋 About Me

Hi, I'm **Aripravina S**, an MCA graduate from **Pondicherry University**.

I'm currently building my cybersecurity knowledge from the ground up, starting with computer and networking fundamentals and gradually moving toward **Security Operations and SOC analysis**.

This blog is my personal learning journal where I document what I study, the labs I practice, and the lessons I learn along the way.

[ **More About Me →** ]({{ '/about/' | relative_url }})

---

## 🔐 What I'm Learning

My current learning journey covers:

**💻 Computer & IT Fundamentals**  
Building the foundation of how computers, operating systems and filesystems work.

**🌐 Networking**  
Understanding IP addresses, protocols, ports, packet flow and how devices communicate.

**🪟 Windows & Active Directory**  
Learning Windows systems, users, permissions, services and Active Directory fundamentals.

**🐧 Linux**  
Practicing Linux commands, permissions, processes, services and logs using Ubuntu.

**🔐 Security Fundamentals**  
Learning core cybersecurity concepts, security controls, authentication, encryption, hashing and risk.

**🔎 SOC & Security Operations**  
Gradually moving toward security monitoring, logs, SIEM, alert triage and incident investigation.

---

## 📝 Latest Posts

The latest lessons from my cybersecurity learning journey will appear here.

{% for post in site.posts limit:5 %}

### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.date | date: "%B %d, %Y" }}

{% if post.excerpt %}
{{ post.excerpt | strip_html | truncate: 180 }}
{% endif %}

---

{% endfor %}

[ **View All Posts →** ]({{ '/archives/' | relative_url }})

---

## 🧪 Learning Through Practice

Whenever possible, I combine what I study with hands-on practice.

- 🌐 Networking exercises and packet analysis
- 🐧 Linux command-line practice
- 🪟 Windows and system exploration
- 🔎 Log analysis
- 🧪 Beginner cybersecurity labs
- 📊 Security monitoring and investigation exercises

---

> **One concept. One lab. One lesson at a time.**
