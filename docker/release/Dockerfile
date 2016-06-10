FROM sc250024/todobackend-base:latest
MAINTAINER Scott Crooks <scott.crooks@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
	pip install --no-index -f /wheelhouse todobackend && \
	rm -rf /wheelhouse