# Dataset_Maker_Anime

# Image Dataset Preparation and Analysis Scripts

These scripts are designed to assist in preparing, analyzing, tagging, and curating image datasets for various purposes. The collection includes multiple functionalities to streamline the dataset preparation process and enhance the quality of your dataset.

## Prerequisites

- Python 3
- Google Colab (optional but recommended for efficient processing)
- Google Drive (for storage and organization)
- A folder containing your image dataset

## Author

[Your Name]

Feel free to modify and use these scripts according to your needs.

---

## Image Preprocessing Script

This script is designed to preprocess a collection of images in a specified input directory and save the resized images to an output directory. It uses the OpenCV library to resize images to a fixed size (512x512 pixels) and supports image formats such as JPG, PNG, and WEBP.

### Usage

1. Place the images you want to process in the `input_directory`.
2. Run the script.

### How it works

The script performs the following steps:

1. Checks if the `output_directory` exists and creates it if it doesn't.
2. Iterates through all files in the `input_directory`.
3. For each image file (with extensions `.jpg`, `.png`, or `.webp`), it does the following:
   - Loads the image using OpenCV.
   - Resizes the image to 512x512 pixels.
   - Saves the resized image to the `output_directory`.
   - Prints a message indicating the image has been resized and saved.

---

## Image Dataset Cleanup Script

This script is designed to help you clean up and curate an image dataset by identifying and removing duplicate or unwanted images. It utilizes the FiftyOne library and a pre-trained CLIP model to find and mark similar images for deletion. Additionally, it provides an interactive interface for manual curation.

### Usage

### 1️⃣ Setup

1. Run the script, and it will guide you through the setup process.
2. Provide a unique project name (avoid spaces) and choose your desired folder structure for organizing your dataset.
3. The script will create the necessary folders in your Google Drive or local directory, depending on whether you're using Google Colab.
4. Once the setup is complete, you'll be ready to proceed with dataset curation.

### 3️⃣ Curate Your Images

1. The script will analyze your dataset to find duplicate images based on a similarity threshold you specify.
2. It will automatically mark similar images for deletion.
3. An interactive interface will be provided for manual curation, allowing you to review and mark images for deletion as needed.
4. You can visualize images, enable "sample tags" to see which ones are marked for deletion, and manually tag images as "delete" if necessary.
5. After curating your dataset, save your changes by entering something in the input box.
6. The script will remove the marked images and save the curated dataset.

---

## Image Dataset Tagging and Curation Script

This script is designed to assist in tagging and curating an image dataset. It offers functionalities for automated tagging using AI models and manual curation of tags.

### Usage

### 1️⃣ Setup

1. Run the script, and it will guide you through the setup process.
2. Provide a unique project name (avoid spaces) and choose your desired folder structure for organizing your dataset.
3. The script will create the necessary folders in your Google Drive or local directory, depending on whether you're using Google Colab.
4. Once the setup is complete, you'll be ready to proceed with dataset curation.

### 4️⃣ Tag Your Images

#### Anime Tags

- Choose the "Anime tags" option.
- Set a tag threshold (confidence level) for including tags.
- Optionally, specify tags to blacklist, which will be excluded from tagging.
- The script will automatically tag your images with relevant labels.

#### Photo Captions

- Choose the "Photo captions" option.
- Set the minimum and maximum length of captions for your images.
- The script will generate captions for your images, enhancing their metadata.

### 5️⃣ Curate Your Tags

This step allows you to modify and refine the tags in your dataset.

- Specify global activation tags that will be added to the start of every text file.
- Remove unwanted tags or duplicates.
- Search for specific tags and replace them with new tags.
- Optionally, sort tags alphabetically and remove duplicate activation tags.
- Review the changes made to your tags.

---

## Lora Dataset Preparation and Analysis Script

This script is designed to assist in preparing and analyzing datasets for training Lora, a language model. It offers various functionalities to streamline the dataset preparation process.

### Usage

### 1️⃣ Setup

1. Run the script, and it will guide you through the setup process.
2. Provide a unique project name (avoid spaces) and choose your desired folder structure for organizing your dataset.
3. The script will create the necessary folders in your Google Drive or local directory, depending on whether you're using Google Colab.
4. Once the setup is complete, you'll be ready to proceed with dataset curation.

### 6️⃣ Ready

This section prepares your dataset for Lora training and provides a link to the Lora trainer.

### 📈 Analyze Tags

- View the top tags in your dataset, helping you understand its content better.

### 📂 Unzip Dataset

- Upload a zip file containing your dataset and extract it to your Google Drive for easier access.

### 🔢 Count Datasets

- Count the number of files (images, captions, and others) in all folders and subfolders of your project folder.

### 🚮 Clean Folder

- Delete all non-image files in the project folder, ensuring that only relevant data is retained.

---


