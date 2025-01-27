# Brian-Boosted Rapid In-silico AutoDock Navigator
## A GUI for Parallel Virtual Screening Based on AutoDock Vina

### Usage Instructions

This tool allows you to perform parallel virtual screening using AutoDock Vina with a graphical user interface (GUI) and You don't need to install any other software.

---

### Input Fields

1. **Receptor File**  
   Provide the file path to the receptor molecule in `.pdbqt` format.

2. **Ligand Folder**  
   Specify the folder containing all ligand files in `.pdbqt` format.

3. **Box Center (x, y, z)**  
   Define the coordinates of the center of the docking box:  
   - `x`: X-coordinate  
   - `y`: Y-coordinate  
   - `z`: Z-coordinate  

4. **Box Size (x, y, z)**  
   Define the dimensions of the docking box:  
   - `x`: Size along the X-axis  
   - `y`: Size along the Y-axis  
   - `z`: Size along the Z-axis  

5. **Number of Parallel Processes**  
   Specify the number of docking processes to run in parallel.

---

### Important Notes

- **Cores per Vina**: It is recommended to use the default value of `4`.  
- **Cores per Vina * Number of Processes ≤ Total CPU Cores**:  
  Ensure that the total CPU usage does not exceed the number of cores available on your computer.  
  - For example, if your computer has 16 CPU cores, you can set `Cores per Vina = 4` and `Number of Processes = 4` (4 × 4 = 16).  
- **Avoid Full CPU Usage**: It is recommended not to use all CPU cores to ensure system stability and responsiveness.  

---

### Example Configuration

| Field                  | Example Value          |
|------------------------|------------------------|
| Receptor File          | `receptor.pdbqt`      |
| Ligand Folder          | `./ligands/`          |
| Box Center (x, y, z)   | `10.0, 15.0, -5.0`    |
| Box Size (x, y, z)     | `20.0, 20.0, 20.0`    |
| Number of Parallel Processes | `4`              |

---

### Execution

Once all fields are filled, click the **Run** button to start the docking process.

---

### Tips for Optimization

- Experiment with the **Number of Parallel Processes** and **Cores per Vina** settings to optimize performance based on your system's resources.  
- Monitor your system's CPU usage during the run to ensure smooth operation.

---

Happy docking!






