# Compatible sensors and calibration parameters

The tables below summarize sensor options mentioned in the IV-Indicators Nano LaTeX sources and the calibration parameters used by the presets.

## Oil/ coolant temperature sensors

| Compatible sensor | Signal/supply | Calibration parameters (from presets) |
| --- | --- | --- |
| Ossca 01176 NTC thermistor (thermometer preset) | Passive NTC | Validate against the Ossca 01176 resistance table (e.g., 270.0 Ω at 58 °C down to 15.9 Ω at 160 °C). For custom NTC probes, update the beta coefficient and nominal resistance in IV-Conf. |

## Air temperature sensors

| Compatible sensor | Signal/supply | Calibration parameters (from presets) |
| --- | --- | --- |
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
