## Task: Lungs detection in grayscale x-ray images

##### Preprocessing
* Apply Gaussian blur
* Apply opencv's AddWeight function (to increase grayscale contrast)
* Thresholding (Grayscale -> binary)

##### Identify lungs area
* Find Contours 
  * different contours will be formed including parts such as trachea and skull, as well as background noise
  * contours near image edges as well as contour < 2% of images are removed
* Draw lungs area

##### Evaluation
* Compare the similarity of lungs area with ground-truth by computing Euclidean distance

![alt text](https://raw.githubusercontent.com/leeshien/Visual-Information-Processing/master/visualize_result.JPG)
