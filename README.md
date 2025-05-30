# Real-Time ASL Interpreter

A machine learning application that translates American Sign Language gestures into text and speech in real-time using webcam input.

## ✨ Features
- **Hand Tracking**: MediaPipe-powered 21-point landmark detection
- **Letter Recognition**: Logistic Regression model for static ASL letters
- **Word Detection**: Random Forest Classifier for dynamic gestures
- **Audio Feedback**: gTTS + pyGame voice output
- **Data Collection**: Live gesture capture for model improvement

## 🚀 Quick Start
```bash
git clone https://github.com/yourusername/sign-language-interpreter.git
cd sign-language-interpreter
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt

# Run modules
python letter_interpreter.py  # For letters
python word_interpreter.py   # For words
```

## 🎮 Controls
| Key | Action |
|-----|--------|
| `q` | Quit |
| `c` | Capture new gesture |

## 🛠 Core Components
- `hand_detector2.py`: MediaPipe hand tracking
- `letter_interpreter.py`: Static letter classification
- `word_interpreter.py`: Dynamic gesture recognition

## 🔮 Roadmap
- [ ] Support full ASL alphabet (including dynamic letters)
- [ ] Expand vocabulary
- [ ] User-specific gesture profiles
- [ ] Mobile app development

> **Note**: Requires Python 3.8+ and a webcam
```

### Key Improvements:
1. **Better Organization**: Clear section headers with emojis
2. **Concise Feature List**: Bullet points instead of paragraphs
3. **Table Format Controls**: Easier to read
4. **Future Plans as Checklist**: More actionable
5. **Removed Redundancies**: Kept only essential technical details
6. **Mobile-Friendly**: Shorter lines and clear formatting

Would you like me to adjust any section further? For example, we could:
- Add a demo GIF/video link
- Include system requirements in detail
- Add contribution guidelines
- Include benchmark results
