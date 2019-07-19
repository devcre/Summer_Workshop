# Summer_Workshop
2019 하계 워크샵 (thread를 이용한 proxy 서버 구축)

주제 : Thread를 이용한 proxy 서버 구축

- 캐싱 프록시 서버

- 에코 프록시 서버

작성자 : 조경찬

- 참고자료
http://amritapnitc.blogspot.com/2015/07/simple-proxy-server-in-c-using-multi.html

How to run the programs?

1. compile main server, proxy server and client codes.
    gcc mainserver.c -o mainserver -lpthread

    gcc proxy.c -o proxy -lpthread

    gcc -o client client.c
    
2. run main server and proxy server.
    ./mainserver

    ./proxy 127.0.0.1 5010 5000

3. run client and type message to send
    ./client

    Enter proxy address:127.0.0.1

    Enter a prot:5000

    Type here: "FREE TO TYPE"

*NOTE*
1. -lpthread is a command used to compile the code if multi-threading is used.

2. client.c file accepts 5000 as a port address for proxy server. It is hard coded in the file. You can either comment that line or write other valid port address if you need it that way
