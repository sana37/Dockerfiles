FROM tensorflow_on_raspberrypi

RUN apt-get update && apt-get install -y \
        portaudio19-dev \
		python3-scipy \
		python3-serial

RUN  apt-get clean && \
        rm -rf /var/lib/apt/lists/*

RUN python3 -m pip install pyaudio

WORKDIR "/root"

CMD ["/bin/bash"]
