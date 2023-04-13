# ====== LIBRARIES ====== #
import matplotlib.pyplot as plt                                                                       # Imports matplot library and renames to plt (great for plotting)
import numpy as np                                                                                    # Imports numpy (great for large data arrays)

# ===== MAIN BODY OF CODE ===== #
data = np.loadtxt(fname = "Runtime_20min Avpower_70w.txt", skiprows = 32, delimiter = ';')            # Locates file, ignores first 32 rows, sets ; as delimeter
Sample_points = np.array(data[:,0])                                                                   # Creates array of sample points from column
Phase_data = np.array(data[:,12])                                                                     # Creates array of phase data from column
plt.plot([Sample_points], [Phase_data], marker=".", markersize=1, c='b')                              # Plots x = sample points, y = phase
plt.suptitle('Pre-Amplifier Benchtest (Phase Against Time)')
plt.xlabel('Sample number in seconds (s)')
plt.ylabel('Phase ($^\circ$)')
plt.grid()
plt.show()


# ISSUES - Requires matplotlib as a python interpreter and in this code the project was placed in the same repository as the txt files.
