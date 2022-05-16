---
layout: post
title: "Increase Max File Size Upload for Wordpress in Docker"
date: 2022-02-04 12:00:00 +0800
categories: [Website, Tutorial, Server]
---

# Increase Max File Size Upload for Wordpress in Docker

Open terminal

List down active containers

```bash
docker ps
```

Run bash inside the wordpress container
```bash
docker exec -it <container_name>
```

List all files, including hidden
```bash
ls -alh
```

Show contents of .htaccess file
```bash
cat .htaccess
```

Insert php values on empty line with sed
```bash
sed -i '/^# END WordPress.*/i php_value upload_max_filesize 256M\nphp_value post_max_size 256M' .htaccess 
```
