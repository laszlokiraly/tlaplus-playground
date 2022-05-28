FROM debian:stretch

RUN apt-get update && apt-get install --assume-yes --no-install-recommends \
	default-jre \
	wget \
	unzip \
	git \
	zsh

RUN apt-get install -y --no-install-recommends texlive-latex-recommended

RUN wget -q -O tla.zip https://github.com/tlaplus/tlaplus/releases/download/v1.8.0/TLAToolbox-1.8.0-linux.gtk.x86_64.zip && unzip tla.zip && rm tla.zip

ENTRYPOINT ./toolbox/toolbox
