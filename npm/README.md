# NPM

## Build instructions
### Build image
docker build -t ajegu/npm .

### Delete image
docker image rm ajegu/npm -f

## Container usage instructions

### Show version
#### NPM
docker run --rm -it -w /data ajegu/npm --version 

### Init NPM project
docker run --rm -it -v ${pwd}:/data ajegu/npm init
