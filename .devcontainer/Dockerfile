FROM continuumio/miniconda3

RUN conda install -c conda-forge jupyterlab
RUN conda install -c conda-forge nodejs
RUN conda install -c conda-forge xeus-python=0.7.1 notebook=6 jupyterlab=2 ptvsd
RUN jupyter labextension install @jupyterlab/debugger

EXPOSE 8888

ENTRYPOINT ["jupyter", "lab","--ip=0.0.0.0","--allow-root","--NotebookApp.password='sha1:ec4ffbe05d95:bc33a87017a077d24dc303f7c008381cb172193f'"]