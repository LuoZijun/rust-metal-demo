rust metal demo
===================

.. contents::


Metal Tools
-------------

:系统路径: /Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/usr/bin
:参考文档: `Building a Library with Metal's Command-Line Tools <https://developer.apple.com/documentation/metal/tools_profiling_and_debugging/building_a_library_with_metal_s_command_line_tools>`_

.. code:: bash
    
    xcrun -sdk macosx metal src/shaders.metal -o src/shaders.air
    xcrun -sdk macosx metallib src/shaders.air -o src/shaders.metallib

    # Or

    xcrun -sdk macosx metal src/shaders.metal -o src/shaders.air
    xcrun -sdk macosx metal-ar rcs src/shaders.metalar src/shaders.air
    xcrun -sdk macosx metallib src/shaders.metalar -o src/shaders.metallib



Build
-------------

.. code:: bash
    
    cargo run 
    cargo run --example ui

