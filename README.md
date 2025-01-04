# daedalus_descriptors
### A list of descriptors to use with Daedalus


# COMPONENT-LEVEL DESCRIPTORS

## Primary Role of Component

### role:

microcontroller

sensor

LED

voltage_reference_source

power_management

indicator

oscillator

clock_source

port

pull_up_resistor

pull_down_resistor

decoupling_capacitor

USB

## Type of sensor
### sensor_type:

IMU

temperature

pressure

## Type of port
### port_type:

JST

SWD

## External connection
### external_mate:

SWD2030NL

JST
  
## Passive component specification
### pull_up_resistor:

U1:45, VDD

### pull_down_resistor:

Q6:1, GND

## When describing a component such as a sensor
### decoupling_capacitor:

C9

# NET-LEVEL DESCRIPTORS

## Type of net
### net_type:

power

ground

signal

PWR_MAIN

GND

GNDREF

SIGNAL_IN

## Type of signal on the net
### signal_type:

I2C_SDA

I2C_SCL

PWM

digital_input

digital_output

analog

USB_Dplus

USB_Dminus

## If the net is part of a specific communication bus
### bus_type:

I2C

SPI

UART

## Voltage range on the net
### voltage_range:

3_3V

1_8-3_3V

5V

## Frequency of the net for clock signals
### frequency:

8MHz

32kHz

## Impedance controlled
### impedance_controlled:

yes

no

## List of connected components from the net, this can describe the node
### connected_components:

REF3020.2

C6

STM32.PA5

## Describes the role of the signal in the circuit
### function:

status_indicator

interrupt

reference_voltage

clock_signal

## Specifies the direction of the signal on the net (can override if unclear if symbol editor has information on it)
### direction:

input

output

bidirectional

## Describes the trigger condition for an interrupt signal
### trigger_type:

rising_edge

falling_edge

## Indicates if the net is part of a critical timing path
### critical_path:

yes

no

## Describes the source of the net's signal (less critical)
### source_component:

REF3020.OUT

STM32.PB6
