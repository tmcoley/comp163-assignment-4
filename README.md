student_name = "Tyler Coley"  # Replace with your actual name
current_gpa = 3.0  # Float between 1.0 - 4.0
study_hours = 38  # Integer
social_points = 50  # Integer
stress_level = 60  # Integer

print(f"Welcome, {student_name} College Life!")
print(f"Name: {student_name}")
print(f"GPA: {current_gpa}")
print(f"Study Hours: {study_hours}")
print(f"Stress Level: {stress_level}")

print("\nChoose your course load:")
print("A) Light (12 credits)")
print("B) Standard (15 credits)")
print("C) Heavy (18 credits)")

choice = input("Your choice: ")

if choice == "A":
    study_hours += 5
    stress_level -= 5
elif choice == "B":
    study_hours += 10
    stress_level += 5
elif choice == "C":
    if current_gpa >= 3.5:
        stress_level += 10
    else:
        study_hours += 8
        stress_level += 20
else:
    print("Invalid choice. Defaulting to Standard load.")
    study_hours += 10
    stress_level += 5

print(f"\nUpdated Stats: GPA: {current_gpa}, Study Hours: {study_hours}, Stress: {stress_level}")

# Define subject list
subjects = ["Programming", "Math", "History"]
subject = input(f"Choose a subject {subjects}: ")

if subject in subjects:
    if subject == "Programming" and current_gpa < 3.0:
        current_gpa += 0.3
        social_points -= 5
    elif subject in ["Math", "History"]:
        current_gpa += 0.1
        social_points -= 2

print(f"\nUpdated Stats: GPA: {current_gpa}, Social Points: {social_points}, Stress: {stress_level}")

# Final Semester Assessment
final_check = True
print("\nFinal Semester Assessment...")

if final_check:
    if type(current_gpa) is not float:
        ending = "Error: GPA type is incorrect!"
    else:
        if current_gpa >= 3.5 and stress_level < 60:
            ending = "You made Dean's List!"
        elif current_gpa >= 3.5 and stress_level >= 60:
            ending = "High GPA, but stressed out."
        elif current_gpa >= 2.0 or study_hours >= 25:
            if social_points > 0:
                ending = "You passed the semester successfully!"
            else:
                ending = "You passed, but neglected social life."
        else:
            ending = "You are on academic probation."
else:
    ending = "Final check skipped."
# AI helped me with the use of GIT
print(f"\nGame Over! {student_name}, here are your final stats:")
print(f"GPA: {current_gpa}")
print(f"Study Hours: {study_hours}")
print(f"Social Points: {social_points}")
print(f"Stress Level: {stress_level}")
print("Ending:", ending)
