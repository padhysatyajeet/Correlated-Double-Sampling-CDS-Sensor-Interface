## Correlated Double Sampling

CDS operates using two sampling phases.

### Ph1 – Offset Sampling

During Ph1, the circuit samples the input-referred offset of the amplifier and stores the corresponding charge on the sampling capacitors.

### Ph2 – Signal Sampling

During Ph2, the input signal is sampled. The previously stored offset information is used during charge redistribution to cancel the amplifier offset.

The basic principle is:

```text
Sample 1 = Voffset

Sample 2 = Vinput + Voffset

Output = Sample 2 - Sample 1

Output = Vinput
