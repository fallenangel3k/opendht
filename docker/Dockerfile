FROM aberaud/opendht-deps
MAINTAINER Adrien Béraud <adrien.beraud@savoirfairelinux.com>
RUN git clone https://github.com/savoirfairelinux/opendht.git \
	&& cd opendht && mkdir build && cd build \
	&& cmake .. -DCMAKE_INSTALL_PREFIX=/usr && make -j8 && make install \
	&& cd ../.. && rm -rf opendht