FROM debian:stable-slim

RUN apt-get update && apt-get install --assume-yes --no-install-recommends \
	default-jre \
	wget \
	unzip \
	git

RUN apt-get install -y --no-install-recommends texlive-latex-recommended

RUN apt-get install -y zsh
RUN wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | zsh || true

RUN wget -q -O tla.zip https://github.com/tlaplus/tlaplus/releases/download/v1.8.0/TLAToolbox-1.8.0-linux.gtk.x86_64.zip && unzip tla.zip && rm tla.zip

ENTRYPOINT ./toolbox/toolbox
