# FEKERNI

**FEKERNI** ("remind me" in Moroccan Arabic) is a medication reminder app for people with early-stage Alzheimer's and their caregivers. It was built for the CSC 3324 Software Engineering course.

**Live app:** https://sarabenslimane14.github.io/FEKERNI/

## What it does

**For the patient (Nora)**
- Shows today's medicines and the next reminder time.
- Gives a large, simple reminder with two buttons: **Done** and **Help**.
- Sends follow-up reminders if there is no answer, then alerts the caregiver.
- Shows a waiting screen between two medicines ("Nothing to do now").

**For the caregiver (Karim)**
- Sets up each medicine: name, type, instructions and time.
- Sets the waiting time between the first and second medicine.
- Receives **Normal** or **Urgent** alerts, and acknowledges them.
- Sees what happened: Done, Help, or no answer.

## How the reminders work

| Event | What happens |
|---|---|
| Scheduled time arrives | The reminder appears. |
| No answer | Follow-up every 30 seconds for 3 minutes. |
| Patient taps Done | Follow-ups stop. No alert is sent. |
| Patient taps Help | An urgent alert goes to the caregiver. |
| Still no answer after 3 minutes | An urgent alert goes to the caregiver. |
| Caregiver does not acknowledge in 2 minutes | The app calls the caregiver. |

The second medicine reminds only after the first one is confirmed, plus the waiting time the caregiver set.

## Languages

English, French and Moroccan Darija (right-to-left).

## Safety

FEKERNI does **not** give medical advice, recommend doses, or change schedules. It only shows what a caregiver or prescriber entered. The medicine names and times in the demo are samples, not prescriptions. Do not enter real patient data.

## Limits of this demo

- The clock is simulated so reminders can be tested in minutes.
- It does not send real push notifications or phone calls.
- Data is saved in your own browser only.
- It is a course project, not a medical product.

## Run it

Open the live link above, or open `index.html` in any modern browser. No install needed.

## Project

Course: CSC 3324-03, Software Engineering.
Team: FEKERNI team.
