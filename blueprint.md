# Carrot and Stick Game

## Overview
This is a web application game where the user gains or loses "LIFE" points by receiving "comfort" (Carrot) or "insults" (Stick). It's a simple, interactive game designed to simulate the ups and downs of motivation.

## Design and Features

### Style and Design
*   **Theme:** Clean, modern interface with a focus on typography and clear feedback.
*   **Colors:** Uses distinctive colors for actions (Green for Comfort, Red for Insult/Stick).
*   **Animation:** Features floating text animations for score changes (+1, -1).
*   **Responsiveness:** Fully responsive layout suitable for mobile and desktop.

### Features
*   **Life System:** Starts with 10 LIFE. Game Over at 0, Win at >20.
*   **Interaction:**
    *   **Comfort Button:** Decreases LIFE by 1, shows a comforting message.
    *   **Insult Button:** Increases LIFE by 1, shows an insulting (motivating) message.
*   **Comment System:** Users can leave comments which are stored locally.
    *   **Deletion:** Users can delete their own comments using a password set during creation.

## Current Task: Enhance Comment Deletion with Password

*   **Objective:** Secure the comment deletion feature so that only the author (or someone with the password) can delete a comment.
*   **Steps:**
    1.  **HTML (`index.html`):** Add a password input field to the comment submission form.
    2.  **CSS (`style.css`):** Style the password input to fit the existing form layout.
    3.  **JavaScript (`main.js`):** 
        *   Update `saveComment` to store the password.
        *   Update `deleteComment` to prompt the user for a password and verify it before deleting.
        *   Handle backward compatibility for comments without passwords (allow deletion or require a default).
