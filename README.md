# Considering_Neuron_length

**Software**
1. NEURON 8.2 https://www.neuron.yale.edu/neuron/
2. Python 3.9.18
3. TI Planing Tool TIP V2.0 https://itis.swiss/tools-and-systems/ti-planning/



**Code explanation 1**

dt = 1e-3  # Time step size (in ms)

stim_t = np.arange(0, duration, dt)  # Time array

plus_wave_1 = amp1_1 * np.sin(2 * np.pi * freq1 * stim_t / sec_unit) 

-> sec_unit is about unit of time
  example) sec_unit = 1000 -> ms (unit)
  
-> When u change frequency, then dt also should be changed
   1) frequency: 1e6, dt: at least 1e4
   2) frequency: 1e9, dt: at least 1e7
