
NAME=brackets_server_dev

build:
	docker build -t $(NAME) .

run:
	docker run --rm -p 6800:6800 --name $(NAME) -v ${PWD}:/root/Projects $(NAME)

stop:
	docker stop `docker ps -qa -f name=$(NAME)`
rm:
	docker rm `docker ps -qa -f name=$(NAME)`

rmi:
	docker rmi $(NAME)
