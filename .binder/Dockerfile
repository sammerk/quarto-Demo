FROM rocker/binder:4.5.1
LABEL maintainer='Samuel_Merk'
COPY --chown=${NB_USER} . ${HOME}
USER ${NB_USER}



RUN wget https://github.com/sammerk/quarto-Demo/raw/master/DESCRIPTION && R -e "options(repos = list(CRAN = 'http://mran.revolutionanalytics.com/snapshot/2025-10-04/')); devtools::install_deps()"

RUN rm DESCRIPTION.1; exit 0
