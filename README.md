# Project 3 for CSE321, Fall 2022
Repository for files related to Project3 of CSE321, Fall 2022
<b>Explanation</b>
The traffic light, when triggered, will follow this sequence:
  1. Light1 starts as Green, Light2 starts as Red
  2. If motion sensor timer has not reached 0: <br>
  a. Light1 turns yellow at 0 seconds <br>
  b. Light1 turns red at 15 seconds <br>
  c. Light2 turns green at 60 seconds <br>
  d. Buzzer sounds at 60 seconds <br>
  e. Light2 turns yellow at 105 seconds <br>
  f. Light2 turns red at 120 seconds <br>
  g. Light1 turns green at 165 seconds <br>
  h. Buzzer sounds at 165 seconds <br>
  i. Return to step 2
  3. If IR sensor timer has reached 0: <br>
  a. Wait for motion sensor to trigger <br>
  b. Return to step 2

# Project Overview
The circuit I am designing is meant to simulate a traffic light at an intersection. The light includes 3 sensors, one for weather, one for counting the number of cars at the intersection, and a master enabling sensor. If the weather sensor detects snow, it will turn on. The weather sensor turning on will turn off the counting sensor. The counting sensor turning off will also turn off the enabling sensor. The lights on either road cannot both be green at the same time, but they can both be red at the same time. In fact, between each transition of the lights' colors, they must both be red for a short time.

