- [A Standardized Approach for Skin Detection: Analysis of the Literature and Case Studies](https://www.notion.so/lecture-1-d545272ec7514ba1a59cd09edbe33d70?pvs=21)
- [Human skin detection: An unsupervised machine learning way](https://www.sciencedirect.com/science/article/pii/S1047320324000014#baep-article-footnote-id1)
- [Skin Detection - a Short Tutorial](https://people.cs.rutgers.edu/~elgammal/pub/skin.pdf)
- [Skin detection Tutorial Medium](https://medium.com/@madadihosyn99/skin-detection-using-hls-color-space-b73114de076b)
  
- Sampling and Quantization
    - https://wimarshikathamali1995.medium.com/sampling-quantization-in-digital-image-processing-8c4490357039
    - https://dev.to/haratena9/memorandum-image-processing-1-pixels-quantization-and-sampling-1n02
    
    ### 1. **Sampling:**
    
    - **Definition**: Sampling refers to the process of converting a continuous image (analog) into a discrete image (digital) by measuring the image's intensity at regular intervals.
    - **How it works**: An image can be thought of as a continuous signal in two dimensions (x and y coordinates). To digitize it, the image is sampled at specific points, usually arranged in a grid. Each sample represents a pixel in the digital image.
    - **Impact**: The spacing of these samples determines the resolution of the image. Higher sampling rates (more pixels per unit area) result in higher resolution images with more detail, while lower sampling rates result in lower resolution images with less detail.
    
    ### 2. **Quantization:**
    
    - **Definition**: Quantization refers to the process of mapping a large set of continuous amplitude values (intensity or color values) to a smaller set of discrete values.
    - **How it works**: Once an image is sampled, each sample (pixel) has an intensity value, often representing the color or brightness. Since digital systems can only store a finite number of values, these continuous values must be rounded off to the nearest available value in a predefined set. This set could be, for instance, 256 levels of gray in an 8-bit grayscale image.
    - **Impact**: The number of discrete levels available is determined by the bit depth of the image. A higher bit depth allows for more levels and more accurate representation of the original image. Lower bit depth results in more noticeable quantization errors, such as banding in gradients.
    
    ### Example in Practice:
    
    - Consider an analog grayscale image. When you sample it, you decide on a grid (like 100x100 pixels), and measure the brightness at each of those grid points. That’s sampling.
    - Then, for each measured brightness (which could theoretically have any value within a range), you assign it to one of 256 possible values (if you’re using 8-bit quantization). This rounding-off process is quantization.
    
    ### Importance in Computer Vision:
    
    - **Sampling** affects the spatial resolution of an image, which is crucial for tasks like object detection, where fine details might be important.
    - **Quantization** affects the color or intensity resolution, impacting how accurately the visual content is represented. It can also affect the performance of algorithms, particularly in tasks that rely on subtle color or intensity variations.
    - Skin detection
    - bitwise operations in CV