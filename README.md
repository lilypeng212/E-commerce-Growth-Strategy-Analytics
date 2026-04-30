# Business Analyst — E-commerce Analytics

**Role:** Business Analyst (Full-Time: 40 hrs/wk)  
**When:** Nov. 2024 – Nov. 2025  
**Location:** Taipei, Taiwan  

> **Disclaimer:** This portfolio uses sanitized descriptions and synthetic examples only.  
> No proprietary code, data, screenshots, internal IDs, or client configurations are included.

---
# E-commerce Growth Strategy & Analytics

## 📌 Problem
The e-commerce platform lacked visibility into product performance and customer conversion behavior, resulting in missed growth opportunities and inefficient resource allocation.

---

## 💡 Solution
Designed a structured analytics framework to identify revenue drivers, optimize product assortment, and improve conversion rates.

Key components:
- Defined core business metrics (GMV, AOV, Conversion Rate)
- Built product performance segmentation logic
- Designed customer funnel analysis framework
- Proposed dashboard for continuous monitoring

---

## 🔍 Highlights
- Developed KPI tree linking traffic → conversion → revenue
- Identified high-traffic but low-conversion product segments
- Designed customer segmentation logic (new vs returning users)
- Proposed experiment framework for conversion optimization

---

## 📈 Impact
- Identified potential 10–15% GMV uplift through product optimization
- Improved decision-making speed by structuring key metrics
- Enabled data-driven prioritization for product and marketing teams

---

## 🧠 Framework
import matplotlib.pyplot as plt

stages = ['Visit', 'Click', 'Add to Cart', 'Purchase']
values = [10000, 3000, 1000, 400]

plt.figure()
plt.plot(stages, values, marker='o')
plt.title('Conversion Funnel')
plt.xlabel('Stage')
plt.ylabel('Users')
plt.show()

import networkx as nx
import matplotlib.pyplot as plt

G = nx.DiGraph()

G.add_edges_from([
    ('GMV', 'Traffic'),
    ('GMV', 'Conversion Rate'),
    ('GMV', 'AOV'),
    ('Conversion Rate', 'Add to Cart'),
    ('Conversion Rate', 'Checkout')
])

pos = nx.spring_layout(G)
nx.draw(G, pos, with_labels=True)
plt.show()
