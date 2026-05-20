# Heat Pump DHW Card

Lovelace dashboard card voor de [Heat Pump DHW](https://github.com/FutureCow/ha-heatpump-dhw) integratie.

## Installatie via HACS

1. Voeg deze repository toe als aangepaste repository in HACS (type: **Lovelace**)
2. Installeer "Heat Pump DHW Card"
3. Herstart Home Assistant / doe een hard refresh (Ctrl+Shift+R)

## Configuratie

```yaml
type: custom:heatpump-dhw-card
title: Warmtepomp Boiler
temp_sensor: sensor.dhw_boiler_temp
mode_sensor: sensor.dhw_active_mode
status_sensor: sensor.dhw_status_text
session_kwh_sensor: sensor.dhw_session_kwh
session_cost_sensor: sensor.dhw_session_cost
next_heating_sensor: sensor.dhw_next_heating
power_sensor: sensor.dhw_power_w              # optioneel
heat_up_sensor: sensor.dhw_heat_up_duration_min  # optioneel
price_forecast_sensor: sensor.zonneplan_current_electricity_tariff  # voor prijsgrafiek
target_temp_sensor: number.boiler_setpoint    # optioneel
heat_now_button: button.heat_pump_dhw_zet_aan  # optioneel
solar_switch: switch.dhw_solar_mode
price_switch: switch.dhw_price_mode
boost_switch: switch.dhw_boost_mode
vacation_switch: switch.dhw_vacation_mode
legionella_switch: switch.dhw_legionella_mode
```

Zie de [integratie documentatie](https://github.com/FutureCow/ha-heatpump-dhw) voor alle opties.
