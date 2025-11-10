import matplotlib.pyplot as plt
import numpy as np

# Years and data (approximate estimates in ₹ crore)
years = ["2019-20", "2020-21", "2021-22", "2022-23", "2023-24", "2024-25"]
lpg_subsidy = [32000, 38000, 19000, 6000, 12000, 14500]      # Govt expenditure on LPG subsidy
percent_subsidy = [80, 90, 50, 15, 35, 40]                   # % of subsidy distributed

x = np.arange(len(years))

# Create chart
fig, ax1 = plt.subplots(figsize=(9,6))

# Bar chart for LPG subsidy
ax1.bar(x, lpg_subsidy, color='skyblue', label='LPG subsidy (₹ crore)')
ax1.set_xlabel('Financial Year')
ax1.set_ylabel('LPG Subsidy (₹ crore)', color='blue')
ax1.tick_params(axis='y', labelcolor='blue')

# Title and x-axis formatting
ax1.set_title('LPG Subsidy Over the Years (2019–20 to 2024–25)')
ax1.set_xticks(x)
ax1.set_xticklabels(years)

# Line chart for % subsidy
ax2 = ax1.twinx()
ax2.plot(x, percent_subsidy, color='orange', marker='o', label='% LPG Subsidy')
ax2.set_ylabel('% LPG Subsidy', color='orange')
ax2.tick_params(axis='y', labelcolor='orange')

# Legend and grid
lines, labels = ax1.get_legend_handles_labels()
lines2, labels2 = ax2.get_legend_handles_labels()
ax1.legend(lines + lines2, labels + labels2, loc='upper left')

plt.grid(axis='y', linestyle='--', alpha=0.5)
plt.tight_layout()
plt.show()
