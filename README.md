# 🔥 ChainsawFire Client

A modified Minetest 0.4.17 client with enhanced combat features and quality-of-life improvements.

## ⚡ Features

### Combat Enhancements
- **KillAura** — Automatically attacks all entities within range (toggle with `G` key)
- **High Damage Mode** — Sends multiple interaction packets for amplified damage output
- **Multi-target Support** — KillAura hits all nearby entities simultaneously, not just one
- **Visual Feedback** — Mobs flash and show damage prediction when hit by KillAura
- **Continuous Damage** — No more attack delays; punch timers are managed for rapid, uninterrupted hits

### Other Cheats
- **X-Ray** — See through blocks to find ores (toggle with `X` key)
- **Fullbright** — Full lighting everywhere, no dark areas

## 🔧 Building from Source

### Prerequisites
- CMake 3.5+
- C++ compiler (GCC, Clang, or MSVC)
- Irrlicht 1.8.3+
- SQLite3
- zlib
- Optional: LevelDB, cURL, OpenAL + Vorbis (for sound), Freetype2 (for fonts)

### Build (Linux)
```bash
mkdir build && cd build
cmake .. -DBUILD_CLIENT=ON -DBUILD_SERVER=OFF
make -j$(nproc)
```

### Build (Windows with MSVC)
```bash
mkdir build && cd build
cmake .. -G "Visual Studio 17 2022" -DBUILD_CLIENT=ON -DBUILD_SERVER=OFF
cmake --build . --config Release
```

### Build (Android)
See `doc/README.android` for detailed Android build instructions.

## 🎮 Controls

| Key | Action |
|-----|--------|
| `G` | Toggle KillAura |
| `X` | Toggle X-Ray |
| `WASD` | Movement |
| `Space` | Jump |
| `Shift` | Sneak |
| `Left Click` | Attack / Dig |
| `Right Click` | Place / Use |

## 📋 Configuration

ChainsawFire uses the same configuration file as Minetest (`minetest.conf`). All standard Minetest settings are supported.

## 📜 License

This project is licensed under the **GNU Lesser General Public License v2.1** — see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Credits

### Core Developer
- **GP-commits** — gamerpayyan1@gmail.com

### Based On
- [Minetest](https://www.minetest.net/) by celeron55 and contributors

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📧 Contact

- **Email**: gamerpayyan1@gmail.com
- **GitHub**: [@GP-commits](https://github.com/GP-commits)
