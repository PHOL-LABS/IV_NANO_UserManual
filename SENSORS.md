# Compatible sensors and calibration parameters

The tables below summarize sensor options mentioned in the IV-Indicators Nano LaTeX sources and the calibration parameters used by the presets.

## Oil/ coolant temperature sensors

| Compatible sensor | Signal/supply | Calibration parameters (from presets) |
| --- | --- | --- |
| Ossca 01176 NTC thermistor (thermometer preset) | Passive NTC | Validate against the Ossca 01176 resistance table (e.g., 270.0 Ω at 58 °C down to 15.9 Ω at 160 °C). Nominal calibration parameters: R25 = 1 kΩ, β = 3950. For custom NTC probes, update the beta coefficient and nominal resistance in IV-Conf. |
| RIDEX 829S0003 (Opel/BMW/Volvo compatible) | 2-pin NTC, M12×1.5 thread | Nominal resistance 2080 Ω at 25 °C and 294 Ω at 80 °C (β ≈ 3740 K). Operating temperature range 25–80 °C. Sensor body Ø 7.4 mm, hex 19 mm, supplied with sealing gasket. |

## Air temperature sensors

| Compatible sensor | Signal/supply | Calibration parameters (from presets) |
| --- | --- | --- |
| MFA outside air temperature sensor (VAG 171 919 379 A, Golf Mk2/Jetta II/Passat B2/B3) | 2-wire NTC, floating | Approx. display span −40 °C to +96 °C. Empirical calibration: R25 ≈ 510 Ω, β ≈ 3400–3500 K (fit between +4 °C and +50 °C). Diagnostic reference: 200 Ω ≈ +50 °C. |
| NTC thermistor equivalent to Ossca 01176 (thermometer preset) | Passive NTC | Use the Ossca 01176 resistance table as the reference and adjust beta coefficient/nominal resistance for custom NTC sensors via IV-Conf. |

## Oil pressure sensors

| Compatible sensor | Signal/supply | Calibration parameters (from presets) |
| --- | --- | --- |
| VAG 03C906051A pressure sensor (barometer preset) | 5 V supply, analogue output | 10 bar absolute range, 0.4–0.5 V nominal output at rest; configure measurement range with the barometer preset and adjust min/max ranges in IV-Conf if required. |

## Fuel level gauges

| Compatible sensor | Signal/supply | Calibration parameters (from presets) |
| --- | --- | --- |
| Custom sensor (no specific model listed) | Depends on sensor | Use IV-Conf to set the minimum/maximum measurement range to match the installed sensor. |

## Boost pressure sensors

| Compatible sensor | Signal/supply | Calibration parameters (from presets) |
| --- | --- | --- |
| Dacia 223657266R (also 161B0004/8200225971) | 5 V supply, analogue output | 20–250 kPa operating window, ~1.8 V nominal output at boost; use the boost preset and adjust range min/max if needed. |

## Wideband lambda

| Compatible sensor | Signal/supply | Calibration parameters (from presets) |
| --- | --- | --- |
| Wideband controller (SLC Free, DIY-EFI TinyWB, Sigma Lambda Controller Free 2) with Bosch LSU 4.9 probe | 0–5 V linear output to gauge | Wideband controllers translate the LSU 4.9 probe into a linear 0–5 V signal accepted by the gauge; narrowband sensors provide 0.1–0.9 V swing. |
