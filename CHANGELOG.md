# Changelog / Historial de cambios

## MP4 STABLE — November 2026 / Noviembre de 2026

| Change | Cambio |
|---|---|
| Native MP4/H.264 and AAC playback | Reproducción nativa MP4/H.264 y AAC |
| One decoder thread per context | Un hilo por contexto de decodificación |
| Direct aligned RGB output with compatible fallback | Salida RGB alineada con alternativa compatible |
| Progressive audio decoding instead of full-track buffering | Audio progresivo en lugar de cargar toda la pista |
| PTS-based scheduling and estimated audio clock | Temporización PTS y reloj de audio estimado |
| FIX3: runtime SIMD selection disabled after H.264 crash | FIX3: selección SIMD desactivada tras cierre H.264 |
| Static Windows x86 build and GCC -O3 | Compilación Windows x86 estática y GCC -O3 |

Both video and audio initialization applies FIX3. / La inicialización de video y audio aplica FIX3.

The Windows build disables the legacy SVGAWIN and SVGAlib backends; use SDL. AdvMenuPLUS-specific features are retained in the port, but not every feature has been regression-tested.

La compilación Windows desactiva los controladores antiguos SVGAWIN y SVGAlib; utilizar SDL. Se conservan las funciones propias de AdvMenuPLUS en el port, aunque no se probaron exhaustivamente todas ellas.

Local playback was reported successful; no complete benchmark or regression suite. / Se informó reproducción correcta localmente; no hay benchmark ni pruebas de regresión exhaustivas.
