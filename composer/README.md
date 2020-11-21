# PHP Composer image

## Build instructions

### Build image
docker build -t ajegu/composer .

### Delete image
docker image rm ajegu/composer -f

## Container usage instructions

### Show version
docker run --rm ajegu/composer -v

### Init project
docker run --rm -v ${pwd}:/data ajegu/composer init --name `PROJECT_NAME`

### Laravel install 
docker run --rm -v ${pwd}:/data ajegu/composer create-project --prefer-dist laravel/laravel `PROJECT_NAME`