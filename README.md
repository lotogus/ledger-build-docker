# ledger-build-docker
dockerfile for building a Ledger App. It's an builder alternative to https://github.com/fix/ledger-vagrant , I couldn't make work so I've tried with Docker!

## run

docker build . ##--> this will return an hash on the last line, eg: Successfully built c8638d26b08e
docker run -it c8638d26b08e

then you can go to /root, checkout your git project and compile it!

## compile example

	cd /root
	git clone https://github.com/lotogus/ledger-app-casinocoin
	cd ledger-app-casinocoin
	make clean
	make
