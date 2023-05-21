# JAX

## 설치

### CPU-only
```bash
pip install "jax[cpu]"
```

### GPU(CUDA)
```bash
pip install "jax[cuda]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
```

### TPU(Google Cloud)
```bash
pip install "jax[tpu]" -f https://storage.googleapis.com/jax-releases/libtpu_releases.html
```

## JAX Quickstart
JAX는 CPU, GPU, TPU 모두에서 동작하는 Numpy로, machine learning 연구에서 고성능을 기대할 수 있다.  

### XLA
XLA는 Accelerated Linear Algebra의 약자로, CPU, GPU 및 맞춤형 액셀러레이터(예: Google의 TPU)와 같은 기기에 대해 JIT 컴파일 기법을 사용하여 런타임에 사용자가 생성한 TensorFlow 그래프를 분석하고 실제 런타임 차원과 유형에 맞게 최적화하며, 여러 연산을 함께 합성하고 이에 대한 효율적인 네이티브 기계어 코드를 내보낸다.  
JAX는 XLA를 사용하여 JIT 컴파일을 지원하며, 이는 GPU나 TPU와 같은 가속기에서 컴파일을 통해 더 빠른 연산을 수행할 수 있게 해준다.

