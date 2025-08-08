QingLong Dashbord
docker run -dit \
  -v $/mydocker/qinglong/config:/ql/config \
  -v $/mydocker/qinglong/log:/ql/log \
  -v $/mydocker/qinglong/db:/ql/db \
  -v $/mydocker/qinglong/repo:/ql/repo \
  -v $/mydocker/qinglong/raw:/ql/raw \
  -v $/mydocker/qinglong/scripts:/ql/scripts \
  -p 5700:5700 \
  --name qinglong \
  --hostname qinglong \
  --restart unless-stopped \
  whyour/qinglong:2.10.13
