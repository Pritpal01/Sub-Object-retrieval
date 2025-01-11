# requirements:

pip install ultralytics
pip install torch torchvision torchaudio
pip install opencv-python
pip install numpy
pip install matplotlib
pip install tensorflow


# check for installation using:
import sys
def check_installations():
    packages = ['ultralytics','torch','torchvision','torchaudio','opencv-python','numpy','matplotlib']
    for package in packages:
        try:
            __import__(package)
            print(f"{package} is installed.")
        except ImportError:
            print(f"{package} is NOT installed.")
    python_version = sys.version
    print(f"\nPython version: {python_version}")
check_installations()
