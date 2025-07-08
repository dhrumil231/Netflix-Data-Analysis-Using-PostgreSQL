# Netflix-Data-Analysis Movies and TVShows -Using-PostgreSQL

![NetFlix Logo](https://github.com/dhrumil231/Netflix-Data-Analysis-Using-PostgreSQL/blob/main/Netflix_Logo.png) 

🧾 Overview
This project explores and analyzes Netflix’s content catalog using advanced SQL techniques. The primary goal is to extract actionable insights about the type, origin, genre, and release patterns of content available on Netflix. Through this analysis, we address real-world business questions that can aid in making data-informed content strategy decisions.

🎯 Objective
Understand the distribution of Movies vs. TV Shows.
Identify top countries, genres, and creators contributing to Netflix's content.
Extract trends in content additions over time.
Uncover hidden insights like most active actors, content without directors, and keyword-based classifications.
Demonstrate SQL skills in data transformation, aggregation, filtering, joins, string manipulation, and date processing.

🧮 Dataset Used
Source: Netflix content dataset (imported into PostgreSQL)
Format: SQL script (.sql) containing CREATE TABLE and analysis queries
Records: 8,000+ titles from Netflix
Fields:
show_id: Unique ID of the show
type: Movie or TV Show
title: Title of the content
director: Director's name
casts: Cast members
country: Country of origin
date_added: Date the content was added to Netflix
release_year: Year of original release
rating: Age rating (TV-MA, PG, etc.)
duration: Runtime or number of seasons
listed_in: Genre(s)
description: Summary of the title

🗂️ Database Schema
CREATE TABLE netflix (
  show_id     VARCHAR(6),
  type        VARCHAR(10),
  title       VARCHAR(150),
  director    VARCHAR(208),
  casts       VARCHAR(1000),
  country     VARCHAR(150),
  date_added  VARCHAR(50),
  release_year INT,
  rating      VARCHAR(10),
  duration    VARCHAR(15),
  listed_in   VARCHAR(100),
  description VARCHAR(250)
);

❓ Business Questions Answered
1) What is the count of Movies vs. TV Shows on Netflix?
2) What are the most common ratings for Movies and TV Shows?
3) List all movies released in a particular year (e.g., 2020).
4) Which 5 countries produce the most Netflix content?
5) What is the longest-duration movie available?
6) What content was added in the last 5 years?
7) Which shows or movies are directed by Rajiv Chilaka?
8) Which TV shows have more than 5 seasons?
9) What is the distribution of content by genre?
10) What are the top 5 years for Netflix content releases in India?
11) Which titles are listed as Documentaries?
12) What content has no director listed?
13) In how many movies has Salman Khan appeared in the last 10 years?
14) Who are the top 10 actors in Indian Netflix content?
15) Categorize content as “Good” or “Bad” based on keywords like "kill" or "violence" in descriptions.

🛠 Tools & Technologies
PostgreSQL
SQL (Window functions, CTEs, UNNEST, ILIKE, TO_DATE, RANK, etc.)
Data Cleaning & Transformation
Query Optimization
