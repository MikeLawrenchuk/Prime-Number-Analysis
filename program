# Function to read primes from a file
def read_primes_from_file(filename):
    with open(filename, 'r') as file:
        primes = [int(line.strip()) for line in file]
    return primes

# Function to find pairs of primes whose last digits multiply to a certain target
def find_prime_pairs(target_last_digit, primes):
    pairs = []
    for i in range(len(primes)):
        for j in range(i+1, len(primes)):
            # Convert primes to strings and get the last digits
            last_digit1 = int(str(primes[i])[-1:])
            last_digit2 = int(str(primes[j])[-1:])
            if last_digit1 * last_digit2 == target_last_digit:
                pairs.append((primes[i], primes[j]))
    return pairs

# Read primes from a file
filename = 'primes.txt'  # replace with your filename
primes = read_primes_from_file(filename)

# Find pairs of primes whose last digits multiply to 91
pairs = find_prime_pairs(91, primes)

# Print the pairs
for pair in pairs:
    print(pair)
