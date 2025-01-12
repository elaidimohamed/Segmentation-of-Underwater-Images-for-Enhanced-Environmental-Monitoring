# 🎯 Underwater Depth Estimation App

An advanced application for estimating and visualizing depth in underwater images and videos using state-of-the-art AI models. Built with Gradio, PyTorch, and the Depth Anything model family, optimized for underwater environments.

![output_depth_video_1-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/6991658d-b7b6-40a8-a104-8e1eaec3c817) 


## 🌟 Features

- **Multi-Format Support**: Process both underwater images and videos
- **Interactive Interface**: User-friendly Gradio web interface
- **Underwater-Specific Enhancements**: Contrast correction for murky water and handling of unique lighting conditions
- **Multiple Visualization Options**: Various colormaps optimized for underwater depth visualization
- **Analysis Tools**: Depth distribution histogram for detailed analysis
- **Model Options**: Choice between different model sizes tailored for underwater use
- **Real-Time Processing**: Live preview of results

  ![SharedScreenshot](https://github.com/user-attachments/assets/401a1865-0348-4686-9835-8fcd7308e1ac)
  ![SharedScreenshot_](https://github.com/user-attachments/assets/56599d00-91bc-4adb-b8c5-9c79e10c1030)



## 🔧 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/underwater-depth-estimation-app.git
cd underwater-depth-estimation-app
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

## 📦 Requirements

```plaintext
torch
torchvision
transformers
opencv-python
pillow
gradio
tqdm
matplotlib
numpy
```  

## 🚀 Usage

1. Start the Gradio app:
```bash
python app.py
```

2. Open your browser and navigate to the provided URL (typically `http://localhost:7860`)

3. Choose between image or video processing:
   - Upload an underwater image or video
   - Select your preferred colormap and model
   - Enable/disable histogram and underwater contrast enhancement
   - Click "Process" to generate the depth visualization


## 🎨 Available Colormaps

- INFERNO (recommended for underwater)
- JET
- VIRIDIS
- PLASMA
- MAGMA
- HOT

## 🤖 Available Models

- **Depth Anything Small**: Faster processing, smaller memory footprint
- **Depth Anything Base**: Higher accuracy, larger model size

## 📊 Output Examples

The app generates:
- Depth maps with underwater-specific color visualization
- Depth distribution histograms (for images)
- Processed videos with underwater depth visualization

## 🔧 Troubleshooting

### Common Issues and Solutions

1. **Murky or Low-Visibility Water**:
   - Enable contrast enhancement
   - Use the "Base" model for better depth estimation

2. **CUDA Out of Memory**:
   - Reduce input image/video resolution
   - Use the "Small" model instead of "Base"
   - Free up GPU memory

3. **Slow Processing**:
   - Ensure CUDA is available
   - Check GPU usage
   - Consider reducing input resolution

4. **Video Codec Issues**:
   - Install required codecs
   - Try converting video to MP4 format
   - Check OpenCV installation


