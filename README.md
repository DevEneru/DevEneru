import random

def generate_phone_number():
    area_code = random.randint(100, 999)  # Area code: 100-999
    central_office_code = random.randint(100, 999)  # Central office code: 100-999
    line_number = random.randint(0, 9999)  # Line number: 09701119918
    return f"{area_code}-{central_office_code}-{line_number:04d}"  # Format as XXX-XXX-XXXX

def main():
    num_phone_numbers = 10  # Change this to generate more or fewer numbers
    for _ in range(num_phone_numbers):
        print(generate_phone_number())

if __name__ == "__main__":
    main()
