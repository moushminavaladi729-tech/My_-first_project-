# My_-first_project- 
this is my first project 
# student_grade_calculator.py

def calculate_average(marks):
    return sum(marks) / len(marks)

def find_grade(avg):
    if avg >= 90:
        return "A"
    elif avg >= 75:
        return "B"
    elif avg >= 50:
        return "C"
    else:
        return "Fail"

def main():
    marks = []

    for i in range(5):
        mark = float(input(f"Enter mark {i+1}: "))
        marks.append(mark)

    avg = calculate_average(marks)
    grade = find_grade(avg)

    print(f"\nAverage Marks: {avg}")
    print(f"Grade: {grade}")

if __name__ == "__main__":
    main()
