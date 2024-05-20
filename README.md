# Queing_System
# Overview
This program analyzes a simple M/M/1 queuing system, providing metrics such as the length of the system, length of the queue, and the total wait time in the system and queue. It also calculates the probability of a specific number of people being in the system and the probability of having at least a certain number of people in the system.

# Features
* Calculate the probability of n people being in the system.
* Calculate the probability of having at least n people in the system.
* Display key metrics of the queuing system:
  - Length of the system
  - Length of the queue
  - Total wait time in the system
  - Total wait time in the queue

# Usage
1. Clone the repository or download the code.

2. Open a terminal or command prompt.

3. Navigate to the directory where the code is located.

4. Run the program using the following command:

   python queuing_system.py

5. Follow the prompts to enter the arrival rate and service rate.
  
6. Enter the number of people in the system to calculate the probability.

7. Enter the minimum number of people in the system to calculate the probability of having at least that many people.

8. View the system metrics.

   # Example
Welcome to the Queuing System Analysis Program!
Enter arrival rate per hour: 5
Enter service rate per hour: 10

The arrival rate is 5.00 per hour.
The service rate is 10.00 per hour.

Probability Calculation:
Enter the number of people in the system: 3
The probability of 3 people being in the system is: 0.1250

Probability of at least 'n' people in the system:
Enter the minimum number of people: 2
The probability of at least 2 people in the system is: 0.8750

System Metrics:
  Length of the System: 0.50
  Length of the Queue: 0.00
  Total Wait Time in the System: 0.10 hours
  Total Wait Time in the Queue: 0.00 hours

Rerun? (yes/no): no
Exiting the program. Goodbye!

# Code Explanation
  # QueuingSystem Class
The QueuingSystem class encapsulates the logic for calculating probabilities and system metrics. It contains the following methods:

  - __init__(self, arrival_rate: float, service_rate: float): Initializes the queuing system with the given arrival and service rates.
  - calculate_probability(self, num_people: int) -> float: Calculates the probability of num_people being in the system.
  - probability_at_least(self, min_people: int) -> float: Calculates the probability of having at least min_people in the system.
  - display_metrics(self) -> None: Calculates and displays the system metrics.
# Functions
  - get_positive_float(prompt: str) -> float: Prompts the user to enter a positive float and validates the input.
  - main(): The main function that runs the program, handles user interaction, and displays results.
