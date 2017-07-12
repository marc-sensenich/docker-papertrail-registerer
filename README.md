# docker-papertrail-registerer

This image allows for the registration of a system through the Papertrail HTTP API. Although it was designed with this in mind, it should run most of their API commands using the environment variables PAPERTRAIL_API_PATH, PAPERTRAIL_API_METHOD, and PAPERTRAIL_API_DATA; YMMV.

## Usage

```sh

docker run --rm -e PAPERTRAIL_API_TOKEN='123456' -e PAPERTRAIL_API_DATA='system[name]=ProdWebServer&system[hostname]=wwwprod&destination_id=1234' marcsensenich/papertrail-registerer

```