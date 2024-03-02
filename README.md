# Image-to-Text-Conversion-and-Extraction
Uses keras_ocr and opencv to detect text and convert it into editable format.
Optical Character Recognition (OCR), a field of study combining computer vision, artificial intelligence, and pattern recognition, is the main driver of this technology. With the use of optical character recognition (OCR) technology, computers can identify text contained in digital images, such as scanned documents, photos of documents, or video frames, and transform it into a digital text format that can be edited, searched, stored, and handled.
Key Components:
1. Libraries: Increasing the quality of the image to aid in text recognition. Using Libraries such as keras_ocr and Open_cv is used to detect text areas in the image.
2. Text Detection:Producing predictions and the position of the image using subplots and predictions obtained through keras ocr.
3. Post-processing: The output thus obtained is then sorted by finding distance of the text from the origin and then inserting it into a dataframe.
4. Functions in the main FILE
1. Process_image(images): Takes a list of path of images to process and using pipeline object predicts the string and position of the text on the image. Also, usessubplots to draw boxes around the text
2. get_distance(predictions): It takes the predictions obtained using pipeline and will return a dictionary of text, its centre coordinates, and distance from origin and distance between origin and y-ordinate.
3. distingush_rows(list, threshold_value): takes two parameters first is list of the dictionary obtained using get_distance and second is a threshold value used to determine the rows uniquely.
4. Lastly the obtained predictions will be appended in a list or dictionary.
