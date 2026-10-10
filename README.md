# Energy Systems Optimization

Optimization models for power-system scheduling and network operation, developed in Python with Pyomo.

## What this project demonstrates

- **Unit commitment:** minimize generation cost while meeting hourly demand and generator operating limits.
- **Stochastic scheduling:** evaluate multiple wind and solar scenarios and account for renewable uncertainty.
- **Optimal power flow:** formulate and solve both AC and DC network models, including voltage, reactive-power, and power-balance constraints.
- **Analysis and communication:** load structured CSV data, validate solver results, export JSON outputs, and visualize generation schedules, costs, and voltage profiles.

## Technology

Python · Pyomo · NumPy · pandas · Matplotlib · NetworkX · CPLEX/CONOPT via NEOS

## Project structure

- `stoch_unit_commitment.ipynb` — scenario-based unit commitment
- `unit_commitment_expected_values.ipynb` — expected-value unit commitment
- `OPF/opf_starter.ipynb` — AC/DC optimal power flow
- `visualization_stage_1.ipynb` — exploratory data analysis and plots
- `Data/` and `Results/` — input datasets, figures, and solver outputs

## Running the notebooks

Open the notebooks in Jupyter or VS Code, install the Python dependencies used in the Technology section, and run the cells in order. The optimization notebooks submit models to the NEOS solver service, so a compatible solver configuration and network access are required.
