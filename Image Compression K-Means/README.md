## **Image Compression with k-means implemented from scratch**
In a colored image, each pixel has a size 3 bytes (RGB), where each color can have intensity values from 0 to 255. As humans, we can only practically visualize a few colors in an image. Image compression takes advantage of the visual perception of the human eye by using only the most prominent colors of an image to represent the image with all of its original (full) colors. By reducing the number of colors needed to represent the image, you also decreases the size of the image file. This project implements the k-means algorithm from scratch to demonstrate how it can be used to compress images using their most prominent colors while maintaining the perception of the full-color, original image.

Images (k=2, k=3, k=4, k = 5, full img)

## **k-means algorithm**
k-means is an unsupervised clustering algorithm, 

#### **Key Algorithm Takeaways:**
- Every intialization of the k-means algorithm may lead to different results
    - Since the k-means objective function is non-convex, we cannot guarantee that any particular local minimum found is a global minimum. Therefore, k-means may converge to different local minima on different runs, given a particular initialization (starting point). Sometimes different intializations may lead to different results, since one could find specific intializations that lead to the same results. 

- The k-means algorithm will converge in a finite number of iterations
    - At some point, the k-means algorithm will converge - it cannot run forever. Becasuse there is a fixed number of data points, there is a limit to the number of total combinations of cluster assignments. The k-means algorithm will always try to reduce a specific metric, but after many iterations it will converge to a point where it can no longer decrease that metric any further.

#### **Math of k-means clustering**
