# 1. LIST
students = ["Rahul", "Priya", "Aman", "Neha"]
print("Original list:", students)
students.append("Rohit")
students.remove("Aman")
students.sort()
print("After append, remove and sort:", students)
print("First student:", students[0])
print("Number of students:", len(students))

# 2. TUPLE
student_marks = (85, 92, 67, 76, 55)
print("\nTuple:", student_marks)
print("First mark:", student_marks[0])
print("Highest mark:", max(student_marks))
print("Lowest mark:", min(student_marks))
print("Total marks:", sum(student_marks))

# 3. SET
marks_with_duplicates = {85, 92, 67, 76, 55, 85, 92}
print("\nUnique marks:", marks_with_duplicates)
set_a = {1, 2, 3, 4}
set_b = {3, 4, 5, 6}
print("Union:", set_a | set_b)
print("Intersection:", set_a & set_b)
print("Difference:", set_a - set_b)

# 4. DICTIONARY
student = {"name": "Abhishek", "course": "B.Tech CSE", "semester": 8, "marks": 82}
print("\nDictionary:", student)
print("Student name:", student["name"])
student["marks"] = 88
student["grade"] = "A"
student["city"] = "Fatehpur"
del student["city"]
print("Updated dictionary:", student)
print("Keys:", list(student.keys()))
print("Values:", list(student.values()))

# 5. PRACTICAL STUDENT DATA PROCESSING
student_records = [
    {"name": "Rahul", "marks": 85}, {"name": "Priya", "marks": 92},
    {"name": "Aman", "marks": 67}, {"name": "Neha", "marks": 76},
    {"name": "Rohit", "marks": 55}
]
print("\nStudent records with grades:")
for record in student_records:
    if record["marks"] >= 80:
        record["grade"] = "A"
    elif record["marks"] >= 60:
        record["grade"] = "B"
    else:
        record["grade"] = "C"
    print(record)

# 6. EMPLOYEE DATA
employees = {
    "E101": {"name": "Amit", "department": "IT", "salary": 65000},
    "E102": {"name": "Sneha", "department": "HR", "salary": 58000},
    "E103": {"name": "Karan", "department": "IT", "salary": 82000},
    "E104": {"name": "Pooja", "department": "Finance", "salary": 72000}
}
print("\nEmployees with salary >= 70000:")
for emp_id, data in employees.items():
    if data["salary"] >= 70000:
        print(emp_id, data)

# 7. COMPARISON TABLE
comparison = [
    ["List", "Ordered", "Mutable", "Duplicates allowed", "[]"],
    ["Tuple", "Ordered", "Immutable", "Duplicates allowed", "()"],
    ["Set", "Unordered", "Mutable", "Duplicates not allowed", "{}"],
    ["Dictionary", "Key-value mapping", "Mutable", "Keys unique", "{key: value}"]
]
print("\nComparison table:")
for row in comparison:
    print(row)

# 8. COMMON METHODS
numbers = [5, 2, 8, 1, 4]
numbers.append(10)
numbers.remove(2)
numbers.sort()
print("\nList methods result:", numbers)
data_set = {1, 2, 3}
data_set.add(4)
data_set.discard(2)
print("Set methods result:", data_set)
data_dict = {"name": "Abhishek", "skill": "Python"}
data_dict.update({"level": "Beginner"})
print("Dictionary methods result:", data_dict)
