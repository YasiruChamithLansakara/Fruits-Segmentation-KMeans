# 🍓 Strawberry-Segmentation-KMeans

This project applies **K-Means image segmentation** on a strawberry image using the **Lab color space** for improved and more realistic color-based clustering.
It includes **multi-K analysis (K=2,3,4,5)**, **cluster masks**, and a fully functional segmentation pipeline.

---

## 📌 Project Features

✔ Segmentation using **K-Means Clustering**
✔ Works in **Lab Color Space** (better than RGB for color-based grouping)
✔ **Multi-K comparison** (2, 3, 4, 5 clusters)
✔ **Cluster masks** for each K
✔ Fully documented **Jupyter Notebook version**
✔ Clean and organized **GitHub folder structure**
✔ Ready-to-use **PDF Reports**

---

## 📁 Repository Structure

```
Fruits-Segmentation-KMeans/
│
├── README.md
├── requirements.txt
├── notebook_version.ipynb
│
├── images/
│   └── strawberry1.jpg
│
├── notebook_outputs/
│   └── strawberry1_20251123_152359/
│       ├── strawberry1_mask_0.png
│       ├── strawberry1_mask_1.png
│       ├── strawberry1_mask_2.png
│       └── strawberry1_segmented_K3.png
│
└── reports/
    └── Image Segmentation - Report.pdf
```

---

## 🚀 How to Run the Project

### 1️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 2️⃣ Run Segmentation (Default K=3)

```bash
python kmeans_segmentation.py --input images/strawberry1.jpg --k 3 --output_dir outputs
```

### 3️⃣ Preview Multiple K Values

```bash
python kmeans_segmentation.py --input images/strawberry1.jpg --preview --k_list 2,3,4,5
```

This will generate outputs such as:

* `strawberry_segmented_K2.png`
* `strawberry_segmented_K3.png`
* Cluster masks for each K
* Multi-K comparison preview grid

---

## 🎨 Example Output Previews

### **Original Image**

*(Place your original strawberry image here once uploaded to GitHub)*

### **Segmented Images**

* **K = 2** → Background vs Strawberry
* **K = 3** → Strawberry, Leaves, Background
* **K = 4–5** → Seeds, Highlights, Shadows (more fine-grained)

### **Cluster Masks**

Each cluster is isolated to show how pixels were grouped.

---

## 📘 Reports Included

Located in the `reports/` folder:

* **Image Segmentation – Report.pdf**

  * Multi-K comparison
  * All masks visualized
  * Full explanations of clustering

---

## 🛠 Technologies Used

* Python
* OpenCV
* NumPy
* Matplotlib
* ReportLab
* Jupyter Notebook

---

## 🧑‍💻 Author

This project was created by **Yasiru Lansakara**,
for the *Higher National Diploma in Computer Science with Artificial Intelligence*.

---

## 📄 License

Licensed under the **MIT License**.

---