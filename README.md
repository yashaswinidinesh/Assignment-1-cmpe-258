# CMPE 258 - Assignment 1: AI/ML Projects

**Author:** Yashaswini Dinesh  
**Course:** CMPE 258 - Deep Learning  
**University:** San Jose State University

---

## Assignment Overview

| Assignment | Description | Demo Video |
|------------|-------------|------------|
| 1A | Multimodal AI with Google Gemini | [Watch Demo](https://www.youtube.com/watch?v=IjBQ1fu7_zc) |
| 1B | Full Stack Web App (Antigravity) | [Watch Demo](https://youtu.be/VIDEO_ID_HERE) |
| 1C | Flutter Mobile App (Antigravity) | [Watch Demo](https://youtu.be/VIDEO_ID_HERE) |
| 1D | MNIST Neural Network Classifier | [Watch Demo](https://youtu.be/VIDEO_ID_HERE) |

---

## 1A: Multimodal AI with Google Gemini

**Colab Notebook:** `1A/258_Assignment_1A_Yashaswini.ipynb`

**Demo Video:** [https://youtu.be/VIDEO_ID_HERE](https://youtu.be/VIDEO_ID_HERE)

### What it does:
- Text-to-Image generation using Imagen 3
- Text-to-Video generation using Veo 2
- Image analysis with detailed insights
- Multi-turn conversational chat

### How to run:
1. Open notebook in Google Colab
2. Get API key from https://aistudio.google.com/apikey
3. Paste key in Section 2 where it says YOUR_API_KEY_HERE
4. Run all cells
5. Upload any image for analysis

### Technologies:
- Google Gemini 2.0 Flash
- Imagen 3 (image generation)
- Veo 2 (video generation)
- Python, PIL, Matplotlib

---

## 1B: Full Stack Web App - Flashcard Forge

**Colab Notebook:** `1B/258_Assignment_1B_Yashaswini.ipynb`

**Demo Video:** [https://youtu.be/VIDEO_ID_HERE](https://youtu.be/VIDEO_ID_HERE)

### What it does:
- AI-powered flashcard generation
- User authentication
- Study mode with card flipping
- Progress tracking

### Built with Antigravity:
- Used Google Antigravity to generate the full stack app
- Natural language prompt to code generation

### Technologies:
- Frontend: Next.js + TypeScript + Tailwind CSS
- Backend: Firebase Authentication + Firestore
- AI: Google Gemini API
- Hosting: Firebase Hosting

### Project Structure:
```
1B/
  web/              Next.js application
    src/
      app/          Pages and API routes
      components/   UI components
      lib/          Firebase config
  firebase/         Firebase configuration
  docs/             Documentation
```

---

## 1C: Flutter Mobile App - Receipt2Split

**Colab Notebook:** `1C/258_Assignment_1C_Yashaswini.ipynb`

**Demo Video:** [https://youtu.be/VIDEO_ID_HERE](https://youtu.be/VIDEO_ID_HERE)

### What it does:
- AI receipt scanning with Gemini Vision
- Bill splitting among friends
- Automatic tax and tip calculation
- Split history saved locally

### Built with Antigravity:
- Used Google Antigravity to generate Flutter app
- Cross-platform: iOS, Android, Web, Desktop

### Technologies:
- Framework: Flutter (Dart)
- AI: Google Gemini Vision API
- State Management: Provider
- Storage: Hive (local database)

### Project Structure:
```
1C/
  app/              Flutter application
    lib/
      models/       Data models
      screens/      UI screens
      services/     API services
      providers/    State management
  docs/             Documentation
```

---

## 1D: MNIST Neural Network Classifier

**Colab Notebook:** `1D/258_Assignment_1D_Yashaswini.ipynb`

**Demo Video:** [https://youtu.be/VIDEO_ID_HERE](https://youtu.be/VIDEO_ID_HERE)

### What it does:
- Loads MNIST handwritten digit dataset
- Trains baseline model (Dense layers) - ~97% accuracy
- Trains CNN model (Conv2D layers) - ~99% accuracy
- Generates all evaluation metrics

### How to run:
1. Open notebook in Google Colab
2. Enable GPU: Runtime -> Change runtime type -> GPU
3. Run all cells
4. Download outputs zip file

### Output files generated:
```
outputs/
  plots/
    mnist_samples.png
    baseline_training_curves.png
    cnn_training_curves.png
    confusion_matrix.png
    prediction_grid.png
  metrics/
    confusion_matrix.txt
    classification_report.txt
  models/
    mnist_cnn.keras
```

### Technologies:
- TensorFlow / Keras
- Scikit-learn (metrics)
- Matplotlib (visualization)
- NumPy

---

## How to Use This Repository

### For Colab Notebooks (1A, 1B, 1C, 1D):
1. Download the notebook file
2. Go to https://colab.research.google.com
3. File -> Upload notebook
4. Follow instructions in each notebook

### For Web App (1B):
```bash
cd 1B/web
cp .env.example .env.local
# Add your Firebase and Gemini credentials
npm install
npm run dev
```

### For Flutter App (1C):
```bash
cd 1C/app
cp .env.example .env
# Add your Gemini API key
flutter pub get
flutter run
```

---

## References

- Google AI Studio: https://aistudio.google.com/
- Google Antigravity: https://antigravity.google/
- Firebase: https://firebase.google.com/
- Flutter: https://flutter.dev/
- TensorFlow: https://www.tensorflow.org/
- Janus Pro: https://www.datacamp.com/blog/janus-pro
- DeepSeek R1: https://www.datacamp.com/blog/deepseek-r1

---

CMPE 258 - Deep Learning - San Jose State University
