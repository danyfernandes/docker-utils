# Use the official Airflow image as the base
FROM apache/airflow:2.10.2
LABEL Maintainer="daniel.fernandes@adopt.fr"

# Install the required Python packages listed in requirements.txt
COPY requirements.txt .

USER root
RUN apt-get update && \
    apt-get install -y libpq-dev gcc

USER airflow
RUN pip install --no-cache-dir --extra-index-url ${PIP_EXTRA_URL} -r requirements.txt



# Set the entrypoint (this is necessary for Airflow to start correctly)
ENTRYPOINT ["/entrypoint"]

# Default command
CMD ["webserver"]
