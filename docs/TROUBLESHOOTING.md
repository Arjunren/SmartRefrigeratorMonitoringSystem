# Troubleshooting — SmartRefrigeratorMonitoringSystem

| Symptom | Check |
|---|---|
| No cabinet temperature proxy | Verify sensor power, grounds, pin table, voltage limits, and module orientation. |
| Invalid sample | Check 0–4095 ADC counts range and sensor calibration. |
| Wi-Fi disconnected | Check SSID, 2.4 GHz coverage, and local network policy. |
| MQTT disconnected | Check broker DNS, port 8883, CA PEM, device credentials, and publish ACL. |
| Unexpected alert | Inspect raw cabinet temperature proxy and door open; calibrate the threshold in `logic.h`. |
| Build failure | Confirm PlatformIO is installed and dependency downloads are permitted. |

ADC threshold needs temperature calibration; not suitable for regulated cold-chain assurance.
