<image align="right" alt="Milad" width = "420" src="http://up44.ir/previews/c3c5f7dab58aa78702557eeb7517235e.jpg"> 
import math <br />
<br />
ζ_a = 1 <br />
L_w = 20 <br />
g = 9.81 <br />
π = 3.14 <br />
<br />
V_w = (g * L_w) / (2 * π) <br />
time_values = [0, 0.1, 0.2, 1]  # Assuming you want to calculate ζ for specific time values <br />
<br />
for t in time_values: <br />
    for x in range(21):  # Assuming x ranges from 0 to 20 <br />
        ζ = ζ_a * math.sin((2 * π / L_w) * (x - (V_w * t))) <br />
        print(f"ζ at t={t:.1f}, x={x}: {ζ:.4f}") <br />
