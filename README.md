## Docker Compose를 다루는 방법

[DOCKER-COMPOSE](https://docs.docker.com/compose/compose-file/)

- restart 옵션은 4가지가 있다.
	- no: container를 재시작 시키지 않는다. (default)
	- on-failure[:max-retries]: container가 정상적으로 종료되지 않은 경우(exit code가 0이 아님)에만 재시작 시킨다. max-retries도 함께 주면 재시작 최대 시도횟수를 지정할 수 있고, 테스트 서버 등과 같은 리모트에 설정하면 좋을 것 같다.
	- always: container를 항상 재시작시킨다. exit code 상관 없이 항상 재시작 된다.
	- unless-stopped: container를 stop시키기 전 까지 항상 재시작 시킨다.

- shm_size : docker 내부 호스트 메모리 용량 지정
