GPU-Accelerated Bayer Pattern Demosaicing
=========================================

Max Smolens  
UNC-Chapel Hill  
Research for Office of the Future Group; Assignment for COMP 238: Advanced Image Generation  
Fall 2004

## Components
[bayer_cg](bayer_cg): Bayer renderer using fragment programs.  
[bayer_viewer_ogl](bayer_viewer_ogl): Bayer renderer using OpenGL texturing.  
[utils](utils): Utilities for generating test data.  

## Overview
Digital cameras commonly use only a single CCD to capture an image. To support color imaging with a single CCD, a color filter array (CFA) only allows particular wavelengths of light to pass through at each pixel. These programs resconstruct ("demosaic") images created by a Bayer pattern CFA back to an RGB image.

### Bayer CFA pattern:
![Bayer CFA pattern](/bayer_cg/doc/bayer_pattern.png?raw=true)

### Bayer pattern image:
![Bayer pattern image](/bayer_cg/doc/out_bayer.png?raw=true)
![Detail view](/bayer_cg/doc/out_bayer_zoom.png?raw=true)

### Reconstructed image:
![Reconstructed image](/bayer_cg/doc/out_color.png?raw=true)
![Detail view](/bayer_cg/doc/out_color_zoom.png?raw=true)

## More information

See [`bayer_viewer_ogl/doc/bayer_renderer.pdf`](bayer_viewer_ogl/doc/bayer_renderer.pdf) for an overview of the reconstruction technique.

See [`bayer_cg/doc/index.html`](bayer_cg/doc/index.html) for implementation details and performance analysis.

