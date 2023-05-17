# image-optimizer

## Quick start

Run the command `docker-compose up`.

## URL structure

`http://localhost/{s3_backet_domain}/{w}/{h}/{[resize|crop]}/{s3_backet_image_uri}`.

**Examples:**

The original image URL: [https://via.placeholder.com/600/24f355](https://via.placeholder.com/600/24f355).

- Resizing: [http://localhost/via.placeholder.com/200/200/resize/600/24f355](http://localhost/via.placeholder.com/200/200/resize/600/24f355).
- Croping: [http://localhost/via.placeholder.com/200/200/crop/600/24f355](http://localhost/via.placeholder.com/200/200/crop/600/24f355).

## Customization

1. Replace the S3 backet URL (`via.placeholder.com`) in `nginx/default.conf` with your own.
1. Add your own `$resize_variant` in `nginx/default.conf`.