from datetime import datetime

def greet(name):
    """Print a personalized greeting based on the time of day."""
    hour = datetime.now().hour
    
    if hour < 12:
        time_of_day = "morning"
    elif hour < 18:
        time_of_day = "afternoon"
    else:
        time_of_day = "evening"
        
    print(f"Good {time_of_day}, {name}! Welcome to our program.")

# Example usage
greet("Alice")
