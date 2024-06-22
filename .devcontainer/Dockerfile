FROM huggingface/transformers-pytorch-gpu
LABEL maintainer="Hugging Face"

RUN python3 -m pip install -U ipykernel ipywidgets packaging ninja
RUN python3 -m pip install -U flash-attn --no-build-isolation
RUN pip install -U qdrant-client
RUN pip uninstall -y transformers
RUN pip install git+https://github.com/huggingface/transformers