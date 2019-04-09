There are circuit elements that we have identified in encoder and decoder circuits. 

- Comparators
- Invertors
- AND gates
- Adders

The way that we have implemented these circuits is by using analog electronic components such as transistors, resistors, capacitors etc.

### Comparator 

Comaparator is used to compare the digital signal with a reference voltage. For that we use a opamp ic. If the reference voltage is given to the positive input and the signal is given to the negetive input, the output wave form is inverted. 

![opamp106](https://user-images.githubusercontent.com/45971162/55793192-f79d5180-5adf-11e9-927e-3b19c456e265.gif)
### Invertor

This simply invert the digital signal. The signal should be given to the negetive input and the positive input is grounded. Somewhat similar to the comparator circuit if the reference is zero.

![opamp10](https://user-images.githubusercontent.com/45971162/55793378-5f539c80-5ae0-11e9-887b-ac840187e943.gif)

### AND gate

Using a AND gate IC is very easy rather than building AND gates using transistors. However, to have high frequency response, its better to build AND gates using transistors (2sc828). Basically we need two transistors for this and few resistors to bias those transistors.

![and4](https://user-images.githubusercontent.com/45971162/55799318-afd1f680-5aee-11e9-9696-53f4585e4e0c.gif)

### Adders

Two signals are added together by giving two signals to the positive input of the opamp. Otherthan that the output signal can be amplified by changing resistor values.


