# hadolint global ignore=DL3008,DL3015
FROM docker.gitea.com/runner-images:ubuntu-24.04@sha256:b41ad2910fd25e86e52570cdf456075067f2e4f2c575d46f7a16c107fd354368

RUN \
	apt-get update -q && \
	apt-get install -q -y buildah podman containers-storage iptables qemu-user-static skopeo && \
	mkdir -p /root/.docker && \
	apt-get clean && \
	rm -rf /var/lib/apt/lists/*
