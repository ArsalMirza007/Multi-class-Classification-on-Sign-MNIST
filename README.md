# Multi-class-Classification-on-Sign-MINST

# Instructions:
Here's the list of tasks performed in the provided code with the headings bolded:

**1. Import necessary libraries:**
   - `csv`: For parsing CSV files.
   - `string`: For accessing ASCII letters.
   - `numpy`: For numerical operations and array handling.
   - `tensorflow`: For building and training neural networks.
   - `matplotlib.pyplot`: For plotting images.
   - `tensorflow.keras.preprocessing.image.ImageDataGenerator, array_to_img`: For generating image data batches and converting arrays to images.

**2. Install required packages:**
   - `gdown`: Version 4.6.0 for downloading files from Google Drive.

**3. Download the training and test datasets using Google Drive IDs.**

**4. Define global variables:**
   - `TRAINING_FILE`: Path to the training CSV file.
   - `VALIDATION_FILE`: Path to the validation CSV file.

**5. Define a function `parse_data_from_input(filename)` to parse images and labels from a CSV file.**

**6. Implement the `parse_data_from_input(filename)` function:**
   - Open the CSV file.
   - Use `csv.reader` to read the file.
   - Skip the header row.
   - Extract labels and pixel values for each image.
   - Reshape pixel values to a 28x28 array.
   - Convert the data type to `float64`.
   - Return the images and labels as numpy arrays.

**7. Test the `parse_data_from_input(filename)` function by parsing training and validation datasets.**

**8. Define a function `plot_categories(training_images, training_labels)` to plot sample images with their corresponding labels.**

**9. Plot a sample of 10 images from the training set using `plot_categories(training_images, training_labels)`.**

**10. Define a function `train_val_generators(training_images, training_labels, validation_images, validation_labels)` to create training and validation data generators.**

**11. Implement the `train_val_generators(training_images, training_labels, validation_images, validation_labels)` function:**
    - Add an extra dimension to the images array.
    - Instantiate `ImageDataGenerator` for training data with data augmentation parameters.
    - Create a training data generator using `ImageDataGenerator.flow()`.
    - Instantiate `ImageDataGenerator` for validation data without data augmentation.
    - Create a validation data generator using `ImageDataGenerator.flow()`.

# Screenshots:
![arr](https://github.com/ArsalMirza007/Multi-class-Classification-on-Sign-MINST/assets/121928372/8d1ea47e-039e-4639-95c9-59a766346bb7)
![training](https://github.com/ArsalMirza007/Multi-class-Classification-on-Sign-MINST/assets/121928372/4c8e8b7f-2d1b-4e87-ad28-37b0b328c443)
![loss](https://github.com/ArsalMirza007/Multi-class-Classification-on-Sign-MINST/assets/121928372/dfd5c079-50ff-4d83-a2f6-480f3bde3fb7)
