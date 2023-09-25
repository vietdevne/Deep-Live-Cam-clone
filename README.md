![demo-gif](demo.gif)

## Như cái con cặc


## Tải mấy cl này về trước nè Tố ơi
#### 1.Setup your con cặc
-   [conda](https://repo.anaconda.com/archive/Anaconda3-2024.06-1-Windows-x86_64.exe)
-   [git](https://github.com/git-for-windows/git/releases/download/v2.45.2.windows.1/Git-2.45.2-64-bit.exe)
-   ffmpeg thì cài như này: mở powershell với quyền admintrator chạy: "iex (irm ffmpeg.tc.ht)" xong đợi tí rồi nhấn "3" cho nó chạy tiếp

-   [visual studio 2022 runtimes (windows)](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=community&rel=17)

#### 2. Download Models

 1. [GFPGANv1.4](https://huggingface.co/hacksider/deep-live-cam/resolve/main/GFPGANv1.4.pth)
 2. [inswapper_128.onnx](https://huggingface.co/hacksider/deep-live-cam/resolve/main/inswapper_128.onnx)

#### 4. Install dependency

1.  Install  [CUDA Toolkit 11.8](https://developer.download.nvidia.com/compute/cuda/11.8.0/local_installers/cuda_11.8.0_522.06_windows.exe)
    
2.  Install dependencies:
    

```
pip uninstall onnxruntime onnxruntime-gpu
pip install onnxruntime-gpu==1.15.1

```

3.  Usage in case the provider is available:

```
python run.py --execution-provider cuda

```