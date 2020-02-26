FROM nfcore/base:1.7
LABEL authors="Sabrina Krakau" \
      description="Docker image image for use in nf-core/sarek"

COPY environment.yml /
RUN conda env create -f /environment.yml && conda clean -a
ENV PATH /opt/conda/envs/sarek-trimgalore-2.5.2/bin:$PATH
