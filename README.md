🖼️ Image Augmentation & Visualization with Keras + TensorFlow
🚀 This project demonstrates how to perform image data augmentation using TensorFlow’s ImageDataGenerator and visualize the effects in a clear side-by-side format. It loads a single input image and generates multiple augmented variations to help you better understand and debug your augmentation pipeline.

✨ Features
✅ Load and preprocess a single input image
🔄 Apply powerful image augmentation techniques:
🔃 Rotation
↔️ Width shift
↕️ Height shift
🔄 Shearing
🔍 Zoom
🔁 Horizontal flip
🖼️ Visualize the original image vs. augmented images in a two-column layout
📊 Enhance your deep learning pipeline with synthetic image variation

💡 Why Use Image Augmentation?
Image augmentation is essential for training robust deep learning models. It helps:
🧠 Prevent overfitting
🎯 Improve generalization
🎨 Simulate real-world image variations
📈 Improve model performance with less data

🗂️ Project Structure
bash
Copy
Edit
.
├── shihtzu.jpg             # 🐶 Input image
├── augment_visualize.py    # 🧪 Main Python script
├── README.md               # 📘 Project documentation
⚙️ Requirements

📦 Install the required libraries using:

pip install tensorflow matplotlib numpy
✅ Python 3.x
✅ TensorFlow 2.x
✅ NumPy
✅ Matplotlib

▶️ How to Run
🖼️ Add your image and name it shihtzu.jpg (or modify the path in the script).

🏃‍♂️ Run the script:

python augment_visualize.py
🪟 A window will appear showing the original image in the left column and 10 augmented versions in the right column.

🧠 Code Overview
🔧 Augmentation Config:

python
Copy
Edit
datagen = ImageDataGenerator(
    rescale=1./255,
    rotation_range=20,
    width_shift_range=0.2,
    height_shift_range=0.2,
    shear_range=0.2,
    zoom_range=0.2,
    horizontal_flip=True,
    fill_mode='nearest'
)
🎨 Visualization:

python
Copy
Edit
visualize_original_and_augmented(img, augmented_images, 10)
Generates a 2-column view: original (left) and augmented (right), repeated for 10 variations.

📄 License
📝 MIT License – Free to use, modify, and share!

🤝 Contributing
🎉 Contributions are welcome!
📬 Feel free to open issues or pull requests for improvements, fixes, or new features.

🙋‍♀️ Let's Connect
💬 For questions, suggestions, or feedback, feel free to reach out or open an issue!
