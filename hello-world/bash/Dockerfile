FROM ubuntu:22.04
RUN apt-get update && apt-get install bash -y
COPY script.sh /script.sh
RUN chmod +x /script.sh
CMD ["/bin/bash", "/script.sh"]
