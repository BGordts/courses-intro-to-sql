---
title: Introduction
description: >
  Get to know relational database management systems, and get to know the SELECT
  statement.

--- type:VideoExercise lang:r xp: skills: key:4c8a1ecacb
## What is an RDBMS? 
Explain the concept of a relational database, about SQL, and about queries. But why use SQL in the first place, and not R/Python/other data analysis languages? You want the computation to be on the database side. When you've got the exact information you need, you can start your analyses in the tool of choice. Also interesting for real time dashboarding/visualization. Be very clear about what SQL is, and what it is not. We won't talk about updating SQL, we're data scientist, not data engineers.
Give example database: use DESCRIBE and basic SELECT statement as a first reconnaissance.

*** =video_link

--- type:NormalExercise lang:r xp: skills: key:b9c57149c3
## A first date 
Use DESCRIBE to figure out the different tables in the database.

*** =instructions

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

```

*** =solution
```{r}

```

*** =sct
```{r}

```

--- type:NormalExercise lang:r xp: skills: key:be24790269
## Your first SQL query 
Very basic:
select a from x

*** =instructions

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

```

*** =solution
```{r}

```

*** =sct
```{r}

```

--- type:VideoExercise lang:r xp: skills: key:9fbbe50887
## SELECT 
How to select a column, multiple columns, all columns, and how to use aliases.
select a from x
select a, b from x
select * from x
select a as new_a, b as new_b from x
Also mention here that using SELECT or select does not matter. In general, SQL is not case-sensitive when it comes to keywords, but it does when it comes to table and column names! We will use uppercase, to separate the SQL reserverd words from column and table names.


*** =video_link

--- type:NormalExercise lang:r xp: skills: key:6d78b3f5d9
## Select all columns 
Use the * to select all columns at once

*** =instructions

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

```

*** =solution
```{r}

```

*** =sct
```{r}

```

--- type:NormalExercise lang:r xp: skills: key:11f67e4d31
## Select multiple columns 
Separate column names with commas to select multiple columns. The order matters!

*** =instructions

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

```

*** =solution
```{r}

```

*** =sct
```{r}

```

--- type:NormalExercise lang:r xp: skills: key:c40a8b9a7b
## Using aliases 
Use the 'as' thing to load in certain columns under certain aliases.

*** =instructions

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

```

*** =solution
```{r}

```

*** =sct
```{r}

```

--- type:VideoExercise lang:r xp: skills: key:65abca1ebb
## SELECT (2) 
COUNT, SUM, AVG, MIN, MAX, DISTINCT to get a first idea about aggregates of your data.

*** =video_link

--- type:NormalExercise lang:r xp: skills: key:ea6d2d5f9f
## COUNT 
SELECT COUNT(*) FROM posts (to count the total number of posts)

*** =instructions

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

```

*** =solution
```{r}

```

*** =sct
```{r}

```

--- type:NormalExercise lang:r xp: skills: key:1dfc842e29
## SUM and AVG 
SELECT AVG(age) FROM readers

*** =instructions

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

```

*** =solution
```{r}

```

*** =sct
```{r}

```

--- type:NormalExercise lang:r xp: skills: key:e2226785a6
## MIN and MAX 
SELECT MAX(published_at) FROM posts to get the most recent post that was launched

*** =instructions

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

```

*** =solution
```{r}

```

*** =sct
```{r}

```

--- type:NormalExercise lang:r xp: skills: key:72c34d0508
## DISTINCT 
Number of distinct users that read something:
SELECT COUNT(DISTINCT user_id) FROM reads

*** =instructions

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

```

*** =solution
```{r}

```

*** =sct
```{r}

```