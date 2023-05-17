# image-optimizer

## Quick start

1. Replace the S3 URL (`s3.exapmle.com`) in `nginx/default.conf` with your own.
1. Run the command `docker-compose up`.

## URL structure

`http://localhost/{s3_backet_domain}/{w}/{h}/{[resize|crop]}/{s3_backet_image_uri}`.

**Example:**

`https://s3.example.com/680/380/crop/image_1fe47c2a1f_e72eb738f7.png`.