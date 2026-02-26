# SDLC Capstone — Sprint 1 Process Analysis

**Course:** Software Quality Assurance  
**Sprint:** Sprint 1  
**Model Selected:** Waterfall  
**Submission Type:** Solo  
**Due:** End of class Thursday

---

## Section 1 — Model Selection and Rationale

**Selected Model:** Waterfall  

**Rationale:**  
Sprint 1 mostly followed the Waterfall model because we worked step by step. First, we made a spec for our Python Tamagotchi game, planning all the main features like **eat, sleep, play, and evolve**.

Then we built the game based on that plan. Most of the bugs, like the “Play” command increasing hunger and the evolution status showing too early, were found during the Week 6 swap after we finished coding.

Any changes we made after testing were part of maintenance. Even though we had a retrospective and small feedback, the project basically went in order: **plan → build → test → fix**, which is what Waterfall is all about.

---

## Section 2 — Phase Analysis

### Phase: Requirements
**What Sprint 1 produced:**  
We created a one-page spec before starting development. It listed all the main features of our Python Tamagotchi game, including eat, sleep, play, and evolve.

**What strict adherence would have looked like:**  
Under strict Waterfall, the requirements would have been more detailed and formally approved before moving on. After sign-off, no changes would be allowed without a formal change request.

### Phase: Design
**What Sprint 1 produced:**  
We planned how the stats would work and how the functions would connect in Python. However, not everything was fully documented before coding.

**What strict adherence would have looked like:**  
All game logic, stat rules, and technical structure would have been completely documented before writing any code.

### Phase: Implementation
**What Sprint 1 produced:**  
We built the game based on our spec and added working functions for eat, sleep, play, and evolve. Most features were finished before formal testing.

**What strict adherence would have looked like:**  
Developers would only build exactly what was written in the design, with no feature changes or adjustments during development.

### Phase: Testing
**What Sprint 1 produced:**  
QA mainly happened during the Week 6 swap. Classmates tested the finished game and created GitHub Issues for bugs like the “Play” command increasing hunger and the incorrect evolution status.

**What strict adherence would have looked like:**  
QA would receive the fully completed system and test it against the original requirements using a formal test plan. Testing would only happen after development was completely finished.

### Phase: Deployment
**What Sprint 1 produced:**  
The deployment and testing happened in the same phase. We let out our game to the other class, and they tested it.

**What strict adherence would have looked like:**  
The final, fully tested version would only be released after passing all QA checks and formal approval.

### Phase: Maintenance
**What Sprint 1 produced:**  
After testing, we fixed the reported bugs and made some feature updates since we had extra time.

**What strict adherence would have looked like:**  
Maintenance would mainly focus on fixing defects found in testing. Major feature changes would likely require starting a new development cycle.

---

## Section 3 — Defect Case Studies

### Bug 1
**GitHub Issue:** [Play command bug](https://github.com/Gcc07/GroupSprint-QA/issues/5)  

**Description:**  
When the player used the “Play” command, the Spirit’s hunger stat increased instead of increasing the happiness stat. This made it impossible to increase the happiness stat without the Spirit dying of hunger.  

**Phase that introduced the defect:** Implementation. The error happened when writing the stat logic for the Play function.  

**Phase that caught it:** Testing. It was discovered during the Week 6 swap when classmates tested the finished game and created GitHub Issues.  

**Would your chosen model have caught it earlier?**  
Under strict Waterfall, it likely would not have been caught earlier because testing happens after development. However, better design review or clearer stat rules might have reduced the chance of this mistake.  

**Cost of catching it late:**  
The cost was moderate. We had to go back into the code, fix the stat logic, and retest the feature to make sure it worked correctly and didn’t affect other stats.  

### Bug 2
**GitHub Issue:** [Evolution status bug](https://github.com/Gcc07/GroupSprint-QA/issues/4)  

**Description:**  
The status screen showed that the Spirit was ready to evolve even when its stats were not high enough. This gave players incorrect information and broke the progression system.  

**Phase that introduced the defect:** Implementation. The conditional logic checking stat requirements was written incorrectly.  

**Phase that caught it:** Testing. It was found during the Week 6 swap when QA tested evolution conditions.  

**Would your chosen model have caught it earlier?**  
In strict Waterfall, it still would have been caught in the testing phase. Since testing comes after development, this type of logic bug would likely not be found earlier.  

**Cost of catching it late:**  
The cost was moderate. The evolution conditions had to be corrected and tested again to make sure the system worked properly and did not allow false evolution messages.  

---

## Section 4 — QA Assessment

**How QA actually operated:**  
During Sprint 1, QA mostly acted as a gate at the end of development. We built the full Tamagotchi game first, and testing mainly happened during the Week 6 swap. That is when classmates played the game and created GitHub Issues for bugs. We did some small testing while coding, but most problems were found after the game was finished.

**How that compares to your chosen model:**  
This matches the Waterfall model because Waterfall has a separate testing phase after implementation. In our project, QA did not continuously test during development. Instead, testing happened mostly after the main features were complete.

**What QA would have looked like under strict adherence:**  
Under strict Waterfall, QA follows a formal and structured process. The team creates written test cases based on the original requirements document. QA tests every feature against the approved specification to confirm it meets the defined criteria. The team blocks new features during this phase and allows only documented bug fixes. Deployment occurs after QA verifies that all requirements are satisfied.

---

## Section 5 — Team Retrospective on Process

**The gap:**  
The biggest gap between our Sprint 1 process and strict Waterfall was that we made major feature changes after testing. In strict Waterfall, once the team finishes and signs off on requirements, the team does not change or add features without starting a new cycle. We adjusted and improved features after the swap instead of limiting changes to bug fixes.

**What it cost the team:**  
This decision created extra work and confusion. The team modified code that QA had already tested. The change blurred the line between development, testing, and maintenance. The process no longer followed a clear sequence. The team blended phases together at the end.

**The one change for Sprint 2:**  
If we ran Sprint 2 under strict Waterfall, the most important change would be locking requirements before development begins. Once coding starts, the team would fix only bugs during testing and move new feature ideas to the next cycle. This structure would keep phases organized and clearly separated.

---

## Contributors

| Name           | Section Led        |
|----------------|------------------|
| Masoud Moawiye | All Sections (1–5) |
