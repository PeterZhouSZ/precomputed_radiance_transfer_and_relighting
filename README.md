# precomputed_radiance_transfer_and_relighting
Implementation of All-Frequency Shadows Using Non-linear Wavelet Lighting Approximation by Ren Ng et al.
https://www.youtube.com/watch?v=_5wzg2F_x7Y

First, execute "GenerateLightTransportMatrix.exe" (or "GenerateLightTransportMatrixGeometryRelighting.exe" for geometry relighting). Once the process is complete, 18 files (ltm_ir, ltm_ig, ltm_ib (i=1-6)), each of which stores the corresponding light transport matrix, will be created in the directory "data". Note that this will take several hours and require large disk space (more than 20GB). Then, execute "RealtimeRendering.exe" (or "RealtimeRenderingGeometryRelighting.exe). For image religting, if you run "RealtimeRendering.exe" with argument "1", you can quantize and dither the entries of the light transport matrix.
