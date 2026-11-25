# Capstone Brainstorming - Group 104

Group member: Rafael Eskinazi (Z23346103). The final project is individual, so I did the brainstorming on my own.

## New App Ideas - List

1. **SnapSpend** - Take a picture of a receipt and the app reads the total and saves it as an expense. You see what you spent this month by category. I got the idea from expense apps I've worked on outside of class, where people take photos of receipts to get reimbursed.
2. **TripSplit** - Plan a group trip (flights, hotel, activities) and split the costs between friends, with a running balance of who owes who.
3. **StudySpot FAU** - Map of study spots on campus (library floors, labs, lounges). Students check in and say how full and how quiet it is, so others can see it in real time.
4. **PantryChef** - Add what you have in the fridge and the app suggests recipes using a recipe API. Also tracks expiration dates.
5. **GymBuddy** - Log workouts (exercise, sets, reps, weight) and see charts of your progress. Rest timer between sets.
6. **WordADay** - Learn a word a day in another language with flashcards, using the MyMemory API from Project 6 for translations and a daily notification.
7. **PetCare** - Reminders for pet food, walks, vet visits and medicine, shared between family members.
8. **LostAndFound Campus** - Post a photo and location of something you found on campus, or search for something you lost.

## Top 3 New App Ideas

1. SnapSpend
2. StudySpot FAU
3. TripSplit

## New App Ideas - Evaluate and Categorize

1. **SnapSpend**
   - **Description**: Personal expense tracker. The user takes a photo of a receipt, the app reads the total with on-device text recognition, and the user picks a category. Expenses are saved in Firebase and shown by month and by category.
   - **Category:** Finance / Productivity
   - **Mobile:** Uses the camera, on-device text recognition (Apple Vision) and location (where the purchase was made). Taking the photo right at the store is something you can only do well on a phone.
   - **Story:** Everybody loses receipts and doesn't know where their money went at the end of the month. "Snap it and forget it" is easy to explain to friends.
   - **Market:** Very large: students, people on a budget, freelancers and employees who need to keep receipts for reimbursement.
   - **Habit:** Used every time you buy something (several times a week), and you check the monthly total and the chart often.
   - **Scope:** Clear MVP: login, add expense with photo, list, detail, delete and a chart. Reading the total from the photo is the challenging part, but the user can always type it, so a stripped-down version still works. APIs: Firebase (Auth + Firestore) and Apple Vision, both free.

2. **StudySpot FAU**
   - **Description**: Campus map with study spots. Students check in to a spot and rate how busy and how quiet it is right now.
   - **Category:** Education / Social
   - **Mobile:** Maps, location and real time updates.
   - **Story:** Useful during finals week when the library is full. Clear value for FAU students.
   - **Market:** Small and specific (FAU students), but could work for any campus.
   - **Habit:** Used before going to study, a few times a week. Only works if many students check in.
   - **Scope:** Map and check-ins are doable, but the app is not useful without a lot of users, which is hard to show in a demo.

3. **TripSplit**
   - **Description**: Plan a trip with friends and split the costs.
   - **Category:** Travel
   - **Mobile:** Push notifications and photos of receipts, but most of it would work the same as a website.
   - **Story:** Everybody has had a trip where nobody knows who paid what.
   - **Market:** Large, but there are already very popular apps that do this (Splitwise).
   - **Habit:** Only used when there is a trip, a few times a year.
   - **Scope:** Group invites, balances between many people and currencies make it big for two sprints.

## Final Idea

**SnapSpend.** It scored best on Mobile (camera + text recognition + location), it is something I would use every week, and the scope fits two sprints: the MVP is clear and the text recognition can be improved in the second sprint without blocking the rest of the app. It also builds on what we learned in class: SwiftUI, Firebase Auth and Firestore from Lab 6 and Project 6, and networking.
