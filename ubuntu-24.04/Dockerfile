# hadolint global ignore=DL3008,DL3015
FROM docker.gitea.com/runner-images:ubuntu-24.04@sha256:612a5865c64d61d68d914c2058969ed06cf7701d7d21c18b3b9917a6af90528f

RUN \
	apt-get update -q && \
	apt-get install -q -y buildah podman containers-storage iptables qemu-user-static && \
	mkdir -p /root/.docker && \
	apt-get clean && \
	rm -rf /var/lib/apt/lists/*
