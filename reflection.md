# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
  - number guessing game 
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").
  - when guess a lower number that the secret number, the hint is wrong and tells you to go lower
  - when guess a higher number that the secret number, the hint is wrong and tells you to go higher
  - hard mode on the game difficulty makes it easier since it gives a smaller range
  - normal mode has more chances to guess than hard mode

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
  - copilot
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
  - copilot suggested: "Ensure "Normal" has fewer guesses than "Easy", and "Hard" has the fewest."
  - Changing the guessing chance limit to a higher number (10) for easy and a lower nunmber for hard (5)
  - increasing number range for hard mode from a lower number to 500
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
-   

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
