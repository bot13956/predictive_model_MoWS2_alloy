# predictive_model_MoWS2_alloy

This code performs first-principle calculations for the MoWS2 alloy at fixed geometry. The geometry parameters like bond lengths and lattice constants are obtained experimentally. A self-consistent calculation is performed using atomic pseudopotentials to obtain the converged electron density, which is then used to calculate the quantum energy levels of the system. A band structure calculation is performed at the end of the self-consistent field calculation in order to predict important optoelectronic parameters such as energy band gap and electron/hole effective masses. All calculations are performed using the Quantum Espresso DFT Solver. For more information, see the following link: https://www.quantum-espresso.org/

Mo.rel-pw91-spn-rrkjus_psl.0.3.0.UPF: atomic pseudopotential file for Molybdenum.

W.rel-pw91-spn-rrkjus_psl.0.2.3.UPF: atomic pseudopotential file for Tungsten.

S.rel-pw91-n-rrkjus_psl.0.1.UPF: atomic pseudopotential file for Sulfur.

scf.in: performs self-consistent field calculations using density functional theory.

bands.in: performs band structure calculation after self-consistent field calculation is completed.

bands_plot.in: re-arranges band structure data in a format that projects two-dimensional band structure into a one-dimensional plot along high symmetry lines in the Brillouin zone.

batch_script.pbs: batch script for batch scheduling and allocating of computer resources.

output.pdf: shows the structure of the MoWS2 alloy and useful outputs such as band structure plots and energy band gap.
