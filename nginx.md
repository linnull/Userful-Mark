###开启 gzip 压缩

```
gzip on;
gzip_buffers 32 4k;
gzip_comp_level 6;
gzip_min_length 100;
gzip_types *;
```
