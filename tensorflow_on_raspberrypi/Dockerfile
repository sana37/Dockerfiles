FROM resin/rpi-raspbian

RUN apt-get update && apt-get install -y \
        python3 \
        python3-dev \
		python3-pip \
		python3-numpy \
		build-essential

RUN  apt-get clean && \
        rm -rf /var/lib/apt/lists/*

RUN python3 -m pip install numpy -U

WORKDIR "/root"

ADD tensorflow-1.1.0-cp34-cp34m-linux_armv7l.whl .

RUN python3 -m pip install tensorflow-1.1.0-cp34-cp34m-linux_armv7l.whl

RUN rm tensorflow-1.1.0-cp34-cp34m-linux_armv7l.whl

CMD ["/bin/bash"]
