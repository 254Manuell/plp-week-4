# Power Learn Project: AI for Software Engineering (Week 4 Assignment) 🚀

**Group 21**
**Members:** Brilliant Mwendwa, Lowell Owuor, Emmanuel Baraka, Teddy Brian

---

## Table of Contents 📚

1. [Project Overview 🎯](#project-overview)
2. [Part I: Theoretical Analysis 🧠](#part-i-theoretical-analysis)

   * [Q1: AI-Driven Code Generation Tools 🤖](#q1-ai-driven-code-generation-tools)
   * [Q2: Supervised vs. Unsupervised Learning in Bug Detection 🐛](#q2-supervised-vs-unsupervised-learning-in-bug-detection)
   * [Q3: Bias Mitigation for AI-Powered UX Personalization ⚖️](#q3-bias-mitigation-for-ai-powered-ux-personalization)
   * [AIOps Case Studies 📈](#aiops-case-studies)
3. [Part II: Practical Implementation 🛠️](#part-ii-practical-implementation)

   * [Task 1: AI-Powered Code Completion ✍️](#task-1-ai-powered-code-completion)
   * [Task 2: Automated Testing with Katalon Studio ✅](#task-2-automated-testing-with-katalon-studio)
   * [Task 3: Predictive Analytics for Resource Location 📊](#task-3-predictive-analytics-for-resource-location)
4. [Part III: Ethical Considerations 🤝](#part-iii-ethical-considerations)
5. [Bonus: AI-Powered Code Review Coach Proposal 💡](#bonus-ai-powered-code-review-coach-proposal)
6. [Project Structure 📂](#project-structure)
7. [Getting Started 🏁](#getting-started)
8. [License 📝](#license)

---

## Project Overview 🎯

This repository contains the Week 4 deliverables for the **AI for Software Engineering** course, showcasing both theoretical analyses and practical applications of AI-driven tools in software development. The assignment is divided into three parts:

* **Part I:** In-depth comparison and discussion of AI techniques and their impacts.
* **Part II:** Hands-on implementations demonstrating AI-powered code completion, automated testing, and predictive analytics.
* **Part III:** Ethical reflection on deploying AI models in real-world scenarios.

---

## Part I: Theoretical Analysis 🧠

### Q1: AI-Driven Code Generation Tools 🤖

* **Benefits:**

  * **Boilerplate Automation 🔄:** CRUD endpoints, configuration files—reduces repetitive coding.
  * **Context-Aware Suggestions 💡:** Inline completions based on existing code and comments.
  * **On-the-Fly Documentation 📑:** Auto-generated docstrings and type hints.
  * **Faster Reviews & Merges ⚡:** Higher-quality initial code yields quicker PR approvals.
* **Limitations:**

  * Hallucinations (buggy code), security/license risks, limited architectural understanding, skill atrophy, domain specificity, data privacy concerns.

### Q2: Supervised vs. Unsupervised Learning in Bug Detection 🐛

* **Supervised:**

  * Requires labeled datasets; high precision/recall on known bug types; can localize errors.
  * Drawbacks: annotation cost, class imbalance, limited generalization.
* **Unsupervised:**

  * Uses anomaly detection on clean code corpora; no labels needed; broad coverage for novel bugs.
  * Drawbacks: high false positives, less actionable insight, threshold tuning.
* **Recommendation:** Combine both—use unsupervised to surface issues, then supervised models on critical modules.

### Q3: Bias Mitigation for AI-Powered UX Personalization ⚖️

* **Why It Matters:** Fairness, legal compliance (e.g., GDPR), user trust, market reach, robustness.
* **Key Strategies:** Data auditing & rebalancing; fairness-aware objectives; controlled exploration (bandits); post-hoc score calibration; transparency & user control.

### AIOps Case Studies 📈

1. **Predictive CI/CD & Smart Rollbacks 🔄:**

   * Example: CircleCI ranks tests by failure risk; Harness auto-rollback on anomalies.
2. **Automated Canary Deployments & Resource Optimization 🚀:**

   * Example: Netflix’s AI-driven canary analysis and dynamic scaling.

---

## Part II: Practical Implementation 🛠️

### Task 1: AI-Powered Code Completion ✍️

* **Manual vs. AI:** Both implementations use `sorted()` with lambda keys for sorting student records by age, name, and grade.
* **Observations:** Identical performance (O(n log n)); AI code is more concise; manual code features more detailed docstrings.
* **Conclusion:** Choose the variant that balances readability and maintainability for your team.

### Task 2: Automated Testing with Katalon Studio ✅

* **Tool:** Katalon Studio v10.2.2 on Windows 10.
* **Workflows:** Valid and invalid login tests recorded via Web Recorder.
* **Outcomes:**

  * `TC_ValidLogin` passed in \~20.9s;
  * `TC_InvalidLogin` failed in \~16.8s.
* **Insights:** Self-healing locators and smart waits reduce flaky tests and maintenance.

### Task 3: Predictive Analytics for Resource Location 📊

* **Pipeline:**

  1. Image preprocessing (resize to 64×64×3, flatten).
  2. Train/Test split (80/20 stratified).
  3. Random Forest (100 trees).
* **Results:** 81.ic% accuracy; weighted F1 of 80.4%; minority-class recall of 52%.
* **Future Work:** CNN-based feature extraction, systematic hyperparameter tuning, data augmentation, fairness auditing with IBM AIF360.

---

## Part III: Ethical Considerations 🤝

* **Dataset Biases:** Class imbalance, demographic/acquisition bias, feature extraction bias.
* **Mitigation (IBM AIF360):** Bias metrics dashboards, pre-processing reweighting, adversarial debiasing, post-hoc calibration.

---

## Bonus: AI-Powered Code Review Coach Proposal 💡

* **Purpose:** Context-aware, real-time feedback in PR workflows.
* **Workflow:**

  1. Integrate with GitHub/GitLab.
  2. Analyze diffs against best practices & historical comments.
  3. Generate actionable suggestions & explanations.
  4. Interactive clarifications & pattern lookup.
  5. Continuous learning from accepted/rejected feedback.
* **Impact:** Improved code quality, faster onboarding, reduced reviewer fatigue, scalable knowledge sharing.

---

## Project Structure 📂

```
├── part1/                # Theoretical write-ups (PDFs, slides)
├── part2/                # Code and test scripts
│   ├── code_completion/
│   ├── katalon_tests/
│   └── predictive_model/
└── part3/                # Ethical reflection and fairness notebooks
README.md
```

---

## Getting Started 🏁

1. **Clone the repository**:

   ```bash
   git clone https://github.com/<your-org>/power-learn-ai-swe.git
   cd power-learn-ai-swe
   ```
2. **Install dependencies** (Python 3.8+):

   ```bash
   pip install -r part2/predictive_model/requirements.txt
   ```
3. **Run examples**:

   * Code completion scripts in `part2/code_completion`.
   * Katalon test suite in `part2/katalon_tests`.
   * Train predictive model:

     ```bash
     python part2/predictive_model/train.py
     ```

---

## License 📝

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

