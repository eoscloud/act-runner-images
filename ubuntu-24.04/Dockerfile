# hadolint global ignore=DL3008,DL3015
FROM docker.gitea.com/runner-images:ubuntu-24.04@sha256:40aa20a462b701a97b18a59e356549004afc9259d5bd3314c19194db14a80237

RUN \
	apt-get update -q && \
	apt-get install -q -y buildah podman containers-storage iptables qemu-user-static && \
	mkdir -p /root/.docker && \
	apt-get clean && \
	rm -rf /var/lib/apt/lists/*
