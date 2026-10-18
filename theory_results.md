Parameters:
ΔL = 100.014 µm = 100014 nm
λ = 1550 nm
n_g = 4.2 (group index of silicon at 1550 nm)

Phase difference:
Δφ = (2π/λ) · n_eff · ΔL
(use n_eff here, not n_g; keep ΔL and λ in the same units)

Free Spectral Range (theory):
FSR = λ² / (n_g · ΔL)
FSR = 1550² / (4.2 × 100014)
FSR ≈ 5.7194 nm

Extracting FSR from the simulated graph:
FSR = λ(k+1) − λ(k)
where λ(k) and λ(k+1) are the wavelengths of two adjacent transmission peaks.
For N peaks, average over all of them:
FSR = (λ(N) − λ(1)) / (N − 1)

Group index from the graph:
n_g = λ² / (FSR_graph · ΔL)

Simulation results:

<img width="1000" height="500" alt="FSR" src="https://github.com/user-attachments/assets/9d919dbf-337b-47be-9ed2-c9bcc3c7e223" />

FSR(simulated)=5.7184nm
n_g= 4.2008


