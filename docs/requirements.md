# Requirements (Brainstorming)

## Main HW features

  - Balancing triggered by highest cell voltage for top-balancing
    * Passive balancing top-only
    * Active Balancing (add-on-module) top and if possible bottom (triggered by lowest cell voltage)
      * single-coil-multi-wire
      * coil-per-cell
      * capacitor-based
  - Battery-Interconnect with RS485
  - No manual adress settings
  - WiFi for config
  - CAN for Upstream
  - BLE for initial setup (master/slave)
  - Active Current Limiting (implemented by separate uC e.g., STM32)
  - SC, OC, OV, UV limiting (implemented by BMS circuit)
  - Integrated DC/DC with 3 x USB (5V), 2 x USB-C PD (5/9/12/15/20V@5A)
  - Wireless charging option
  - Display connector
  - Main On/Off SW (Soft-Button)

## Main SW features

  - Master BMS serves WebUI, Slaves have locked WebUI -> forwarding
  - WebUI with REST-API
  - Modbus TCP
  - MQTT
  - ESPhome (custom component for HW parts and full BMS)
    
