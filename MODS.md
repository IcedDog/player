# Mods

## Roadmap

- [ ] Scroll Speed
- [ ] Auto-Play
- [ ] Reorder Z-Index
- [ ] Floating Text
- [ ] Floating Image
- [ ] Render Texture and Realtime Blits
- [ ] QoL Shaders
  - [ ] Flash
  - [ ] Darken
  - [ ] Tape Rewind (Rhythm Doctor)
  - [ ] 3D Playfield Transform
- [ ] NotITG-Style Modifiers
  - [ ] Playfield Transform
    - [ ] X, Y movements
    - [ ] Scale & Rotation
    - [ ] Skew
  - [ ] Camera Transform
    - [ ] X, Y movements
    - [ ] Zoom & Rotation
  - [ ] Appearance Modifiers
    - [ ] Hidden
    - [ ] Color
    - [ ] Dizzy, Rotation
    - [ ] Pulse
    - [ ] Skew
  - [ ] Path Modifiers
    - [ ] Beat
    - [ ] Drunk
    - [ ] Bounce
    - [ ] Wave
    - [ ] Tornado
    - [ ] Brake
  - [ ] DrawSize

## Format

在你的 `extra.json` 文件中配置你的模组。请注意，`effects` 字段被视为弃用，如果使用则会禁用模组中的相关事件。

### Events

添加 `events` 字段，它是一个数组，其中包含你的模组事件。一个事件可能长得像这样：

```json
{
  "events": [
    {
      "type": "FloatingText",
      "start": [0, 0, 1],
      "text": "Hello, world!",
      "textStyle": {
        "font": "Arial",
        "fontSize": 24,
        "color": [255, 255, 255]
      }
    }
  ]
}
```

每个 `event` 都有一个 `type`，它决定了模组的类型。同时，每个 `event` 需要规定其 `start`，代表其触发时间。
大部分模组也都需要 `end` 字段，代表其结束的时间。其余的字段则根据模组的类型不同而不同。

### FloatingText

### FloatingImage

### RenderTexture

### Camera

### MainCameraTransform

### PlayfieldTransform

### Blit

### Effect

### Reorder
