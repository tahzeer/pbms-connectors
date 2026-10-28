# Staff API image a cluster runs. Adds registry-adapters on the PBMS base.
# REGISTRY_ADAPTERS_CONNECTOR selects db or dci.
# PBMS_VERSION matches helm/openg2p-pbms/Chart.yaml.
ARG PBMS_IMAGE=openg2p/openg2p-pbms-staff-api-base
ARG PBMS_VERSION=develop
FROM ${PBMS_IMAGE}:${PBMS_VERSION}

COPY extensions/registry-adapters /src/registry-adapters
RUN pip install --no-cache-dir /src/registry-adapters
