# Advanced Styling and Javascript

A single-page project that demonstrates:

Responsive layouts with CSS Grid and media queries

An interactive JavaScript quiz (multiple choice + scoring)

An image carousel (auto-rotate + manual controls)

Fetching and displaying live data from a public API (random jokes)

This repository contains a compact, easy-to-follow example for learners to experiment with modern front-end fundamentals.

# Project Overview

This is a single HTML file that combines CSS and JavaScript to deliver three learning tasks in one place:

Task 1: Responsive cards layout using CSS Grid + media queries

Task 2: Two interactive components — a quiz and an image carousel

Task 3: Fetch data from a public API and render it dynamically

The goal is to provide a compact lab project students can open in a browser, read, and extend.

# Tech Stack

HTML5

CSS3 (Grid, media queries)

Vanilla JavaScript (DOM API, events, Fetch API)

# Step-by-Step Procedure

## Step 1: Create the single-page HTML file

Created advanced_styling_js_project.html.

Added the base HTML skeleton:

        <!DOCTYPE html>
        <html lang="en">
        <head>
          <meta charset="utf-8" />
          <meta name="viewport" content="width=device-width,initial-scale=1" />
          <title>Advanced Styling and JavaScript Project</title>
        </head>
        <body>
          <!-- sections here -->
        </body>
        </html>

Save and open in your browser to verify the page loads.

## Step 2: Build Responsive Layout

In the same file, added a header, nav, and a .grid-container with three .card elements.

Add CSS: grid-template-columns for desktop and two media queries:

@media (max-width: 768px) → 2 columns

@media (max-width: 480px) → 1 column

## Step 3: Add Interactive Quiz

Added a section#quiz containing placeholders for question, options, and result.

In a <script> block, define quizData (array of objects), loadQuiz() and checkAnswer() functions.

Wire up buttons dynamically and test by answering questions.

## Step 4: Add Image Carousel 

Add section#carousel with an <img id="carousel-img"> and Prev/Next buttons.

In JavaScript, create an images array, showImage(), nextImage(), prevImage() and a setInterval() for auto-rotation.

Test manual buttons and auto-rotate.

## Step 5: Fetch Data from Public API

Added section#api-section with a div#joke and a Get Joke button.

Implemented async function getJoke() using fetch('https://official-joke-api.appspot.com/random_joke').

Parsed JSON and display setup and punchline.

Test while online.

## Step 6: Add Navigation

Add a nav with buttons that call a small showSection(id) function that toggles .active on sections.

Ensure one section (e.g., #responsive) is visible by default.

## Step 7: Styling polish

Add niceties: header colors, button styles, card shadow, border-radius, spacing.

Double-check styles in mobile emulator.

## Step 8: Commit & push
git add .
git commit -m "chore: initial project with responsive layout, quiz, carousel, and API fetch"
git push origin main

Opened the html file in any modern browser (Chrome, Firefox).
