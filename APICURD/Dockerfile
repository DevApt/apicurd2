FROM golang

RUN mkdir /build
WORKDIR /build

RUN export GO111MODULE=on
RUN go get github.com/DevApt/apicurd2
RUN cd /build && git clone https://github.com/DevApt/apicurd2.git

RUN cd /build/APICURD/main && go build

EXPOSE 8080

ENTRYPOINT [ "/build/APICURD/main/main"]