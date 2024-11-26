FROM alpine:latest
# Install bash using apk
RUN apk update && apk add bash
# Copy your script into the container
COPY script.sh /script.sh
# Make the script executable
RUN chmod +x /script.sh
# Run the script using bash
CMD ["/bin/bash", "/script.sh"]
