🧪 Lab 5 – Spatial Filtering (Smoothing & Sharpening)
📚 Course Information
Course: ARTI 406 – Image Processing
Department: Computer Engineering
University: Imam Abdulrahman Bin Faisal University
🎯 Objective

This lab demonstrates fundamental spatial filtering techniques including:

Image smoothing using Box and Gaussian filters
Image sharpening using Laplacian filtering

All tasks are implemented using Python and OpenCV.

🛠️ Tools & Technologies
Python 3
OpenCV (cv2)
NumPy
Matplotlib
📂 Project Structure
lab5/
│── Images/
│    └── cat.jpg
│
│── main.py (or notebook)
│── task1_box_filter.png
│── task2_gaussian_filter.png
│── task3_laplacian_sharpening.png
│── README.md
🧩 Tasks Overview
🧩 Task 1 – Box Filter Smoothing
Apply a 7×7 box (averaging) filter
Implemented using cv2.filter2D()
Output:
Original image
Smoothed image

📌 Result saved as:
task1_box_filter.png

🚀 Task 2 – Gaussian Filtering
Apply:
5×5 Gaussian filter (mild smoothing)
21×21 Gaussian filter (strong smoothing)
Implemented using cv2.GaussianBlur()

📌 Output:

Original image
5×5 filtered image
21×21 filtered image

📌 Result saved as:
task2_gaussian_filter.png

🔪 Task 3 – Laplacian Sharpening

Steps performed:

Read image
Convert to float32
Apply 3×3 Laplacian filter using cv2.Laplacian()
Sharpen using:
sharpened = np.clip(image_float - laplacian, 0, 1)

📌 Output:

Original image
Laplacian result
Sharpened image

📌 Result saved as:
task3_laplacian_sharpening.png

⚙️ Program Execution

Run the script:

python main.py

The program will:

Execute all 3 tasks sequentially
Display results
Save output images automatically
🧠 Key Concepts
📦 Box Filter
Simple averaging filter
Reduces noise but blurs edges
🌀 Gaussian Filter
Weighted smoothing (center pixels have higher importance)
Produces more natural blur than box filter
🔪 Laplacian Filter
Detects edges using second-order derivatives
Enhances details when subtracted from the original image
📊 Results Summary
Increasing kernel size increases smoothing strength
Gaussian filtering preserves image quality better than box filtering
Laplacian filtering enhances edges and sharpens the image
📌 Notes
All images are loaded from: Images/cat.jpg
Output images are saved automatically using matplotlib
Error handling included for missing image file