# Remote Administration Tool

A lightweight remote administration tool for Windows systems with embedded file delivery capabilities.

## ⚠️ DISCLAIMER

**FOR EDUCATIONAL AND AUTHORIZED TESTING PURPOSES ONLY**

This tool is provided for educational purposes, security research, and authorized penetration testing only. By using this software, you agree to the following terms:

- This tool should ONLY be used on systems you own or have explicit written permission to test
- The developer is NOT responsible for any misuse, damage, or illegal activities performed with this tool
- Unauthorized access to computer systems is illegal in most jurisdictions
- Users are solely responsible for complying with all applicable local, state, national, and international laws
- This tool is provided "AS IS" without warranty of any kind
- The developer assumes NO liability for any consequences resulting from the use or misuse of this software

**USE AT YOUR OWN RISK**

## 📋 Features

- UAC elevation handling
- Windows Defender exclusion management
- Embedded file delivery system
- Resource embedding (images, files)
- Silent execution mode
- MOTW (Mark of the Web) removal
- Multiple language implementations (C++, Go, Python)

## 🛠️ Supported Languages

### C++ Version
- Native Windows API
- Small executable size (~2-3 MB)
- Resource embedding support
- Custom icon support

### Go Version
- Built-in `embed.FS` for file embedding
- Cross-platform code
- Medium executable size (~5-8 MB)
- Fast compilation

### Python Version
- PyInstaller packaging
- Easy to modify
- Larger executable size (~10-15 MB)
- Rapid development

## 📦 Building

### C++ Build
```bash
build_cpp.bat
```

### Go Build
```bash
build.bat
```

### Python Build
```bash
build_python_with_images.bat
```

## 📁 Project Structure

```
.
├── files/              # Embedded files folder
├── loader.cpp          # C++ implementation
├── loader.go           # Go implementation
├── loader.py           # Python implementation
├── resource.rc         # Windows resources
├── icon.ico            # Application icon
└── build scripts       # Build automation
```

## 🔧 Requirements

### C++
- MinGW-w64 or MSVC
- windres (resource compiler)

### Go
- Go 1.21 or higher
- rsrc tool for icon embedding

### Python
- Python 3.x
- PyInstaller

## ⚙️ Configuration

Edit the source files to configure:
- Target URL for file delivery
- Embedded files location
- Execution parameters
- Defender exclusion paths

## 🔒 Security Notice

This tool modifies system security settings including:
- Windows Defender exclusions
- UAC (User Account Control) settings
- File execution policies

**Only use on systems you are authorized to modify.**

## 📜 Legal Notice

The use of this tool for attacking targets without prior mutual consent is illegal. It is the end user's responsibility to obey all applicable local, state, national, and international laws. The developer assumes no liability and is not responsible for any misuse or damage caused by this program.

**By using this software, you acknowledge that:**
1. You have read and understood this disclaimer
2. You will use this tool only for lawful purposes
3. You accept full responsibility for your actions
4. You will not hold the developer liable for any consequences

## 🤝 Contributing

This project is for educational purposes. Contributions should maintain the educational and ethical nature of the project.

## 📄 License

This project is provided for educational purposes only. Use responsibly and ethically.

---

**Remember: With great power comes great responsibility. Use this tool ethically and legally.**
