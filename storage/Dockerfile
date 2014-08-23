FROM busybox
VOLUME /data
CMD /bin/sh

# Attach the storage to an instance.  The container is op_data.  op_data 
# is the container for this image.  Generate that container via:
# docker run -v /data:/data -name mydata dsklopp/mydata
# Then attach to docker via
# docker run -t -i -volumes-from op_data dsklopp/wlan_mib_ap_scanner
