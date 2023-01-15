# 23-01-aritziagirlcode

01/13~01/14 UBC GirlCode Hackathon project: Capsule Closet
Input an image, produce the season color that suits the skin tone the best.

# File Structure:

part1-train model for classification
files: 
 - step1-processdata.ipynb
 --> process the csv file, turn rgb into hsv, manually label 123 dataset
 - step2-training.ipynb
 --> use svm to train the data, map the image to its corresponding seasonal color type
output: 
 - datall.csv: the file that contains the processed csv file
 - model.pickle: the trained model
data source: skin tone dataset: https://github.com/the-pudding/data/blob/master/vogue/models.csv

part2:implement the model
files:
 - wholeline.ipynb
 --> Input an image, output its image with color palette on top.
face detection framework: https://google.github.io/mediapipe/solutions/face_detection.html

additional part: the color for four classes
files:
 - autumn.jpg: the color palette picture for autumn
 - spring.jpg: the color palette picture for spring
 - summer.jpg: the color palette picture for summer
 - winter.jpg: the color palette picture for winter
 - d-getrgb.ipynb: function that converts the above .jpg into a list of (r,g,b) values
output:
 - mapseason.pickle: the dictionary that maps season to its corresponding list of 3 (r,g,b) colors




