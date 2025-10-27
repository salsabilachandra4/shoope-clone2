# Gunakan image nginx resmi
FROM nginx:alpine

# Hapus default nginx HTML
RUN rm -rf /usr/share/nginx/html/*

# Salin file project ke folder nginx
COPY . /usr/share/nginx/html

# Ekspos port 80 (bukan 84)
EXPOSE 80

# Jalankan nginx di foreground
CMD ["nginx", "-g", "daemon off;"]
