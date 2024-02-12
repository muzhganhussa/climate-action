# climate-action
import matplotlib.pyplot as plt

# Initial values
temperature = 15  # Initial temperature in Celsius
years = 50  # Number of years to simulate
temperature_increase_per_year = 0.02  # Temperature increase per year in Celsius

# Lists to store data for plotting
year_data = []
temperature_data = []

# Simulate climate change
for year in range(years):
    temperature += temperature_increase_per_year
    year_data.append(year)
    temperature_data.append(temperature)

# Plotting the data
plt.plot(year_data, temperature_data, color='red')
plt.title('Climate Change Simulation')
plt.xlabel('Years')
plt.ylabel('Temperature (Celsius)')
plt.grid(True)
plt.show()
