ARG PYTHON_VERSION=3.10
ARG TRTLLM_VERSION="latest"

FROM tensorrt_llm/release:v${TRTLLM_VERSION}-py${PYTHON_VERSION}

COPY . /opt/optimum-nvidia

# Install dependencies
RUN python -m pip install /opt/optimum-nvidia

# Let's put our users in the examples folder
WORKDIR /opt/optimum-nvidia/examples
