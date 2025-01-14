# daedalus_descriptors
### A list of descriptors to use with Daedalus


# COMPONENT-LEVEL DESCRIPTORS

## Primary Role of Component

### role:

microcontroller

sensor

led

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

swd2030nl

jst
  
## Passive component specification
### pull_up_resistor:

u1:45, vdd

### pull_down_resistor:

q6:1, gnd

## When describing a component such as a sensor
### decoupling_capacitor:

c9

# NET-LEVEL DESCRIPTORS

## Type of net
### net_type:

power

ground

signal

pwr_main

GND

gnd_ref

signal_in

## Type of signal on the net
### signal_type:

i2c_sda

i2c_scle

pwm

digital_input

digital_output

analog

usb_dplus

usb_dminus

## If the net is part of a specific communication bus
### bus_type:

i2c

spi

uart

## Voltage range on the net
### voltage_range:

3_3v

1_8_to_3_3v

5v

## Frequency of the net for clock signals
### frequency:

8_megahz

32_khz

## Impedance controlled
### impedance_controlled:

yes

no

## List of connected components from the net, this can describe the node
### connected_components:

ref3020.2

C6

stm32.pa5

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

ref3020.out

stm32.PB6
