# Optimized-Polar-Return-to-Zero-Line-coding-Transceiver

### Why not just 'polar return-to zero' ?

Here we have implemented a polar return-to-zero line coding transceiver which is optimized using a clock delay. The ordinary polar return zero line encoding technique can be graphically visualize as follows, 

![image](https://user-images.githubusercontent.com/45971162/55667712-b1e14e80-587d-11e9-8329-c43bc32ceec0.png)

To encode the data signal into this polar return to zero signal, the usual way is to have the clock frequency doubled the frequency of the data signal. This data signal and clock signal are initially synchronized as follows, and that synchronized signals are sent through the encoder circuit to obtain the encoded signal.

![image](https://user-images.githubusercontent.com/45971162/55667724-e228ed00-587d-11e9-8124-b06168162ad6.png)

There are some practical issues with above methods when implemented using an analog encoding circuit. The main concern (which will create lot of problems) is asynchronized clock. In this method if the clock pulse is not synchronized with the data pulse it will generate an unnecessary impulse at each clock cycle (main reason is when the two signals are AND together since they are asynchronized a small pulse will be generated). These impulses will corrupt the encoded signal in large scale.

### How did we optimizi ?

However, to optimize this encoding method, we used a different approach. To address this issue, we intentionally delayed the clock pulse (a known delay) so that one clock pulse will come in the middle of each data pulse. 
