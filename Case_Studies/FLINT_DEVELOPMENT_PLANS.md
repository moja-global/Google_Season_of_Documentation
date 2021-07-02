# FLINT Development Plans

## Table of contents

-   [Core 2.0](#core-20)
-   [Science 2.0](#science-20)
-   [Maturing the FLINT ecosystem](#maturing-the-flint-ecosystem)
-   [Deployments and interfaces](#deployments-and-interfaces)
-   [Optimisation and coordination](#optimisation-and-coordination)

## Core 2.0

-   Refactoring for improved code clarity, paying down technical debt.
-   Profiling model runs to establish performance benchmarks.
-   Improved and standardised metadata format to enable spatial outputs with attribute tables.
-   Improved accessibility for less technical users. Simplified installation. Possibly pre-configured sets of modules to reduce complexity.
-   Pre- and post-processing functions + resources for analytic capability development of external organisations, particularly reporting and visualisation.
-   Best use case for spatial models is planning. (Can we couple projections with policy making?)
-   Improved uncertainty analysis.
-   Agnostic framework for “spatialising” and scaling pet models (example: DAYCENT) - FLINT as “the scaling tool”
-   Best-practice guides and configuration for for scaling inputs + outputs to next-gen remote sensing data and model complexity, including optimised performance.
-   Synthesis and aggregation of model values when working with supra-individual scales (30cm)  or daily temporal resolution [possibly core 3.0] 
-   How do we enable statistically ‘learning’ models (aka ‘online models’ or ‘checkpointing’) for adaptive forecasting - updating projections as new data become available.

## Science 2.0

-   Enable as many different additional modules as possible- grasslands, permafrost.
-   Improved representation of forest structure for size based modelling of multi-species cohort productivity. Leverage existing models, but requires optimisation of potentially large outputs.
-   Improved environmental covariates (soil, aspect, hydrology) to avoid assigning pixel based yield curves. 
-   Vertical stratification of soil layers, sub-annual time resolution for seasonal environmental changes.
-   Current architecture design and limitations
    -   the space vs. time loop
    -   Cohort tracking
    -   Data aggregation
    -   Dynamic unpacking
    -   Database structure
    -   Build toolkit
    -   Pixel independence makes things like fire-risk propagation difficult

### Performance targets and Hardware requirements

-   $$ vs time vs complexity vs resolution
-   Are there existing bottlenecks that can be designed around?
-   Model runtime often faster than post-processing
-   Could publish benchmarks as best-practice implementations and regression tests for base library.

## Maturing the FLINT ecosystem

### Support for exising and future implementations

-   **Existing**: 
    GCBM (Canadal; Chile; Belize), FLINTpro (FullCAM), SLEEK (+/-), iNCAS.

-   **Future**:
    FAO + SEPAL - containerised Tier 1, good onramp for developing countries but comes with maintenance burden.

-   Agriculture and other land uses- required for spatial coverage without overlaps.

### Features that moja should maintain vs. endorse community led projects (aka minimum requirements)

-   Data pre-processing for a country.
-   Model run : Retrospective + Projective.
-   Compare scenarios for a few key indicators (Example: area) / reporting.
-   Visualisation.
-   Case studies : tier 1 spatial analysis, exemplify benefits of spatial modelling always with focus of long term impact on GHG and land use change, policy making should be based on sound science. Otherwise advocacy neutral.
-   What would data and validation standards for modules look like?

## Deployments and interfaces

-   Improving usability and onboarding.
-   Policy makers - what are they going to receive?
-   Report makers - what do they need in order to deliver to policy makers?

## Optimisation and coordination

-   Begin prioritising foundational work items/design decisions required to enable future development.
-   Reduced barriers to entry.
-   Breadcrumbs to increasing complexity.
-   Improved data pre-processing for non-technical users.
