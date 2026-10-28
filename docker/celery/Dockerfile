# Celery image a cluster runs, for both the worker and the beat deployments.
# CELERY_APP on the pod selects which process starts.
# PBMS_VERSION matches helm/openg2p-pbms/Chart.yaml.
ARG PBMS_IMAGE=openg2p/openg2p-pbms-celery-base
ARG PBMS_VERSION=develop
FROM ${PBMS_IMAGE}:${PBMS_VERSION}

COPY extensions/registry-adapters /src/registry-adapters
RUN pip install --no-cache-dir /src/registry-adapters
