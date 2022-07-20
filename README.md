# panorama2cubemap

##build

    mkdir build && cd build
    cmake ..
    make -j12


##interface

    bool pano2cube(std::string inpath, std::vector<std::string>& outpaths, int width = -1);

there is test code in the file, read auto_stop_spherical_pano.jpg and generate 6 faces.

6 face order: +X, -X, +Y, -Y, +Z, -Z

    +X right
    -X left
    +Y top 
    -Y bottom
    +Z front
    -Z back


test image:

<img src="src/auto_stop_spherical_pano.jpg"/>

