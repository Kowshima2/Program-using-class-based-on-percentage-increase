# Program-using-class-based-on-percentage-increase
class PercentageIncrease:
    def __init__(self, initial_value):
        self.initial_value = initial_value

    def calculate_increase(self, new_value):
        # Calculate the increase from the initial value
        increase = new_value - self.initial_value
        # Calculate the percentage increase
        percentage_increase = (increase / self.initial_value) * 100
        return percentage_increase

    def display_increase(self, new_value):
        # Get the percentage increase
        increase = self.calculate_increase(new_value)
        print(f"Initial Value: {self.initial_value}")
        print(f"New Value: {new_value}")
        print(f"Percentage Increase: {increase:.2f}%")

# Example usage:
# Initialize the class with an initial value
initial_value = float(input("Enter the initial value: "))
new_value = float(input("Enter the new value: "))

# Create an instance of the PercentageIncrease class
increase_calculator = PercentageIncrease(initial_value)

# Display the result
increase_calculator.display_increase(new_value)

Output 
Enter the initial value: 50
Enter the new value: 75
Initial Value: 50.0
New Value: 75.0
Percentage Increase: 50.00%
