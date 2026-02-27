
解決CUDA out of memory，啟動 ComfyUI 時加入以下參數：
```bash
python main.py --lowvram --fp16 --cpu-vae
```



### 支援模型總覽

| 模型 | 顯存需求 | 8GB 可用 | 備註 |
|------|----------|-----------|------|
| SD 1.5 | 2–3 GB | ✅ 完美 | 最穩定，資源最省 |
| SDXL | 5–6 GB | ✅ 可用 | 建議開 Tiled VAE |
| SDXL Turbo / Lightning | 5–6 GB | ✅ 可用 | 4步出圖，超快 |
| Flux.1 Dev (GGUF Q4) | 7–8 GB | ✅ 可用 | 需量化版本 |
| Flux.1 Schnell (GGUF Q4) | 7–8 GB | ✅ 可用 | 比 Dev 快 4 倍 |
| AnimateDiff (SD1.5) | 4–5 GB | ✅ 可用 | 512px 最穩定 |
---