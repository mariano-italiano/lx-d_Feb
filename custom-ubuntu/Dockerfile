FROM ubuntu:noble-20250127

RUN groupadd -g 2500 appgroup && \
    useradd -m -u 2500 -g appgroup appuser

USER appuser

WORKDIR /home/appuser

#CMD ["sh", "-c", "echo 'Pracuje w kontenerze jako uzytkownik' $(whoami) , UID=$(id -u), GID=$(id -g)" ]

ENTRYPOINT ["/bin/bash"]
CMD ["-c", "tail -f /dev/null"] 
