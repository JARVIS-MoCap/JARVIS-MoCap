# JARVIS - 3D Motion Capture Toolbox

JARVIS makes highly precise markerless 3D motion capture easy. All you need to get started is a multi camera recording setup and an idea of what you want to track. 
Our Toolbox will assist you on every step along the way, from recording synchronised videos, to quickly and precisely annotating your data, 
all the way to the final 3D pose predictions.\
If you are interested in setting up a 3D Motion Capture System or just want to learn more about our toolbox we strongly recommend having a look at our 
[Getting Started Guide](gettingstartd.md). Here you'll find an overview of our workflow as well as tutorials to help you build a succesfull 3D traking pipeline with JARVIS.

## Why JARVIS?
Image based markerlerss motion capture has become an essential data analysis tool in many fields of research, pinoeered largely by DeepLabCut several years ago. 
While there have been significant improvements to those methods both in terms of capabilities and usability, those advances mainly tackle single image based 
2D tracking. Setting up a system for multi camera 3D motion capture on the other hand still remains very challenging and time consuming.\
JARVIS tries to change that by introducing an easy to use toolchain that was developed with highly precise 3D Tracking as the sole goal, not just an afterthought.\
Our System consists of three parts:\
- The **Acquisition Tool** allows you to record synchronised videos from multiple views at hight FPS thanks to GPU accelerated online JPEG compression. If you use FLIR cameras you can get your system setup and running with just a handful of clicks.
- The **Annotation Tool** leverages the fact that you record with multiple cameras at once by projecting your annotations in a subset of those cameras to 
  the remaining ones, significantly reducing the ammount of tedious manual annotations needed. It also provides easy-to-use interfaces for calibrating your cameras 
  and creating datasets.
- The **HybridNet Pytorch Library** is our state of the art 3D pose estimation architecture. Our hybrid 2D/3D CNN architecture is faster to train, more precise and most importantly can run on siginficantly smaller dataset sizes than pure 3D CNNs, saving you countless hours of mind numbing annotations while still achieving highly precise markerless motion capture - even in scenarios with heavy occlusion.
