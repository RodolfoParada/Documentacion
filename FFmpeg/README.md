# Figma
- [Volver al Inicio](../README.md)
 ## FFmpeg convertidor .ts a mp4. en Ubuntu
```actualización
   sudo apt update 
```
```intalación
   sudo apt install ffmpeg
```

**Revisar la version instalada
```
   ffmpeg -version
```
**Actualización de repositorio
```
   sudo apt install handbrake 
```
```
   sudo apt update
```
**Comando ejemplo para convertir archivos
```
  ffmpeg -i "/home/trimogesimo/Documentos/obs/2025-04-11 09-08-18.ts" -c:v copy -c:a aac "/home/trimogesimo/Documentos/obs/2025-04-11 09-08-18.mp4"

```
  
