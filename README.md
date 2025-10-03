## CUSTOM DIRECTX12 EXCEPTION / DIAGNOSTIC TOOL

> HOW TO USE
- clone the repo `git clone https://github.com/sho34/directx-exceptions.git` into your directx12/directx11 project folder.

- Include structure.
  ```
    #include <wrl.h>
    #include <d3d12.h>
    #include <dxgi1_6.h>
    ....

    // then include the files.
    #include "dx_exceptions/Directx12Ex.h"
    #include "dx_exceptions/exception-macros.h"
  ```
- To use just call `THROW_GRAPHICS_INFO(__in__ hr);` e.g. `THROW_GRAPHICS_INFO(D3D12GetDebugInterface(IID_PPV_ARGS(&debug_interface)));`
