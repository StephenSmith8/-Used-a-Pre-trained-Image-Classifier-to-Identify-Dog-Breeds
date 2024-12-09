<h1>Using-a-Pre-trained-Image-Classifier-to-Identify-Dog-Breeds</h1>

<h2>Project Overview</h2>
For this project, I focused on developing an image classification solution that involved identifying whether pet images were of dogs or not, and, if the image was of a dog, classifying the breed correctly. To achieve this, I explored different CNN architectures (ResNet, AlexNet, and VGG), testing their performance based on the project objectives and evaluating their efficiency in terms of runtime. I also considered whether using a less resource-intensive solution could provide a "good enough" result given the time constraints.

<h2>Key Objectives:</h2>
<ol>
<li>Identify dog images: Classify each image as either a "dog" or "not a dog," even if the breed is misclassified.</li>
<li>Classify dog breeds: For images identified as dogs, accurately classify the breed.</li>
<li>Evaluate CNN model architectures: Test ResNet, AlexNet, and VGG to determine which model best achieves the objectives above.</li>
<li>Time efficiency: Consider the time taken by each model to achieve the results and decide whether an alternative solution would suffice.</li>
</ol>
<h2>Tasks Completed:</h2>
<ol>
<h3><li>Image Classification (Dog vs. Non-Dog):</li></h3>
I developed functions within check_images.py to process pet images and correctly identify whether each image was of a dog or not. I used the provided dognames.txt file to match the labels, and ensured that even if a breed was misclassified, the image would still be categorized as a "dog."

<h3><li>Breed Classification for Dogs:</li></h3>
For images identified as dogs, I integrated a classifier function to determine the breed of the dog. This involved using the pretrained CNN models (ResNet, AlexNet, and VGG), which I implemented in the check_images.py script.

<h3><li>Model Evaluation:</li></h3>
I tested each of the three CNN architectures—ResNet, AlexNet, and VGG—to determine which model provided the best performance. This included evaluating the accuracy of dog vs. non-dog classification as well as breed classification accuracy.

<h3><li>Time Analysis:</li></h3>
I implemented timing functionality using Python's time module to measure the runtime of each model. After evaluating the models’ performance, I considered whether a simpler model could have produced "good enough" results in less time, making recommendations based on the trade-offs between accuracy and runtime.

<h3><li>Result Calculation and Output:</li></h3>
I compared the classifier labels to the pet image labels, using a dictionary structure to store the pet labels, classifier results, and their comparison. I calculated how well the algorithm performed in classifying the images and printed a summary of the results, including the total number of images classified correctly as dogs, the breed classification accuracy, and the overall runtime.

<h3><li>Iterative Development and Testing:</li></h3>
I edited and debugged check_images.py, incorporating the provided TODO comments and hints. I tested the implementation repeatedly, refining the code as I progressed. I also utilized helper functions from other files like print_functions_for_lab_checks.py to verify specific parts of the project.

<h3><li>Command-Line Input Handling:</li></h3>
I integrated command-line arguments to allow users to provide inputs dynamically, such as specifying image files for classification or choosing the model architecture to use. This flexibility ensured that the program could be run with different inputs and configurations.
<br />

<h2>Conclusion:</h2>

By the end of the project, I had a fully functioning solution that not only identified whether pet images were of dogs or not but also classified the dog breeds with high accuracy. Additionally, I provided performance insights and recommendations based on runtime considerations for each model architecture.
</ol>
