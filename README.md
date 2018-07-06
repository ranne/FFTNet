# FFTNet

A PyTorch implementation of the [FFTNet: a Real-Time Speaker-Dependent Neural Vocoder](http://gfx.cs.princeton.edu/pubs/Jin_2018_FAR/)

### Audio Samples

* **[Audio Samples](https:///syang1993.github.io/fftnet/)** from models trained using this repo with default hyper-params.

## Quick Start:
1. Install requirements:
  ```
  pip install -r requirements.txt
  ```
2. Download dataset:
  ```
  wget http://festvox.org/cmu_arctic/cmu_arctic/packed/cmu_us_slt_arctic-0.95-release.tar.bz2
  tar xf cmu_us_slt_arctic-0.95-release.tar.bz2
  ```
3. Extract features:
  ```
  python preprocess.py
  ```
4. Training with default hyperparams:
  ```
  python train.py
  ```

## TODO:
- [ ] Fast generation. (Without fast generation, it generates about 230 samples per second with a free TITAN Xp.)
- [ ] Post-synthesis denoising.

## Notes:
  * This is not offical implementation, some details are different from the paper.
  * Now the generated speech from this repo is not so good as wavenet vocoder.
  * Work in progress.
