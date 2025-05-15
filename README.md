# aio-ai-lab-docker

Ein vollständiges AI-Lab für RTX 5090 mit:

- AUTOMATIC1111
- SD.Next
- ComfyUI
- Kohya_ss (Web UI)
- InvokeAI
- TensorBoard

## Nutzung

1. Modelle in `models/` legen
2. `docker-compose` starten:
   ```bash
   ./docker/start.sh
   ```
3. Web-UIs erreichbar unter:
   - A1111 → http://localhost:7860
   - Kohya → http://localhost:7861
   - ComfyUI → http://localhost:8188
   - SD.Next → http://localhost:9090
   - InvokeAI → http://localhost:3000
   - TensorBoard → http://localhost:6006
