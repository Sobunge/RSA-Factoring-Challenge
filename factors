import sys

def factorize(number):
    factors = []
    for i in range(2, number // 2 + 1):
        if number % i == 0:
            factors.append((i, number // i))
    return factors

def main(file_path):
    with open(file_path, 'r') as file:
        numbers = [int(line.strip()) for line in file]

    for number in numbers:
        factorizations = factorize(number)
        for factorization in factorizations:
            print(f'{number}={factorization[0]}*{factorization[1]}')

if __name__ == "__main__":
    if len(sys.argv) != 2:
        print("Usage: factors <file>")
        sys.exit(1)

    file_path = sys.argv[1]
    main(file_path)
