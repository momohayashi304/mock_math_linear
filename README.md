# Lesson Plans: Mock Lessons for the "Teaching Methods for Mathematics Teachers 1" (数学科指導法１) Course

This repository contains the lesson plan overviews and interactive web simulators for **two** mock lessons designed for the 数学科指導法１ (Teaching Methods for Mathematics Teachers 1) course.

Open [`lesson.html`](./lesson.html) and use the **top tabs** to switch between the two units:

| Tab | Unit | Target Grade |
|---|---|---|
| 一次関数（中2） | Linear Functions — *regarding relationships as linear functions* | Junior High School 2nd Year |
| 平方根（中3） | Square Roots — *multiplication of expressions containing radicals* | Junior High School 3rd Year |

### Standalone pages & QR codes

Each unit also has a standalone page so students can scan a QR code on a tablet/phone and jump directly into the simulator without the tab switcher:

- [`linear.html`](./linear.html) — 一次関数 simulator only (standalone)
- [`sqrt.html`](./sqrt.html) — 平方根 simulator only (standalone)
- [`qr.html`](./qr.html) — displays **two QR codes**, one for `linear.html` and one for `sqrt.html`, generated client-side from the page's own URL. Open this on the projector/teacher screen; students scan whichever QR matches the unit they need.

> The QR codes are generated dynamically from `window.location`, so they automatically point at the correct host (e.g. GitHub Pages, local file, intranet server) wherever `qr.html` is served from.

---

## Unit 1: Linear Functions (一次関数)

### Overview
- **Subject:** Mathematics
- **Target Grade:** Junior High School 2nd Year (8th Grade equivalent)
- **Unit:** Chapter 3: Linear Functions (Tokyo Shoseki p.85)
- **Section:** Application of Linear Functions (Regarding relationships as linear functions)

### 1. Unit Concept & Value (単元観)
This unit builds upon the concepts of proportional and inversely proportional relationships learned in the first year. The primary goal is to deepen students' understanding of linear functions, particularly focusing on the rate of change and the characteristics of their graphs.

In the real world, the relationship between two quantities does not always change perfectly uniformly. However, by focusing on a set of observed data and **"regarding it as a linear function" (idealising and abstracting the phenomenon)**, it becomes possible to predict unknown values and analyse overall trends.

Through activities that mathematically model specific phenomena—such as weather data—students will experience the process of problem-solving. This will help them understand how mathematics is utilised in society and realise the practical utility of functional thinking.

### 2. Student Profile (生徒の実態)
A common characteristic among the students in this class is that while they are relatively proficient in mechanical calculation processes (such as solving equations), many struggle to interpret the meaning behind their calculation results or to connect mathematical concepts with real-world phenomena.

### 3. Learning Goals (学習目標)
Based on the Japanese Course of Study (学習指導要領), this lesson focuses on the following evaluation criteria:

* **Knowledge & Skills:** Understand that certain real-world phenomena can be modelled as linear functions, and express these relationships using tables, equations ($y = ax + b$), and graphs.
* **Thinking, Judging, & Expressing:** Regard the relationship between two quantities in a specific phenomenon (e.g., elevation and temperature) as a linear function, predict unknown values based on this assumption, and logically explain the problem-solving method to others.
* **Attitude:** Reflect on the problem-solving process using linear functions, and actively try to apply mathematical thinking to daily life and future learning.

### 4. Instructional Strategies (指導の手立て)
1. **Contextualised Problem Solving:** Instead of abstract math problems, the lesson uses highly relatable scenarios such as predicting the temperature at the summit of Mt. Fuji based on the elevation-temperature rule, or analysing the length of a burning incense stick over time.
2. **ICT Integration (Interactive Web Simulator):** Students manipulate sliders for the slope ($a$) and y-intercept ($b$) to manually fit a straight line to scattered experimental data points. This dynamic, hands-on activity bridges the gap between raw data and the formula $y = ax + b$.
3. **Collaborative Learning (Pair Work):** Students explain *why* they chose a specific slope and intercept and *how* they predicted the unknown future value, ensuring they are not just calculating but truly understanding the mathematical model.

---

## Unit 2: Square Roots (平方根)

### Overview
- **Subject:** Mathematics
- **Target Grade:** Junior High School 3rd Year (9th Grade equivalent)
- **Unit:** Chapter 2: Square Roots
- **Section:** Multiplication of Expressions Containing Radicals (Discovery through Geometric Figures)

### 1. Unit Concept & Value (単元観)
Rather than treating the multiplication of square roots simply as a mechanical algebraic rule to memorise, this unit aims to have students discover the mathematical laws through a geometric perspective, much like ancient Greek mathematicians who equated multiplication with finding the area of a rectangle.

By visualising numerical values as lengths, it provides a strong foundation that prevents common misconceptions in later lessons (such as confusing the rules of multiplication with those of addition). Transitioning from sensory puzzle activities (intuitive geometry) to formal algebraic proofs allows students to experience the beauty of mathematical generalisation and appreciate the logical expansion of the number system.

### 2. Student Profile (生徒の実態)
A common characteristic among the students in this class is that while they are generally enthusiastic and proficient in calculation processes, some struggle to interpret the true meaning behind the operations or to connect new ideas with previously learned concepts (such as the definition of a square root).

Therefore, before introducing operational rules, the lesson incorporates activities that link the abstract concept of square roots to concrete visual representations, such as finding the side length of a square from its known area.

### 3. Learning Goals (学習目標)
Based on the Japanese Course of Study, this lesson focuses on the following evaluation criteria:

* **Knowledge & Skills:** Understand the rules for multiplying numbers with radical signs and be able to perform these calculations efficiently.
* **Thinking, Judging, & Expressing:** Investigate the mechanism and validity of the multiplication rule ($\sqrt{a} \times \sqrt{b} = \sqrt{ab}$) based on specific numbers, approximations, and geometric area expansion, and logically explain the reasoning to others.
* **Attitude:** Proactively attempt to find the rules for calculating with square roots by utilising figures and previously learned mathematical definitions, appreciating the consistency of mathematical laws.

### 4. Instructional Strategies (指導の手立て)
* **Geometric Approach for Conceptual Understanding:** Instead of jumping straight into algebraic formulas, the lesson introduces the historical view of "multiplication = area of a rectangle." Students use a "rectangle expansion puzzle" to visually deduce that if a rectangle with an unknown area $S$ is scaled by $\sqrt{2}$ vertically and $\sqrt{3}$ horizontally, the new area becomes $6$. Since the area is multiplied by $S$, they derive $S^2 = 6$, leading to the natural conclusion that the original area $S$ is $\sqrt{6}$.
* **ICT Integration (Interactive Web Simulator):** Students use a custom-built, interactive HTML/JS simulator distributed via LoiLoNote on their tablets. By manipulating independent sliders for the vertical and horizontal scale factors, they can visually and dynamically experiment with how the area changes. The simulator provides real-time feedback, highlighting when the resulting area becomes a perfect integer, bridging the gap between raw experimental data and the mathematical formula.
* **Collaborative Learning and Rigorous Proof:** Students engage in pair work to articulate *why* the area changes using the concept of scaling factors. Following the visual and empirical conviction, the lesson guides them through a formal algebraic proof using the definition of square roots. Crucially, students explicitly verify the positive and negative signs (since length and area must strictly be positive) to ensure the logical completeness of their proof.

---

## Files

- `lesson.html` — combined interactive simulator (top tabs: 一次関数 / 平方根)
- `linear.html` — standalone 一次関数 simulator (QR code target)
- `sqrt.html` — standalone 平方根 simulator (QR code target)
- `qr.html` — QR code landing page with one QR per unit
- `index.html`, `index2.html` — 3D map visualisations of Mt. Fuji observation stations (used in the 一次関数 lesson)
- `README.md` — this file
