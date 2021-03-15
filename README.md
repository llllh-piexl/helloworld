# Some Introduction about Flutter
Flutter is Google's mobile UI tookit launched in 2015,which can help to complete high quality native user interface on the IOS or Android.It was "sky" when was presented  at 
the Dart Developer Summit in May 2015. Flutter was developed using Dart, a new computer programming language launched by Google in 2011.


STRENGTH
Fast development
Since Flutter chooses Dart as its development language, a language can be compiled as either AOT (Ahead Of Time) or JIT (Just In Time). The JIT compilation feature enables 
Flutter to achieve sub-second stateful hot overload In the development stage, thus greatly improving the development efficiency.

Expressive and Flexible UI
Flutter is built with a number of beautiful Material Design and Cupertino (iOS style) widgets that allow developers to quickly build beautiful user interfaces for a better user 
experience.
 
Superior performance
Use its own high-performance rendering engine (SKIA) for self-drawing, rendering speed and user experience is as good as native.


 FRAMEWORK
 The Flutter Framework is divided into three layers: Framework layer, Engine layer and Embedder layer.

Framework layer: This is implemented by Dart, which includes many Android Material and iOS Cupertino Widgets, as well as rendering, animation, drawing and gestures. Framework 
contains a large number of API needed for daily development, ordinary application development is familiar with the use of these API is basically OK, but many special scenes of 
controls need to be customized according to the actual situation.

Engine layer: realized by C/C++, it is the core Engine of Flutter, mainly including Skia graphics Engine, Dart runtime environment Dart VM, Text Text rendering Engine, etc. If 
you want to learn more about Flutter's principles, you are advised to read the source code for this layer.

Embedder layer: It handles platform-specific operations such as rendering Surface Settings, local plugins, packaging, threading, and so on.


PRINCIPLE
Both iOS and Android provide a platform View to the Flutter layer, and the rendering of page content is completed by the Flutter layer itself.
The general process is as follows:
The GPU's VSYNC signal is synchronized to the UI thread
The UI thread uses Dart to build an abstract view structure
The view structure is composed of layers in the GPU thread
The resultant view data is provided to the Skia graphics engine for processing into GPU data
The data is then fed to the GPU via OpenGL or Vulkan for rendering
