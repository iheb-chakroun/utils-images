FROM quay.io/buildah/stable:v1.28.0

RUN dnf -y update && dnf -y install openssh-server passwd && dnf clean all

RUN ssh-keygen -A

CMD ["/usr/sbin/sshd", "-D"]

