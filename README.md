sudo docker run -p 9000:9000 \
 -e "MINIO_ACCESS_KEY=minio" \
 -e "MINIO_SECRET_KEY=minio123" \
 -v /mnt/data:/data \
 -v /mnt/config:/root/.minio \
 minio/minio:RELEASE.2018-07-13T00-09-07Z server /data
