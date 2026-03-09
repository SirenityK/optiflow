# OptiFlow

**High-performance, private, and local-first video optimization**

OptiFlow is a cross-platform video optimizer built with Astro and Tauri. It is designed to bypass the file size limits on messaging platforms and to allow a poweruser to optimize the video himself on media, preventing transcoding in many cases (e.g. whatsapp).

This app is more meant for general sharing, such as memes or casual videos. So we have strict, lower quality presets

## Features
- **Local-First Privacy**: All processing happens on your wardware. No servers, ads, no telemetry, no corporate shit
- **Native performance**: The engine works on top of ffmpeg, we just provide presets that make video optimization so much easier.
- **Next-Gen Codec Support**: Full support for SVT-AV1, AOM-AV1 or modern codecs like HEVC. We include opus audio as well.
- **Lightweight**: Astro is great for an app like this, you'll be experiencing no issues with it!

## Presets
Every video default size is 854x480. OptiFlow detects automatically if the video is vertical or not, so the aspect ratio is always kept the same.
- **Discord**: Max video size capped at 10MB (or customizable) using two-pass SVT-AV1 and 32kbps Opus audio
- **WhatsApp**: H.264 and AAC. You may compile to get support for fdk-aac, getting access to HE-AACv2.
- **Email**: Capped at 24MB to ensure delivery across every mail server.

## Advanced configuration
- **Color space & Depth**: Support for BT.709, BT.2020 and 10-bit color depth.
- **Custom parameters**: Fine-tune resolution, frame rate and CRF values

### Roadmap
- [ ] Real-time preview
- [ ] Batch Processing
- [ ] Auto HDR-2-SDR

### Building
We use `justfile` for managing dependencies and building more easily.
`TODO`

