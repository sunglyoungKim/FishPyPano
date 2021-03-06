# FishPyPano
Stitch two fish eye images to get 360° panorama

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/ranadeepb)

FishPyPano works with ***Mi Sphere dual*** fisheye photos. I intend to make it work for any dual fisheye images.

It takes two >180° HFOV/VFOV fisheye images and stitches them.

### Comparison
![FishPyPano Comparison](https://raw.githubusercontent.com/rnbdev/FishPyPano/master/img/comparison.jpg)

### Setup
Before running, set up requirements, executing `pip install -r requirements.txt`

### Running
The code offers two functions.
1. Calibrate - `python calibrate.py` You have to do this one time. You give a list of matched points in the image from JSON file and it calibrates the lens parameters. After calibration it will generate a json file with the calibrated parameters.
   - I have cooked up a [html](https://codepen.io/ranadeep/full/XVaPwy/) page which you can use to generate the json file.
2. Stitch - `python stitch.py` Pass the image and wait for the magic.


#### Contribute
Feel free to fork. Pull requests are most welcome. For any suggestion, open an issue.

### Thank you
[Chris Pebble](https://www.facebook.com/chris.pebble.1) for suggesting distortion functions.
