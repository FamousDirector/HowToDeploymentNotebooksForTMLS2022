FROM nvcr.io/nvidia/tritonserver:22.09-py3
# release notes: https://docs.nvidia.com/deeplearning/triton-inference-server/release-notes/rel_22.09.html#rel_22-09

# install python depencies
RUN pip install --upgrade pip setuptools
COPY requirements.txt .
RUN python3 -m pip install -r requirements.txt

CMD ["tritonserver", "--help"]