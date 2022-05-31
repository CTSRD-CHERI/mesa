CHERI Purecap Mesa (without window system support)

Build for Morello (Panfrost)

.. code-block:: sh

 $ mkdir build
 $ cd build
 $ meson .. -Dcpp_rtti=false -Dllvm=disabled -Dgallium-xvmc=enabled -Ddri-drivers= -Dgallium-drivers=panfrost,swrast \
   -Dvulkan-drivers= -Dplatforms= -Dgallium-xa=disabled -Dgallium-vdpau=disabled -Dgallium-va=disabled -Dgles1=enabled \
   -Dgles2=enabled -Dglx=disabled -Dosmesa=false -Dtools= -Ddri-drivers= -Dglvnd=false -Dgbm=enabled -Degl=enabled \
   -Dgallium-nine=false -Dgallium-xa=disabled -Dgallium-va=disabled -Dgallium-omx=disabled -Dgallium-xvmc=disabled \
   -Dgallium-vdpau=disabled
 $ ninja
 $ sudo ninja install
