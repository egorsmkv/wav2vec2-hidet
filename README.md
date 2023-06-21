# wav2vec2-hidet

> NOTE: this is a work-in-progress thing, do not use it anywhere except dev machine

Installation:

```
git clone https://github.com/egorsmkv/wav2vec2-hidet
cd wav2vec2-hidet

conda create -n w2v2-hidet python=3.10
conda activate w2v2-hidet

pip install 'torch>2.0.0' torchaudio
pip install evaluate soundfile transformers jiwer
pip install https://github.com/kpu/kenlm/archive/master.zip pyctcdecode

conda install -c conda-forge nvtx
pip install hidet

conda install -c conda-forge cudatoolkit-dev
```

Running:

```
python export_gpu_version.py

python recognize_gpu_with_lm_and_hidet.py
```

Links:

- https://pytorch.org/blog/introducing-hidet/
- https://docs.hidet.org/stable/gallery/tutorials/optimize-pytorch-model.html
