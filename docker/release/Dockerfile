FROM robertrepka/todobackend-base:latest
MAINTAINER Robert Repka <robo@repka.org>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse
