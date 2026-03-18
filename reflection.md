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
  - copilot at first, then used claude for fomatting and fixing more bugs that copilot was not able to fix
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
  - copilot suggested: "Ensure "Normal" has fewer guesses than "Easy", and "Hard" has the fewest."
  - Changing the guessing chance limit to a higher number (10) for easy and a lower nunmber for hard (5)
  - increasing number range for hard mode from a lower number to 500
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
  - the str part was a bug that wasn't identified at first so I was confused why the game wasn't working when I had already followed the fixes from the first few bug fixes from copilot 

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
  - I tested the game manually
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
  - when I played the game manually and cheked the secret number compared to the guess, the game was more accurate but sometimes it was still giving the wrong hints
- Did AI help you design or understand any tests? How?
  - yes, wrote tests for me to check if code working

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
  - Streamlit works differently from most frameworks since every time a user interacts with a widget (clicks a button, types in a field), the entire Python script re-runs. This means any variable you create gets thrown away and recreated on each run, so if you stored the secret number in a plain variable, you'd get a new random number on every click and the game would be impossible.
  - st.session_state is a dictionary that persists across these reruns, acting like a little save file that survives each script re-execution. 
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
  - reading the full call stack before accepting an AI suggestion so I can figure out what the goal AI is tryign to reach and whether it breaks other code
- What is one thing you would do differently next time you work with AI on a coding task?
  - using AI as a first draft and not a final draft
- In one or two sentences, describe how this project changed the way you think about AI generated code.
  - using AI ethically and responsibly to code projects is important since you have to verify that it is correct. To be able to verify, you really have to understand the code line by line to find the bugs AI misses or misinterprets.
