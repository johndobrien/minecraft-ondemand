FROM itzg/minecraft-server:java17


WORKDIR /data_temp
COPY ./mods ./mods

# Expose the default Minecraft port
EXPOSE 25565

WORKDIR /

COPY copy_mods_and_start.sh copy_mods_and_start.sh
RUN chmod +x copy_mods_and_start.sh
ENTRYPOINT ["/copy_mods_and_start.sh"]