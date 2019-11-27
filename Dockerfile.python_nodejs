ARG node_image=fczuardi/node_download:11.10.1
ARG python_image=python:3.5-buster

# image containing downloaded binaries
FROM ${node_image} as download

# main image
FROM ${python_image}

# copy node binaries and add it to the PATH
WORKDIR "/opt/node"
COPY --from=download /opt/node .
ENV PATH=$PATH:/opt/node/bin
