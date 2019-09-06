# Nucypher Error Report 1

## System Information

- MacOS Mojave 10.14.6 (18G95)
- MacBook Pro (13-inch, 2016, Four Thunderbolt 3 Ports)
- 2.9 GHz Intel Core i5
- 8 GB 2133 MHz LPDDR3

- Python Version: 3.7.2
- Branch: master

## Error 1 found in Nuypher/dev/docker

- URL: https://github.com/nucypher/nucypher/tree/master/dev/docker
- Video: https://youtu.be/ZkVWjrgv4Ho

Trying to test the Nucypher Network in federated mode locally following the demo here: https://www.youtube.com/watch?v=om0tew-Z4gE

After `cd`-ing into `nucypher/dev/docker` and running `docker-compose up --build`

1. I then run `docker-compose run nucypher-dev bash` to spin your docker container and have the nucypher cli installed.
2. I create an ursula and an alice (`nucypher ursula run --dev --federated-only` and `nucypher alice run --dev --federated-only`
   ). I do this in different local bash but ensure to access the same docker container (to make sure that Alice and Ursula are running on the same localhost. I do this by doing `docker exec -it <containerid> bash`)
3. When I try to make an http request to Alice this fails.
