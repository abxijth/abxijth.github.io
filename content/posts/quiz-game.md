---
title: "Building My First Quiz Game with an API"
date: 2025-09-03
categories: ["Python", "APIs", "Projects"]
draft: false
---

As part of the **AMFOSS Club Praveshan tasks**, today I built a **command-line quiz game** powered by the **Open Trivia Database API**. At first, it looked overwhelming (so many API parameters and JSON fields), but step by step, I made it work.  

I learned how to:  
- Fetch categories and questions dynamically from the API.  
- Parse tricky JSON fields like `question`, `correct_answer`, and `incorrect_answers`.  
- Add a **timer with threads**, so the quiz doesn’t freeze while waiting for input.  
- Use `os._exit(0)` at the end to cleanly exit the game when it’s done.  

One issue I ran into was the **countdown timer and user input clashing** — if you didn’t type an answer, the quiz would skip ahead without giving you space to respond. I solved this with **threading**, running the timer in the background while still letting the player type.  

I also wrote a **README** to document how I approached the problem, what I learned, how I tested the code, and even added notes for future improvements. It felt like my first proper “mini-project” instead of just practice code.  

⚡ Overall, I walked away with a stronger understanding of **threads, APIs, and handling user input in Python**. Seeing it all come together into a working quiz game was super satisfying, and I’m excited to keep pushing forward with more Praveshan tasks!  

