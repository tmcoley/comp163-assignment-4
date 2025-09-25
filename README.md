student_name = "Tyler Coley" # Replace with your actual name
current_gpa = 3.0 # Float between 1.0 - 4.0
study_hours = 38 #INteger (Ex. 25)
social_points = 50 # Integer (Ex. 50)
stress_level = 60 # Integer 0 - 10

print(f"Welcome, {student_name}!")
student = {"Full name":"Tyler Coley","Student email": "tmcoley@ncat.edu", "Hometown": "Oxford, NC","Graduation semester": "Spring 2026", "Major": "Computer Science"}



#Lists

current_courses = ["COMP 163", "MATH 150", "ENG 101", "HIS 105"]

completed_courses = ["Biology","Chemistry","Calculus","Spanish II","World History"]
credit_hours = [3,3, 3,3]
gpa_history = [3.2, 3.6, 3.4, 3.7]



#Tuples

emergency_contacts = ("Mom", "Hannah Smith", "704-555-0199")

home_address = ("456 Oak Street,", "Charlotte,", "NC 28202")

insta_info = ("Instagram", "@jordan_codes", "312")

twitter_info = ("Twitter", "@jordandev", "127")

birthday = ("Birthday", "5", "22", "2006")



#Sets

current_skills = {"Python basics", "HTML", "Problem solving", "Time management", "Photography"}

skills_to_learn = {"JavaScript", "Data structures", "Git", "Web design", "Public speaking"}

career_interest = {"Software development","Web development", "Data science", "Game development"}

hobbies = {"Gaming", "Photography", "Reading", "Soccer", "Music"}

entertainment_backlog = {"One Piece", "Barry", "Life", "Incantation", "Memento"}



#dictionary

current_courses_dict = {"COMP 163": 3, "MATH 150": 3, "ENG 101": 3, "HIS 105": 3}

current_courses_professors_dict =  {"COMP 163": "Prof. Rhodes", "MATH 150": "Dr. Lee", "ENG 101": "Dr. Martinez", "HIS 105": "Dr. Brown"}

course_rooms = {"COMP 163": "M-Eric 300", "MATH 150": "Marteena 201", "ENG 101": "Crosby 121", "HIS 105": "Crosby 210"}

monthly_budget_dict = {"Food": 450, "Entertainment": 200, "Books": 125, "Transportation":100}

study_hours_per_subj_dict = {"Programming":10, "Math":8, "English":4, "History":3}

contact_directory_dict = {"Mom": "704-555-0199", "Roommate": "336-555-7821","Academic Advisor": "336-334-5000"}



#Calulations

total_credits = sum(credit_hours)

total_current_courses = len(current_courses)

cummulative_gpa = sum(gpa_history) / len(gpa_history)

weekly_study_hours = sum(study_hours_per_subj_dict.values())

study_cost = monthly_budget_dict["Books"] / weekly_study_hours

skills_current_amount = len(current_skills)

skills_to_learn_amount = len(skills_to_learn)

monthly_budget = sum(monthly_budget_dict.values())

food_daily = monthly_budget_dict["Food"] / 30

annual_budget = monthly_budget * 12

amount_of_platforms = 2

follower_count = int(twitter_info[2]) + int(insta_info[2])

contacts_total = len(contact_directory_dict)

total_completed_courses = len(completed_courses)

total_hobbies = len(hobbies)

total_entertainment_backlog = len(entertainment_backlog)

academic_workload = total_credits + weekly_study_hours


print("================================================================")

print("              PERSONAL ACADEMIC & LIFE PORTFOLIO")

print("================================================================")

print("Student:", student["Full name"], "| Email:", student["Student email"])

print("From:", student["Hometown"], "| Graduating:", student["Graduation semester"])

print("Major:", student["Major"])

print("\n=== ACADEMIC PROFILE ===")

print("Current Semester:", total_credits, "credits across", total_current_courses, "courses")

print(f"Cumulative GPA: {cummulative_gpa:.2f}")

print("Weekly Study Time:", weekly_study_hours, "hours")

print(f"Academic Investment: ${study_cost:.1f} per study hour")

print("\nCurrent Courses:")

print("COMP 163 -",current_courses_dict["COMP 163"],"credits -",current_courses_professors_dict["COMP 163"],"-",course_rooms["COMP 163"])

print("MATH 150 -",current_courses_dict["MATH 150"],"credits -",current_courses_professors_dict["MATH 150"],"-",course_rooms["MATH 150"])

print("ENG 101 -",current_courses_dict["ENG 101"],"credits -",current_courses_professors_dict["ENG 101"],"-",course_rooms["ENG 101"])

print("HIS 105 -",current_courses_dict["HIS 105"],"credits -",current_courses_professors_dict["HIS 105"],"-",course_rooms["HIS 105"])

print("\n=== PERSONAL DEVELOPMENT ===")

print("Current Skills:", current_skills)

print("Learning Goals:", skills_to_learn)

print("Career Interests:", career_interest)

print("Skills Currently Have:", skills_current_amount)

print("Skills Want to Learn:", skills_to_learn_amount)

print("\n=== FINANCIAL OVERVIEW ===")

print(f"Monthly Budget: ${monthly_budget:.0f}")

print(f"Food: ${monthly_budget_dict["Food"]:.0f} (${food_daily:.1f}/day)")

print(f"Entertainment: ${monthly_budget_dict["Entertainment"]:.0f}")

print(f"Books: ${monthly_budget_dict["Books"]:.0f}")

print(f"Transportation: ${monthly_budget_dict["Transportation"]:.0f}")

print(f"Annual Projection: ${annual_budget:.0f}")

print("\n=== CONNECTIONS & CONTACTS ===")

print("Emergency Contact:",emergency_contacts[1],"(Mom) -", contact_directory_dict["Mom"])

print("Home Address:", home_address[0], home_address[1], home_address[2])

print("Social Media Presence:", follower_count,"followers across", amount_of_platforms, "platforms")

print("Key Contacts:", contacts_total, "people in directory")

print("\n=== LIFE STATISTICS ===")

print("Total Courses Completed:", total_completed_courses)

print("Current Academic Load:", academic_workload, "weekly commitments")

print("Entertainment Backlog:", total_entertainment_backlog, "items")

print("Current Hobbies:", total_hobbies, "activities")

print("================================================================")


