# 🎯 Objective of Link Budget Calculation
To ensure that the received optical power at the ONU/OLT is within the acceptable sensitivity range, considering all losses in the fiber network.

## ✅ Link Budget Formula

Total Loss (dB) = Fiber Loss + Splice Loss + Connector Loss + Splitter Loss + Margin (Design Reserve)

Then:

  Link Budget = Transmitter Power (dBm) − Total Loss (dB)

The Link Budget must be greater than or equal to the receiver sensitivity.

## 🔧 Step-by-Step Breakdown

| Component | Typical Value | Notes |
| --- | --- | --- |
| Fiber Loss | 0.35 dB/km (at 1310 nm)/n 0.25 dB/km (at 1490 nm) | Depends on fiber type and wavelength |
| Splice Loss | 0.1 dB per splice | Typically 1 splice every 2 km |
| Connector Loss | 0.2 dB per connector | Usually 2 connectors per link |
| Splitter Loss | Varies by ratio | E.g., 1:8 = ~10.5 dB, 1:16 = ~13.5 dB, 1:32 = ~17 dB |
| Design Margin | 2–3 dB | Accounts for aging, temperature, maintenance |

## 📊 Rule of Thumb
  Always keep ≥3 dB reserve margin.
  
  If you're close to the limit, consider C+ optics or reducing the splitter ratio.
