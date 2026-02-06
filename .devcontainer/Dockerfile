# Start from the official VectorBT image
FROM polakowo/vectorbt:latest-full

# Switch to root to install additional packages if needed
USER root

# Install any extra system dependencies here
# RUN apt-get update && apt-get install -y git

# Switch back to the default user (jovyan is the default in Jupyter images)
USER jovyan

# Install additional Python packages for development (requirements.txt)
COPY requirements.txt /tmp/requirements.txt
RUN pip install --no-cache-dir -r /tmp/requirements.txt
