# kinect-v2-ubuntu16.04
errors with install
#On Ubuntu 16, I had the same issue. Here is how it got fixed. Hope it helps
#Step 1:
#Install libjpeg-turbo8-dev
#Step 2:
#The libturbojpeg.so file was missing so I had to create a sym-link.
#I ran sudo ln -s /usr/lib/x86_64-linux-gnu/libturbojpeg.so.0 /usr/lib/x86_64-linux-gnu/libturbojpeg.so
#Step 3:
#Deleted the build directory and ran cmake again.
