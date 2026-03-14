# Math-quantam-sensor
A math steam task about quantam sensor
import random

# probability that the quantum sensor detects a signal
probability = 0.65

detections = 0
trials = 100

for i in range(trials):
    measurement = random.random()  # random number between 0 and 1

    if measurement < probability:
        detections += 1

print("Total measurements:", trials)
print("Signal detected:", detections)
print("Detection rate:", detections / trials)
