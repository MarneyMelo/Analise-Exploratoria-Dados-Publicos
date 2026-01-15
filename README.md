# Food Security and Homeless Population Analysis - BH

This project was developed as the final assignment for the **Introduction to Databases (2025/2)** course at UFMG.

The goal was to integrate and analyze public data about the homeless population in Belo Horizonte and the availability of food security facilities (community restaurants), identifying gaps in social assistance and demographic patterns.

---

## Objectives and Scope

The system connects data from homeless people (Cadastro Único), CRAS (Social Assistance Reference Centers), and community restaurants. The focus was to answer questions such as:

* What is the availability of restaurants for the homeless population in each administrative region?
* What is the profile of time spent on the streets (time vs. age)?
* Is there a correlation between race, education, and time on the streets?
* Is it viable to create policies for returning to home cities based on family ties?

---

## Methodology and Technologies

* **Database:** PostgreSQL
* **Modeling:** Entity-Relationship (ER) Model and normalized Relational Model
* **Spatial Integration:** Use of Spatial Join to link the geographic location of restaurants to the Administrative Regions of BH
* **ETL:** Data cleaning (sanitization), handling composite primary keys for CRAS with duplicate names, and importing via temporary tables

---

## Main Analysis Results

1. **Peripheral Deficit:** Regions like **Noroeste** and **Leste** have the highest "overload" (more homeless people per restaurant), showing an urgent need for public policies in these areas.
2. **Family Ties:** About **66%** of the residents have broken or fragile family ties, making "return-to-hometown" policies less effective without prior support.
3. **Age and Racial Profile:**
* Young people tend to have entered homelessness recently (less than 6 months), while the elderly show chronic situations.
* The black/mixed-race population on the streets has significantly lower education levels than the white population, showing structural barriers.

---

## Repository Structure

```text
/
├── database/
│   └── backup.sql       # Full database dump (PostgreSQL)
├── docs/
│   ├── Relatorio_pt1.pdf
│   ├── Relatorio_pt2.pdf
│   └── Apresentacao_Final.pdf
└── README.md

```

## Authors

  * **Marney Melo** - [MarneyMelo](https://github.com/MarneyMelo)
  * **Rafael Miranda** - [RRafaelMMiranda](https://github.com/RRafaelMMiranda)
  * **Theo Duarte** - [theolara272727](https://github.com/theolara272727)
  * **Victor Kaizer** - [KaizerBlank](https://github.com/KaizerBlank)
  * **Vinicius Rochar** - [vrrocha-scs](https://github.com/vrrocha-scs)
