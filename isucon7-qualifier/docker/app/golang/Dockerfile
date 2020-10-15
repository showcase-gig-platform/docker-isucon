FROM golang:1.15.3-alpine

ARG GIT_URL=https://github.com/showcase-gig-platform/isucon-study-qualify.git

RUN git clone $GIT_URL /home/isucon/isubata
WORKDIR /home/isucon/isubata/webapp/go
RUN make

EXPOSE 5000

ENTRYPOINT ["/home/isucon/isubata/webapp/go/isubata"]
