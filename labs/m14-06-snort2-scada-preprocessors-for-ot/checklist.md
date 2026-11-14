# Verification checklist

Work through this after the test steps. Do not assume it works: confirm each item.

- [ ] A protocol and port inventory exists.
- [ ] Modbus (and other SCADA) preprocessor ports match the PLC ports.
- [ ] The NAP is deployed to the right devices and networks.
- [ ] `show conn address <PLC_IP> detail` shows the N flag for the PLC connection.
- [ ] `packet-tracer` or test traffic confirms the flow is allowed and inspected as intended.
