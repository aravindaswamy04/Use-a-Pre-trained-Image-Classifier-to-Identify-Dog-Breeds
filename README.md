# Use-a-Pre-trained-Image-Classifier-to-Identify-Dog-Breeds
# Project Overview
The project "Use a Pre-trained Image Classifier to Identify Dog Breeds" involves leveraging pre-trained convolutional neural networks (CNNs) to classify pet images as either dog or not dog, and to further identify the specific breed of the dogs. The main objectives are to accurately identify dog images, correctly classify dog breeds, compare the performance of different CNN architectures (ResNet, AlexNet, VGG), and consider the computational efficiency of these models.

Principal Objectives
Identify Dog Images: The project aims to correctly identify which pet images contain dogs, even if the breed is misclassified.
Classify Dog Breeds: For images identified as dogs, the project aims to correctly classify the breed of the dog.
Evaluate CNN Architectures: The project compares three CNN model architectures (ResNet, AlexNet, and VGG) to determine which one best achieves the above objectives.
Consider Computational Efficiency: The project also considers the time resources required by each model to achieve the objectives and evaluates if an alternative solution could provide a "good enough" result in a shorter time.
Project Structure
Main Program: check_images.py
The primary script for this project is check_images.py, which contains a main() function. This function outlines the overall workflow and calls several undefined functions that you will need to implement.

Detailed Steps
1. Time the Program
Use the Time module to compute the total runtime of the program. This helps in evaluating the computational efficiency of the models.
2. Get Program Inputs
Use command line arguments to get user inputs. This allows flexibility in specifying different parameters without changing the code.
3. Create Pet Image Labels
Extract labels from the pet image filenames and store these labels in a dictionary for easy access.
4. Create Classifier Labels and Compare Labels
Use the provided classifier function to generate labels for the images.
Compare the generated classifier labels with the actual pet image labels.
Store the pet labels, classifier labels, and their comparisons in a dictionary of lists.
5. Classify Labels as "Dogs" or "Not Dogs"
Use a list of dog names from dognames.txt to classify all labels as "Dogs" or "Not Dogs".
Update the dictionary of lists with these new classifications.
6. Calculate the Results
Evaluate the performance of the algorithm by calculating various metrics such as accuracy, precision, recall, and F1 score.
Determine how well the algorithm worked in classifying the images.
7. Print the Results
Display the results for each of the three image classification algorithms (ResNet, AlexNet, VGG).
Implementing Functions
The check_images.py file contains comments with # TODO: indicating where to implement specific functions. Below are descriptions of the key functions you need to define:

1. get_pet_labels()
Input: Directory containing pet images.
Output: Dictionary with filenames as keys and pet image labels as values.
Description: This function reads the filenames in the specified directory, extracts the labels, and stores them in a dictionary.
2. classify_images()
Input: Directory containing pet images and a pre-trained model architecture.
Output: Dictionary with filenames as keys and classifier labels as values.
Description: This function uses the pre-trained model to classify each image and stores the results in a dictionary.
3. compare_labels()
Input: Dictionary with pet labels and dictionary with classifier labels.
Output: Dictionary with filenames as keys and comparison results as values.
Description: This function compares the pet labels with the classifier labels and stores the comparison results.
4. adjust_results4_isadog()
Input: Dictionary with comparison results and a list of dog names.
Output: Dictionary updated with "Dog" or "Not Dog" classifications.
Description: This function classifies each label as "Dog" or "Not Dog" based on the list of dog names and updates the dictionary.
5. calculates_results_stats()
Input: Dictionary with updated comparison results.
Output: Dictionary with calculated statistics.
Description: This function calculates various performance metrics such as accuracy, precision, recall, and F1 score.
6. print_results()
Input: Dictionary with calculated statistics and the total runtime.
Output: Printed results.
Description: This function prints the calculated statistics and the total runtime of the program.

Results:
By implementing the above functions and following the outlined steps, you will be able to classify pet images and evaluate the performance of different CNN architectures. The results will include the total runtime, number of correctly classified dog images, number of correctly classified non-dog images, and the number of correctly classified dog breeds.
