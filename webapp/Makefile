SHELL=/bin/bash

all: isucon

isucon:
	docker compose -f docker-compose/go.yaml build
	docker compose -f docker-compose/go.yaml up -d

down:
	docker compose -f docker-compose/go.yaml down

clean: down
	docker system prune -f