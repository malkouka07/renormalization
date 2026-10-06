# Renormalization and the 2D Ising model

This repository contains a Jupyter notebook exploring the two-dimensional Ising model with single-spin Metropolis updates. The notebook studies equilibration, autocorrelation, blocking estimates of statistical uncertainty, simulation-length dependence, and finite-volume effects at inverse temperatures including $\beta=0.5$ and $\beta=0.45$.

## AI-assisted development

This work was developed collaboratively by Mihaly Marko Cserpak and OpenAI Codex. Mihaly defined the physical questions, selected the simulation cases, directed the analysis, and reviewed the results. Codex assisted with:

- implementing and reorganizing Python notebook cells;
- distinguishing attempted spin flips from Monte Carlo sweeps;
- diagnosing long-lag autocorrelation artifacts;
- implementing hot/cold equilibration comparisons;
- calculating exponential and integrated autocorrelation times;
- constructing blocking estimates and uncertainty-versus-length studies;
- producing finite-volume and convergence plots; and
- validating the notebook structure and code syntax.

All reported numerical values and plots were produced by executing the simulation code locally. The AI did not supply or fabricate simulation data. Its role was to help write, review, debug, and explain the analysis under the author's direction.

Because local Metropolis simulations near the critical point can have long autocorrelation times, results should be interpreted using the equilibration, autocorrelation, and blocking checks included in the notebook.

## Files

- `hw_1.ipynb`: active analysis notebook.
- `hw_1.pre-beta045-backup.ipynb`: recovery snapshot from before the $\beta=0.45$ section was added.
- `hw_1.accidental-reverted-backup.ipynb`: older recovery snapshot retained for provenance; it contains an incomplete cell and is not intended for execution.
