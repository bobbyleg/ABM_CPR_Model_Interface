# Agent-Based Common Pool Resource Model GUI

Welcome to the Agent-Based Common Pool Resource (CPR) model graphical user interface (GUI)! This graphical user interface allows users to interact with and explore the results of an agent-based model that investigates the dynamics of social networks in common pool resource environments.

## Abstract

The study reveals that network structures, particularly skewed degree distributions, lead to multiple possible CPR outcomes, corresponding to alternative stable states for the same conditions. A key finding is the substantial influence of hub agents in shaping network perceptions and decisions, creating phenomena like majority illusions that significantly affect resource states and sustainability. As inequality of impacts rises, this effect disappears, but access to a state with higher welfare also disappears. These findings highlight the critical role of network hubs in CPR dynamics, offering new directions for effective management and policy-making.

The paper can be found at https://github.com/bobbyleg/Centrality_and_environmental_impact/tree/main.

## How to Use the GUI

### Running Python Code for Non-Experts

To run the code files, clone the repository. Downloading all the files (including the gui_plots folder) separately is possible as well, as long as the user saves all files  in same folder on their computer. All files, except the images contained in the gui_plots folder, are .ipynb files, meaning that they are Jupyter Notebooks. To run them, the user needs a compatible code editor, such as Visual Studio Code or Jupyter. 

Moreover, the user requires a few Python libraries (see requirements). Downloading Anaconda is recommended for access to most of these libraries. Users must download CustomerTkinter and pillow themselves. These libraries are easily installed through the terminal using: `pip3 install customtkinter` and `pip install pillow`.

### Running the GUI

To access the graphical user interface, open the gui.ipynb file and run all cells in order. The GUI provides an abstract of the paper on the left. In the upper half of the GUI, four tabs explain the model parameters and give access to the three different output plots. The user can also select which of the output plots to create. The default setting creates all three. The bottom row contains five tabs that let the user set the model parameters. 

### 1. General Tab
-	Simulations: Number of model runs.
-	Generations: Number of generations in each run.
-	Agents: Number of agents in the model.
-	ε : Relative speed of strategic and environmental dynamics.

### 2. Initialization Tab
-	Resource: initial value of the environment.
-	Low effort fraction: fraction of agents initially extracting with low effort.

### 3. Incentives Tab
-	&alpha;: base difference between extracting with high or low effort
-	The difference &gamma;1h-&gamma;1l: governs whether agents want to go with or against the majority.
-	The difference &gamma;2h-&gamma;2l: shapes how agents respond to the state of the environment.
-	The difference &gamma;3h-&gamma;3l: modifies these incentives.

### 4. Network Tab
- Link density: density of links in the Erdös-Rényi network.
-	New links: number of new links in the Barabasi-Albert network.
-	Impact: determines how agents’ environmental impact scales with their network degree.
-	Sigma: parameter influencing agent interaction.

### 5. HSM Tab (Heuristics Switching Model)
-	&beta;1, &beta;2, &beta;3: parameters for adaptive expectations, contrarian, and trend-following rules.
-	&rho;: probability of switching heuristics.
-	&eta;: memory factor for past heuristic performance.
-	&phi;: choice intensity for selecting better-performing heuristics.

## Running the Model

1.	Adjust parameters in each tab if desired.
2.	Optionally enter a plot title in the entry box. Press 'Enter' after typing the plot title.
3.	Click 'Run model' to execute the simulation.

## Outputs

The model generates three types of plots:
-	Resource State Plot: illustrates the state of the common pool resource over time.
-	Payoff Difference Plot: displays the difference in payoffs between agents with different extraction strategies.
-	Heuristics Plot: visualizes the distribution of heuristics used by agents.

## Requirements

-	CustomTkinter (5.2.2)
-	pillow (10.2.0)
-	Numpy (1.24.3)
-	Matplotlib (3.7.2)
-	Networkx (3.1)
-	tqdm (4.65)

## Acknowledgments

This GUI is based on an academic paper investigating common pool resource dynamics in social networks. For more details about the paper, please visit the GitHub repository.

## License

This GUI is distributed under the Creative Commons Attribution 4.0 International license.
The DOI of the project is https://doi.org/10.5281/zenodo.10566363. 

Feel free to explore the model, experiment with parameter settings, and gain insights into the dynamics of common pool resources!
