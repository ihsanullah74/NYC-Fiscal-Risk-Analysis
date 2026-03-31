# NYC Fiscal Risk Analysis: A Monte Carlo Approach 🏙️📊

---

## 📝 Executive Summary
Can New York City’s **"Affordability Agenda"** survive a $12B budget deficit? This project conducts an independent **Quantitative Stress-Test** on proposed policies—including Free Bus Transit, Universal Rent Freezes, and Subsidized Grocery programs.

By simulating **100,000 economic scenarios**, this analysis determines the true probability of fiscal sustainability against a **$2.0 Billion** budget threshold.

---

## ⚙️ Technical Methodology
To account for economic uncertainty (inflation, administrative overhead, and ridership spikes), I modeled the total annual cost as a sum of stochastic variables sampled from normal distributions.

### The Model
The Total Annual Cost ($C_{total}$) is defined as:

$$C_{total} = \sum_{i=1}^{n} P_i$$

Where each individual policy cost ($P_i$) is sampled as:

$$P_i \sim \mathcal{N}(\mu_i, \sigma_i)$$

### Simulation Parameters:
* **Total Iterations:** 100,000 simulations 
* **Budget Ceiling:** $2,000,000,000 
* **Risk Margin:** 20% Standard Deviation applied across policy means 

---

## 📈 Key Findings
Based on the simulation results:
* **Mean Estimated Cost:** $2,670,526,606
* **Max Estimated Cost:** $5,002,921,319
* **Risk of Failure:** There is a **90.00% probability** that implementation costs will exceed the $2.0B budget threshold.

---<img width="606" height="385" alt="Screenshot 2026-03-29 204141" src="https://github.com/user-attachments/assets/9273f389-b850-4279-a9bc-ca200ab9253e" />


## 🛠️ Tools & Libraries
* **Python 3.x**
* **NumPy:** High-performance stochastic simulations 
* **Matplotlib:** Distribution and risk visualization 
* **Pandas:** Data structuring and manipulation
