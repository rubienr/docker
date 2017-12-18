#
# Build
# docker build -t="latex/devel_env".
# docker build -t="https://github.com/rubienr/docker/latex/"
#
# Run
# docker run -it --rm latex/devel_env 
#

FROM ubuntu:17.10

RUN useradd -m -g users user;   \
                                \
    apt-get update &&           \
    apt-get upgrade -y &&       \
    apt-get install -y          \
            texlive-latex-base  \
            texlive-latex-extra \
            texlive-lang-german \
            git

ENV HOME /home/user
WORKDIR  /home/user
USER     user:users

CMD      ["bash"]
