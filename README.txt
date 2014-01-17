******************************************************************************
*   Face Recognition using Eigenfaces or Fisherfaces
******************************************************************************
*   by Shervin Emami, 5th Dec 2012
*   http://shervinemami.info/openCV.html
******************************************************************************
*   Ch8 of the book "Mastering OpenCV with Practical Computer Vision Projects"
*   Copyright Packt Publishing 2012.
*   http://www.packtpub.com/cool-projects-with-opencv/book
******************************************************************************

        #This is a fork, added benchamrking of FPS and to save faces and re-recognize. Vita Vidaurre 2014

Note: You need OpenCV v2.4.1 or later (from June 2012), otherwise the FaceRecognizer will not compile or run.
And you need atleast 3 Face & Eye detection XML files from OpenCV.

install opencv 2.x.x in linux :
Download .zip at opencv.org

extract and cd to the directory

                mkdir build

                cd build

                sudo apt-get install build-essential libgtk2.0-dev libjpeg-dev libtiff4-dev libjasper-dev libopenexr-dev cmake python-dev python-numpy python-tk libtbb-dev libeigen2-dev yasm libfaac-dev libopencore-amrnb-dev libopencore-amrwb-dev libtheora-dev libvorbis-dev libxvidcore-dev libx264-dev libqt4-dev libqt4-opengl-dev sphinx-common texlive-latex-extra libv4l-dev libdc1394-22-dev libavcodec-dev libavformat-dev libswscale-dev
hours later...

                cmake -D WITH_TBB=ON -D BUILD_NEW_PYTHON_SUPPORT=ON -D WITH_V4L=ON -D INSTALL_C_EXAMPLES=ON -D INSTALL_PYTHON_EXAMPLES=ON -D BUILD_EXAMPLES=ON -D WITH_QT=ON -D WITH_OPENGL=ON ..
hours later...

                make
hours later...

                sudo make install
Now you have OpenCV 2.x.x installed in your computer with C, C++, Python, TBB, OpenGL, Video, and Qt support.


----------------------------------------------------------
Building the project using CMake from the command-line:
----------------------------------------------------------
Linux:
        ./Build
     


----------------------------------------------------------
Running the project:
----------------------------------------------------------
Just execute           ./DifferentFacesDetection

If it says it can't find a Haar or LBP cascade XML file, copy those XML files from the OpenCV "data" folder to your current folder.

