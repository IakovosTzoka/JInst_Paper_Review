# Instrumentation review checks

These are technical review prompts developed for this skill, not official journal requirements. Select checks justified by the instrument and claims. Request the minimum evidence needed to support the stated use; distinguish desirable extensions from necessary corrections.

## Measurement chain and operating conditions

- Follow the chain from physical stimulus through sensor, front end, digitization, trigger, reconstruction, and reported observable. Identify missing transfer functions or corrections that could change the result.
- Check geometry, materials, active area or volume, grounding and shielding, bias, gain, shaping, sampling, environmental conditions, and software or firmware settings where relevant.
- Separate demonstrated operating conditions from projected deployment. Check rate, temperature, pressure, fields, radiation, power, and mechanical constraints against the intended application.
- Determine the independent unit of replication: events, channels, devices, fabrication batches, or runs. Many events from one device do not establish device-to-device reproducibility.

## Calibration and uncertainty

- Identify calibration standards, reference-device uncertainty, calibration range, drift, interpolation or extrapolation, and traceability where claimed. Check whether a calibration is independently validated.
- Distinguish repeatability, resolution, precision, and accuracy. An unmeasured systematic offset is not constrained by a narrow distribution.
- Inspect statistical and systematic components, shared calibrations, correlations, nuisance parameters, and the basis for combining uncertainties. Clarify whether error bars are standard deviations, standard errors, confidence intervals, or expanded uncertainties.
- Check propagation through nonlinear transformations, background subtraction, normalization, and efficiency corrections. Include covariance when dependence matters.
- Check physical dimensions, numerical consistency, rounding, and whether quoted performance exceeds the reference apparatus's resolving capability without a supported deconvolution.

## Detector and readout performance

- Define efficiency using a defensible denominator and independent reference or trigger. Check acceptance, dead channels, cuts, accidental coincidences, and threshold dependence.
- For energy, position, or timing resolution, identify estimator, fit model, tails, fit range, reference contribution, and whether the result is single-device or combined performance. FWHM-to-sigma conversion requires a Gaussian interpretation; quadrature subtraction requires an appropriate independent variance model.
- Check noise, baseline stability, gain variation, linearity, dynamic range, saturation, crosstalk, afterpulsing, and pile-up only where relevant to the device.
- Distinguish input rate from accepted throughput. Check live time, dead time, buffering, event loss, latency distributions, clock synchronization, and sustained-load tests for readout or DAQ claims.
- Assess stability, radiation tolerance, aging, yield, and environmental robustness only to the extent that conclusions depend on them. Do not demand lifetime qualification for a paper limited to an early prototype.

## Experiments, statistics, and selection

- Check source or beam characterization, exposure, backgrounds, controls, event counts, and exclusions. Verify that cuts and optimization do not select favorable performance on the same validation data.
- Check likelihood or fitting assumptions against count levels, weighting, binning, censoring, and correlations. Do not automatically require Gaussian errors or a hypothesis test.
- Examine goodness-of-fit and residuals rather than relying solely on a fitted parameter uncertainty. Consider whether alternative plausible models change the claimed outcome.
- Check uncertainty on proportions and low counts, treatment of zero-event bins, repeated comparisons, and whether uncertainty on a ratio accounts for shared events.
- Compare benchmarks at matched operating points and conditions. A better headline number may reflect different area, rate, threshold, power, beam energy, or processing constraints.

## Simulation, reconstruction, and learning methods

- Identify geometry, material properties, boundary conditions, source model, transport or physics configuration, digitization, software versions, and numerical settings needed to reproduce the claim.
- Distinguish numerical verification, calibration or tuning, and independent validation. Agreement with a distribution used for tuning is not independent predictive evidence.
- Check Monte Carlo precision, convergence where relevant, sensitivity to uncertain inputs, and quantitative comparison with measurements. Treat simulation-only performance as a prediction.
- For learned methods, inspect train/validation/test independence at the run or device level, leakage, tuning, simulation-to-data differences, baseline fairness, operating-point selection, and resource costs.

## Figures, artifacts, and practical value

- Check that plots identify units, normalization, binning, uncertainties, sample sizes where needed, operating conditions, and data versus simulation. Look for inconsistent values across text, tables, and figures.
- Judge whether the description permits reconstruction of the essential measurement or analysis. Useful artifacts may include schematics, layouts, calibration constants, event definitions, configurations, code versions, and representative data.
- Respect legitimate proprietary or collaboration constraints; identify their impact on verification and possible alternative evidence without inventing an open-source publication requirement.
- For a technical report, explain the practical contribution: a reproducible method, characterized component, improved instrument, integration result, or useful performance boundary.
