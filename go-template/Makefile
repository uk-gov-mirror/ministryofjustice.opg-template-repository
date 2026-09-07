build:
	docker compose build --no-cache {{APP_NAME}}

build-dev:
	docker compose -f docker-compose.yml -f docker/docker-compose.dev.yml build --no-cache --parallel {{APP_NAME}}

clean:
	docker compose -f docker-compose.yml -f docker/docker-compose.dev.yml down --remove-orphans

dev-up: clean build-dev
	docker compose -f docker-compose.yml -f docker/docker-compose.dev.yml up {{APP_NAME}} watch-assets

up: clean build
	docker compose up -d {{APP_NAME}}

down:
	docker compose down --remove-orphans