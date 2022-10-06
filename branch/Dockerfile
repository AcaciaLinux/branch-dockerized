FROM debian AS branchimage
COPY branch /branch/
RUN apt install python3 make
RUN cd branch && make
RUN mkdir /branchworkdirectory/
COPY entry.sh /entry.sh
RUN mkdir /etc/branch
RUN chmod +x entry.sh
CMD /entry.sh
EXPOSE 27015/tcp
