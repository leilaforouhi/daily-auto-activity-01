import datetime
import random

messages = [
    "Keep going, you're improving every day!",
    "Small progress is still progress.",
    "Consistency beats intensity.",
    "Today is a great day to learn something new.",
    "One more step toward greatness!"
]

def create_daily_log():
    today = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
    message = random.choice(messages)
    log = f"[{today}] - {message}"
    return log

if __name__ == "__main__":
    print(create_daily_log())
