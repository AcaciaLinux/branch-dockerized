FROM debian
COPY branch/branchmaster /branch/
RUN apt update -y && apt install python3 make -y
RUN cd branch && make
COPY entry.sh /entry.sh
RUN chmod +x entry.sh
CMD /entry.sh
EXPOSE 27015/tcp
