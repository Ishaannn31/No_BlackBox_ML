

---

# No Black Box Machine Learning: Drawing Classifier (Phase 1)

A JavaScript-based machine learning project where we build a drawing recognition system **from scratch** (no ML libraries). This phase covers data collection, processing, and visualization.

**Course**: [YouTube Playlist](https://www.youtube.com/playlist?list=PLB0Tybl0UNfYoJE7ZwsBQoDIG4YN9ptyY) by Radu Mariescu-Istodor.

---

## 🚀 Features Implemented (So Far)

1. **Drawing App (Data Collection)**  
   - Web-based sketchpad with undo/save functionality.  
   - Collects drawings (8 categories: car, fish, house, etc.) and saves them as JSON.  
   - Works on both desktop and mobile.  

2. **Data Processing (Node.js)**  
   - Converts raw drawings into a structured dataset (one JSON file per drawing).  
   - Generates PNG thumbnails of drawings using `node-canvas`.  

3. **Feature Extraction**  
   - Extracts basic features (e.g., `pathCount`, `pointCount`) from drawings.  

4. **Data Visualization**  
   - Interactive web app (`viewer.html`) to explore the dataset:  
     - Table view grouped by student.  
     - Scatter plot to visualize features (custom chart implementation).  
     - Click-to-highlight samples between the plot and table.  

---

## 🛠️ Tech Stack  
- **Frontend**: HTML/CSS/JavaScript (Vanilla JS)  
- **Backend**: Node.js (for data processing)  
- **Key Libraries**:  
  - `node-canvas` (for generating PNGs)  
  - Custom chart library (replaces Google Charts)  

---

## 🔧 Setup & Run  

1. **Install Node.js**: Required for data processing.  
   ```bash
   npm install
   ```

2. **Generate Dataset**:  
   ```bash
   cd node
   node datasetGenerator.js    # Processes raw drawings
   node featureExtractor.js   # Extracts features
   ```

3. **Run Web Apps**:  
   - Open `web/creator.html` to collect new drawings.  
   - Open `web/viewer.html` to explore the dataset.
   - I have also added both to `index.html` , so see the github page


---

## 📜 Credits  
- **Course**: Radu Mariescu-Istodor ([YouTube](https://www.youtube.com/@radu)).  
- **Dataset**: Drawings collected from course participants.  

---

## 📌 Next Steps (Phase 2)  
- Implement k-Nearest Neighbors (k-NN) classifier.  
- Add data scaling and decision boundaries.  
- Build a real-time drawing recognizer.  

---

