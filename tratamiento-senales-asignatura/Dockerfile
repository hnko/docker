FROM jupyter/minimal-notebook:82d1d0bf0867

COPY requirements.txt .

RUN conda update -n base conda -y 
RUN conda install pip -y 
RUN pip install -r requirements.txt

EXPOSE 8888