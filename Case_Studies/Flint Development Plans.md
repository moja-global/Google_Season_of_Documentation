# FLINT Development Plans

## Table of Contents

* [Core 2.0](#core)

## Core

* Refactoring for improved code clarity, paying down technical debt.

* Profiling model runs to establish performance benchmarks.

* Improved (standardised?) metadata format to enable spatial outputs with attribute tables.

* Improved accessibility for less technical users. Simplified installation. Possibly pre-configured sets of modules to reduce complexity.

* Pre- and post-processing functions + resources for analytic capability development of external organisations, particularly reporting and visualisation.

* Best use case for spatial models is planning. Can we couple projections with policy making?

* Improved uncertainty analysis.

* Agnostic framework for “spatialising” and scaling pet models (e.g. DAYCENT) - FLINT as “the scaling tool”

* Best-practice guides and configuration for for scaling inputs + outputs to next-gen remote sensing data and model complexity, including optimised performance.

* Synthesis and aggregation of model values when working with supra-individual scales (30cm)  or daily temporal resolution [possibly core 3.0] 

* How do we enable statistically ‘learning’ models (aka ‘online models’ or ‘checkpointing’) for adaptive forecasting - updating projections as new data become available.

## Science 2.0

* Enable as many different additional modules as possible- grasslands, permafrost

* Improved representation of forest structure for size based modelling of multi-species cohort productivity. Leverage existing models, but requires optimisation of potentially large outputs.

* Improved environmental covariates (soil, aspect, hydrology) to avoid assigning pixel based yield curves. 

* Vertical stratification of soil layers, sub-annual time resolution for seasonal environmental changes.

* Current architecture design and limitations
    * the space vs. time loop
    * Cohort tracking
    * Data aggregation
    * Dynamic unpacking
    * Database structure
    * Build toolkit
    * Pixel independence makes things like fire-risk propagation difficult
### Performance targets and hardware requirements

* $$ vs time vs complexity vs resolution

* Are there existing bottlenecks that can be designed around?

* Model runtime often faster than post-processing

* Could publish benchmarks as best-practice implementations and regression tests for base library.



