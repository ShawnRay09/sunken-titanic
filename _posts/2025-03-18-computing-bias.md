---
toc: true
layout: post
title: Computing Bias Lesson
description: By Shawn Ray, Jonah Luo, Tarun Rayavarapu, Arya Savlani
---

# Computing Bias Lesson

## Introduction

Computing bias occurs when computer systems systematically and unfairly discriminate against certain groups. Bias in computing can reinforce social inequalities, create unfair advantages, and lead to real-world harm. This lesson explores how bias emerges, real-world examples, and strategies for mitigation.

---

## What is Computing Bias?

> "We can say that a computer system is biased if it both unfairly and systematically discriminates against one group in favor of another." – *Nissenbaum et al.* ([Cornell Paper](https://nissenbaum.tech.cornell.edu/papers/Discerning%20Bias%20in%20Computer%20Systems.pdf))

### Doctor or Nurse Drawings

<!-- HTML block for interactivity -->
<button onclick="assignRole()">Get Role</button>
<p id="result"></p>

<script>
    function assignRole() {
        let role = Math.random() < 0.5 ? "Doctor" : "Nurse";
        document.getElementById("result").innerText = "Draw a: " + role;
    }
</script>

### **Types of Bias in Computing**

1. **Pre-existing Social Bias**
   - Originates from societal norms, stereotypes, or historical inequalities.
   - Embedded into technology due to biased data, biased creators, or societal influence.
   - **Examples:**
     - Hiring algorithms favoring men over women.
     - Facial recognition systems performing poorly on non-white faces.

2. **Technical Bias**
   - Stems from design, implementation, or structural limitations in technology.
   - Even systems built with good intentions may introduce bias through their function.
   - **Examples:**
     - Google Translate assigning gendered pronouns based on stereotypes.
     - Default settings not representing all user demographics.

3. **Emergent Social Bias**
   - Develops over time as a system interacts with users or adapts to real-world data.
   - AI models may evolve in a biased manner based on user interactions.
   - **Examples:**
     - AI chatbots learning harmful language from users.
     - Search engines amplifying biased content over time.

---

## Real-World Examples of Computing Bias

### **Amazon's AI Hiring Tool**
- **Bias Type:** Pre-existing Social Bias  
- Amazon's AI recruitment system favored male candidates due to past hiring data.
- The system penalized resumes with words like "women" (e.g., *“Women’s Chess Club”*).
- **Impact:** Women were unfairly ranked lower for job opportunities.  
🔗 [Read More](https://www.ml.cmu.edu/news/news-archive/2016-2020/2018/october/amazon-scraps-secret-artificial-intelligence-recruiting-engine-that-showed-biases-against-women.html)

### **Google Translate Gender Bias**
- **Bias Type:** Technical Bias  
- When translating from gender-neutral languages, it introduced gender assumptions.
- Example:
  - Turkish: *O bir doktor* → English: *He is a doctor*  
  - Turkish: *O bir hemşire* → English: *She is a nurse*  
- **Impact:** Reinforced stereotypes about professions.  
🔗 [Read More](https://qz.com/1141122/google-translates-gender-bias-pairs-he-with-hardworking-and-she-with-lazy-and-other-examples)

### **Microsoft’s AI Chatbot Tay**
- **Bias Type:** Emergent Social Bias  
- Tay learned from Twitter interactions but was manipulated into tweeting racist and offensive content within 24 hours.
- **Impact:** AI can absorb and amplify human biases without proper safeguards.  
🔗 [Read More](https://fortune.com/longform/ai-bias-problem)

---

(Insert Bias Fixes here)

| **MCQ Topic** | **Connection to Computing Bias** |
|-----------|---------------------------------|
| **2.3: Extracting Information from Data** | Bias can emerge when datasets are skewed or incomplete, leading to biased AI predictions and decisions. |
| **3.12: Calling Procedures** | If biased functions or APIs are repeatedly used, the bias spreads throughout a system, such as facial recognition errors. |
| **3.17: Algorithmic Efficiency** | Some efficient algorithms may prioritize speed over fairness, reinforcing biases in search engines or recommendation systems. |
| **5.1: Beneficial and Harmful Effects** | Biased algorithms can offer personalized recommendations (benefit) but may also create filter bubbles and reinforce stereotypes (harm). |
| **5.2: Digital Divide** | Bias in computing can worsen accessibility gaps, such as voice recognition software struggling with non-native accents. |
