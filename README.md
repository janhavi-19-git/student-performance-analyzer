# student-performance-analyzer
A Beginneer python project that analyses student academic performance.

students = [
    {
        "name": "Ananya",
        "math": 85,
        "python": 90,
        "english": 78,
        "attendance": 92
    },
    {
        "name": "Riya",
        "math": 72,
        "python": 80,
        "english": 88,
        "attendance": 85
    },
    {
        "name": "Rahul",
        "math": 95,
        "python": 91,
        "english": 90,
        "attendance": 97
    },
    {
        "name": "Aisha",
        "math": 65,
        "python": 70,
        "english": 75,
        "attendance": 78
    }
]


INDEX.HTML
# Calculate average marks for each student

for student in students:

    total = (
        student["math"]
        + student["python"]
        + student["english"]
    )

    average = total / 3

    student["average"] = average


# Display student results

print("===================================")
print("     STUDENT PERFORMANCE ANALYZER")
print("===================================")

for student in students:

    print(
        student["name"],
        "- Average:",
        round(student["average"], 2)
    )
