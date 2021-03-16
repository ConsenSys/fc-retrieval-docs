# PoC1 Expected Test Output
This file contains the expected output when running the following commands:
```
git clone https://github.com/ConsenSys/fc-retrieval-common.git
cd fc-retrieval-common/scripts
bash clonebuildtest.sh 163-poc1-release
```

# Expected Output

```
scripts % bash clonebuildtest.sh 163-poc1-release 
Clone, Build, and Test for branch: 163-poc1-release
Cloning repo: client
Cloning into 'fc-retrieval-client'...
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 802 (delta 0), reused 1 (delta 0), pack-reused 798
Receiving objects: 100% (802/802), 193.51 KiB | 56.00 KiB/s, done.
Resolving deltas: 100% (445/445), done.
Branch '163-poc1-release' set up to track remote branch '163-poc1-release' from 'origin'.
Switched to a new branch '163-poc1-release'
Cloning repo: common
Cloning into 'fc-retrieval-common'...
remote: Enumerating objects: 297, done.
remote: Counting objects: 100% (297/297), done.
remote: Compressing objects: 100% (189/189), done.
remote: Total 297 (delta 154), reused 223 (delta 99), pack-reused 0
Receiving objects: 100% (297/297), 115.54 KiB | 1.10 MiB/s, done.
Resolving deltas: 100% (154/154), done.
Branch '163-poc1-release' set up to track remote branch '163-poc1-release' from 'origin'.
Switched to a new branch '163-poc1-release'
Cloning repo: gateway
Cloning into 'fc-retrieval-gateway'...
remote: Enumerating objects: 317, done.
remote: Counting objects: 100% (317/317), done.
remote: Compressing objects: 100% (190/190), done.
remote: Total 1807 (delta 177), reused 199 (delta 95), pack-reused 1490
Receiving objects: 100% (1807/1807), 7.67 MiB | 392.00 KiB/s, done.
Resolving deltas: 100% (1024/1024), done.
Branch '163-poc1-release' set up to track remote branch '163-poc1-release' from 'origin'.
Switched to a new branch '163-poc1-release'
Cloning repo: gateway-admin
Cloning into 'fc-retrieval-gateway-admin'...
remote: Enumerating objects: 36, done.
remote: Counting objects: 100% (36/36), done.
remote: Compressing objects: 100% (24/24), done.
remote: Total 425 (delta 16), reused 25 (delta 10), pack-reused 389
Receiving objects: 100% (425/425), 161.87 KiB | 47.00 KiB/s, done.
Resolving deltas: 100% (202/202), done.
Branch '163-poc1-release' set up to track remote branch '163-poc1-release' from 'origin'.
Switched to a new branch '163-poc1-release'
Cloning repo: itest
Cloning into 'fc-retrieval-itest'...
remote: Enumerating objects: 198, done.
remote: Counting objects: 100% (198/198), done.
remote: Compressing objects: 100% (133/133), done.
remote: Total 883 (delta 119), reused 123 (delta 56), pack-reused 685
Receiving objects: 100% (883/883), 14.80 MiB | 163.00 KiB/s, done.
Resolving deltas: 100% (530/530), done.
Branch '163-poc1-release' set up to track remote branch '163-poc1-release' from 'origin'.
Switched to a new branch '163-poc1-release'
Cloning repo: provider
Cloning into 'fc-retrieval-provider'...
remote: Enumerating objects: 332, done.
remote: Counting objects: 100% (332/332), done.
remote: Compressing objects: 100% (185/185), done.
remote: Total 950 (delta 195), reused 237 (delta 123), pack-reused 618
Receiving objects: 100% (950/950), 2.33 MiB | 371.00 KiB/s, done.
Resolving deltas: 100% (464/464), done.
Branch '163-poc1-release' set up to track remote branch '163-poc1-release' from 'origin'.
Switched to a new branch '163-poc1-release'
Cloning repo: provider-admin
Cloning into 'fc-retrieval-provider-admin'...
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 227 (delta 0), reused 1 (delta 0), pack-reused 223
Receiving objects: 100% (227/227), 106.50 KiB | 403.00 KiB/s, done.
Resolving deltas: 100% (98/98), done.
Branch '163-poc1-release' set up to track remote branch '163-poc1-release' from 'origin'.
Switched to a new branch '163-poc1-release'
Cloning repo: register
Cloning into 'fc-retrieval-register'...
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 587 (delta 4), reused 6 (delta 2), pack-reused 577
Receiving objects: 100% (587/587), 27.53 MiB | 216.00 KiB/s, done.
Resolving deltas: 100% (333/333), done.
Branch '163-poc1-release' set up to track remote branch '163-poc1-release' from 'origin'.
Switched to a new branch '163-poc1-release'
Already on '163-poc1-release'
Your branch is up to date with 'origin/163-poc1-release'.
"docker stop" requires at least 1 argument.
See 'docker stop --help'.

Usage:  docker stop [OPTIONS] CONTAINER [CONTAINER...]

Stop one or more running containers
"docker rm" requires at least 1 argument.
See 'docker rm --help'.

Usage:  docker rm [OPTIONS] CONTAINER [CONTAINER...]

Remove one or more containers
Untagged: consensys/fc-retrieval-itest:dev
Untagged: consensys/fc-retrieval-itest:develop-163-poc1-release
Deleted: sha256:cdb4771bf31362583ebbf4b50f20c4ef89a41e7cc4400920fa0822823c7093c5
Deleted: sha256:39d60d46dc46687cf025ef8962ffefed0aded3f735fb0c1a4ebd544e5eef2350
Deleted: sha256:1892af8919ca53dfebcb22196da437d8fad421a2458b44491ec490d6afe01caa
Deleted: sha256:cfb304b09b49b3f2205dbebaa7889ab5e8dd49a54e701e5de4e785884152a631
Deleted: sha256:7f102300c72fd514589cb2970633dc5fbb470a7ad7e30225b04d2c8b6feb86b3
Deleted: sha256:64e43c7d8ba365e4f541b99f8cbeebb607c0fad0ad10009ddfefd3a736f83f08
Deleted: sha256:6da219314148206c73f66a7ae67fadd8e799fe0f99818202a10ae53fbd981cc2
Deleted: sha256:b320eb346356d3a5b13724f0805f764cc0b763478ef10446be2b16237f93ebd9
Deleted: sha256:91d7bac8ac679540c9c0bf9b3ea101c0c7a8a75fc58fc6c2a8368eeb947654d6
Untagged: consensys/fc-retrieval-provider:dev
Untagged: consensys/fc-retrieval-provider:develop-163-poc1-release
Deleted: sha256:c454a34f6c50b996ff8ec3d06d1c8303ecb56bc6d9431489980bf23ad2015ea3
Deleted: sha256:691cedc30f983a6de202b33d095add7e43f9b39bd4e18cb84aaa24c078dee813
Deleted: sha256:da05087b1f29a2e6eb0c2fd12cdb8d0d64bb2eb07808a7acd7b002ad8d720c05
Deleted: sha256:50db27b621c08a69cafa26fa82d24b8e52ea96154facd8e882d75ddcf64679b5
Deleted: sha256:dd11d14472c68640330efc18ae06c2b4a405ff61cb857881ad76548170a6c64a
Deleted: sha256:1d8fda575be582ec3a94e8ac17b93b99621d7928173dd92577a32d8d29450cb7
Deleted: sha256:36fc605c00460cb41c3fabd2b80cb10ce9e210f6bddb8c636a0ddf380fe0ecc3
Deleted: sha256:ac56f6687fcca2ffd5db30151a304e5d17c19c398f3f724e2de725fb9df3d157
Deleted: sha256:c0842ea2b384c44c649f8e4673d6b8da893c960fe46adb6e73c3d7ed8939a009
Deleted: sha256:c0b7853e02a32ea0c15e21486ff91523a553855939add39836356dee3c7935fb
Deleted: sha256:8f9140f17decfa8515793eb7f3066e032950515f66c94ae6ddf0f2f702d083b9
Deleted: sha256:b8a9a76a01c9b8fc24e8eb2ec04fd8fbd5e098016b4c3ed1f11d94050d8a59c8
Deleted: sha256:2314b137b0f53cde0f103093cf581e995d835ee63843230cc61b8d8e7f9245ee
Untagged: consensys/fc-retrieval-gateway:dev
Untagged: consensys/fc-retrieval-gateway:develop-163-poc1-release
Deleted: sha256:190d19922ca37a264b5f762dbf0cdf9a30ce5bb4fc921b44170a617c392079c8
Deleted: sha256:31e71e438b28d36ea27508c88a198a726b64a81f6b7955845950ef347197d89f
Deleted: sha256:95ff137d539c659a3f4a68ade7141f7e762b1a3745d0a9741162dbabfdf247cb
Deleted: sha256:7b71e194276bbee71aa255767959ede077b81459e3b93ebf19b03feef3261523
Deleted: sha256:9f43ecebac718aceee4c17690f3ddc27d5062a9f6202880e0a0cee2f63289b23
Deleted: sha256:8911f7d4a2556f0833daeff15a9bddfcbbf4bcf7f9bea0f65add8eebe0d46a45
Deleted: sha256:784bed82f02394a3d634dbea7473df96770bbee9b48d56efe33ce1e747a3d022
Deleted: sha256:d8e25bc99b74169e1ef4384afb77ca8e1323b0c0c89fb934d4cfb49902dc8ec7
Deleted: sha256:743790c4e4006025e8c8a462af6f05ba00c3a2839cd2ebb4e1e0f3fbb1a71379
Deleted: sha256:5582cd5f55ccc99fc05f24832f94c4b38ae7b1578ed49b5a64c49dbd75621d88
Deleted: sha256:e63e49f88e8519070c8a8f23b52693f200b6bdd02faab7ec9c434948acc136fb
Deleted: sha256:5b755a361302add3a598c07dedf3a410c3aaaf609b03166da4fba21a8e7a42b0
Deleted: sha256:02baa6122fe1a15738187c59ed583a9a16b28193e8ecc021901744ba7c1ee388
Deleted: sha256:2a574b1541e5eb058eba715f39b7b02b65403f11b36aac7aebcfb5f76199fc98
Deleted: sha256:76a90d79c2a05f3a28614faae12475c1e3e0e65f6f3d239253229777e32fd20b
Untagged: consensys/fc-retrieval-register:dev
Untagged: consensys/fc-retrieval-register:develop-163-poc1-release
Deleted: sha256:f9f79051dd543156a182731e0fd1088e4cefe2feed9b315fa259880356cff90e
Deleted: sha256:99cd734d9e84c6b242cb9826592cac36beefd69c3d1c3ebdcf898fccf274c76b
Deleted: sha256:d31456d9a1b0b7e8d0bb93ff235552051ed64fb89113883669fa09c1268d7d48
Deleted: sha256:724b96088e9be6d94723b00fdf5b8279ff319518b6c66bba1b454e60ce960187
Deleted: sha256:9fb31a913939c20ac2f3ec788d059e8508c29af57ed27e89f7833655be75ef8a
Deleted: sha256:60052615ead0fbf13414dd441eacd79883f4b29e528504367dee0ae8ada4e97e
Deleted: sha256:f69de7c7049b8bd118538e018f6e6356304dac1d0914401e2e6c15d93f14920b
Deleted: sha256:61ed2e602d6dad74531d82e3d218314304f5acbc00f26808b6dcd3bf68f9c1f3
Deleted: sha256:5dc74ba82a5b9df657e497618b9bff2ce3ce812da845263f3161fe594b0e6231
Deleted: sha256:5a45c3ff3d1fa64082a1a8b415589968164a1ad860910ef6c9787bf808039c5e
Deleted: sha256:d229218ffdd9cc3f1dd60ee73c44fad9b7e463c9316761da6d11d97a16cf6c6e
Deleted: sha256:759bb4cc624e6c18a26eed52c7ed9fc726140cfc5317f422281148933eaf4adb
Deleted: sha256:aeda30aab9f7bf5b72ac285c2a30fbbc6f76867d2672d2abb6cbca5a88aa7eab
Deleted: sha256:28a2e37bad7414385e65a000b909c500edf7c8b51ffa6daafd67d13d4030899d
Deleted: sha256:9ac571777f22a993454c53f898e01eecde4dc9d918a431099cbf1d0a34a3f06a
Untagged: redis:alpine
Untagged: redis@sha256:46857d41d722c11b06f66a4006eb77e6c7180a98d35c48562c5a347e9eb4ec54
Deleted: sha256:5812dfe24a4fd91ce8c5d0b2667fec71259674a2e37c08fda9a9d15a9ff2feb0
Deleted: sha256:b27ebbb9b93d717c498352e8986a6354c0ff770dc9a28fc60c54dfeb782d782e
Deleted: sha256:410c52590216835ec400e62619755d2c9752de6d005cfb07a9ef5467f50b8b5d
Deleted: sha256:9a307a2a321d2a2f0a1e3b72b95a3825ba9eadc1497f205a57a4b0ab04fdd42e
Deleted: sha256:d73fb481b31bda1e82403e3dcc3735954af8884f846400618ec6c3593e8f067a
Deleted: sha256:3c84e760ab315b017012d6ad7230f4033cbd97b2f1eea0719689c822c7594cea
Untagged: golang:1.15-alpine
Untagged: golang@sha256:a025015951720f3227acd51b0a99a71578b574a63172ea7d2415c60ae5e2bc0a
Deleted: sha256:b8d8ad7b4ab7b5b21e2b44393ad8fbfcf12536d0da5642dde6525428455f615b
Deleted: sha256:988f2e5ec0bb8cdccaa5762f492cea1aa16b8df71e8d14ea52ccef7c6cb057b1
Deleted: sha256:1fd4dd9a929bb33a0990a4190d46b8c7b9adb6658806b5cd313840be7622324e
Deleted: sha256:eaf2bb5c67628b08c13264807d9486fd4eea42e5d299bea2c25b2e660ddcfd98
Deleted: sha256:2244b63cd85ece426753f7e7605d7b193e40c19a432da881aefb5c4acca4fa73
Untagged: alpine:latest
Untagged: alpine@sha256:a75afd8b57e7f34e4dad8d65e2c7ba2e1975c795ce1ee22fa34f8cf46f96a3be
Deleted: sha256:28f6e27057430ed2a40dbdd50d2736a3f0a295924016e294938110eeb8439818
Deleted: sha256:cb381a32b2296e4eb5af3f84092a2e6685e88adbc54ee0768a1a1010ce6376c7
Error: No such image: cdb4771bf313
Error: No such image: c454a34f6c50
Error: No such image: 190d19922ca3
Error: No such image: f9f79051dd54
Docker containers:
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
Docker images:
REPOSITORY   TAG       IMAGE ID   CREATED   SIZE
Already on '163-poc1-release'
Your branch is up to date with 'origin/163-poc1-release'.
Checking repo: register
cd scripts; bash use-remote-repos.sh
*******************************************************************************
*** Update go.mod and go.sum to point to the latest packages on github.com  ***
*** for gateway.                                                            ***
*******************************************************************************
register repo branch: 163-poc1-release
Found common repo: ../fc-retrieval-common
common repo branch: 163-poc1-release
register and common branch match
Calling go get to use 163-poc1-release on fc-retrieval-common (4caead038a43ff524b8fc68055320e7b84ff3173)
Checking repo: client
cd scripts; bash use-remote-repos.sh
*******************************************************************************
*** Update go.mod and go.sum to point to the latest packages on github.com  ***
*** for gateway.                                                            ***
*******************************************************************************
client repo branch: 163-poc1-release
Found common repo: ../fc-retrieval-common
common repo branch: 163-poc1-release
client and common branch match
Calling go get to use 163-poc1-release on fc-retrieval-common (4caead038a43ff524b8fc68055320e7b84ff3173)
Found register repo: ../fc-retrieval-register
register repo branch: 163-poc1-release
client and register branch match
Calling go get to use 163-poc1-release on fc-retrieval-register (57ff758e2e2c14443aefc4263f93cd21df64ea4d)
Checking repo: provider-admin
cd scripts; bash use-remote-repos.sh
*******************************************************************************
*** Update go.mod and go.sum to point to the latest packages on github.com  ***
*** for gateway.                                                            ***
*******************************************************************************
provider-admin repo branch: 163-poc1-release
Found client repo: ../fc-retrieval-client
client repo branch: 163-poc1-release
gateway admin and client branch match
Calling go get to use 163-poc1-release on fc-retrieval-client (b5a58266695e533b1c45a260b130c600ac6a6a39)
go: github.com/ConsenSys/fc-retrieval-client b5a58266695e533b1c45a260b130c600ac6a6a39 => v0.0.0-20210315220115-b5a58266695e
Found common repo: ../fc-retrieval-common
common repo branch: 163-poc1-release
gateway admin and common branch match
Calling go get to use 163-poc1-release on fc-retrieval-common (4caead038a43ff524b8fc68055320e7b84ff3173)
Found provider repo: ../fc-retrieval-provider
provider repo branch: 163-poc1-release
gateway admin and provider branch match
Calling go get to use 163-poc1-release on fc-retrieval-provider (40ceb1a5a113b14082bea6f83da3f0a9240030bd)
go: github.com/ConsenSys/fc-retrieval-provider 40ceb1a5a113b14082bea6f83da3f0a9240030bd => v0.0.0-20210315220342-40ceb1a5a113
Found register repo: ../fc-retrieval-register
register repo branch: 163-poc1-release
gateway admin and register branch match
Calling go get to use 163-poc1-release on fc-retrieval-register (57ff758e2e2c14443aefc4263f93cd21df64ea4d)
Checking repo: gateway-admin
cd scripts; bash use-remote-repos.sh
*******************************************************************************
*** Update go.mod and go.sum to point to the latest packages on github.com  ***
*** for gateway.                                                            ***
*******************************************************************************
gateway-admin repo branch: 163-poc1-release
Found common repo: ../fc-retrieval-common
common repo branch: 163-poc1-release
gateway admin and common branch match
Calling go get to use 163-poc1-release on fc-retrieval-common (4caead038a43ff524b8fc68055320e7b84ff3173)
Found register repo: ../fc-retrieval-register
register repo branch: 163-poc1-release
gateway admin and register branch match
Calling go get to use 163-poc1-release on fc-retrieval-register (57ff758e2e2c14443aefc4263f93cd21df64ea4d)
Checking repo: gateway
cd scripts; bash use-remote-repos.sh
*******************************************************************************
*** Update go.mod and go.sum to point to the latest packages on github.com  ***
*** for client, gateway, gateway-admin, and provider-admin.                 ***
*******************************************************************************
gateway repo branch: 163-poc1-release
Found common repo: ../fc-retrieval-common
common repo branch: 163-poc1-release
itest and common branch match
Calling go get to use 163-poc1-release on fc-retrieval-common (4caead038a43ff524b8fc68055320e7b84ff3173)
Found register repo: ../fc-retrieval-register
register repo branch: 163-poc1-release
itest and register branch match
Calling go get to use 163-poc1-release on fc-retrieval-register (57ff758e2e2c14443aefc4263f93cd21df64ea4d)
Checking repo: provider
cd scripts; bash use-remote-repos.sh
*******************************************************************************
*** Update go.mod and go.sum to point to the latest packages on github.com  ***
*** for gateway.                                                            ***
*******************************************************************************
provider repo branch: 163-poc1-release
Found common repo: ../fc-retrieval-common
common repo branch: 163-poc1-release
register and common branch match
Calling go get to use 163-poc1-release on fc-retrieval-common (4caead038a43ff524b8fc68055320e7b84ff3173)
Found register repo: ../fc-retrieval-register
register repo branch: 163-poc1-release
register and register branch match
Calling go get to use 163-poc1-release on fc-retrieval-register (57ff758e2e2c14443aefc4263f93cd21df64ea4d)
docker build -f Dockerfile -t consensys/fc-retrieval-register:dev .
Sending build context to Docker daemon  31.85MB
Step 1/11 : FROM golang:1.15-alpine as builder
1.15-alpine: Pulling from library/golang
ba3557a56b15: Pull complete 
448433d692de: Pull complete 
7c2a3d42746f: Pull complete 
d3242f58a67e: Pull complete 
d9e3b7eac99f: Pull complete 
Digest: sha256:a025015951720f3227acd51b0a99a71578b574a63172ea7d2415c60ae5e2bc0a
Status: Downloaded newer image for golang:1.15-alpine
 ---> b8d8ad7b4ab7
Step 2/11 : RUN apk update && apk add --no-cache make gcc musl-dev linux-headers git
 ---> Running in e2411db9549a
fetch https://dl-cdn.alpinelinux.org/alpine/v3.13/main/x86_64/APKINDEX.tar.gz
fetch https://dl-cdn.alpinelinux.org/alpine/v3.13/community/x86_64/APKINDEX.tar.gz
v3.13.2-83-g73a7825440 [https://dl-cdn.alpinelinux.org/alpine/v3.13/main]
v3.13.2-84-g27aaf862b6 [https://dl-cdn.alpinelinux.org/alpine/v3.13/community]
OK: 13878 distinct packages available
fetch https://dl-cdn.alpinelinux.org/alpine/v3.13/main/x86_64/APKINDEX.tar.gz
fetch https://dl-cdn.alpinelinux.org/alpine/v3.13/community/x86_64/APKINDEX.tar.gz
(1/20) Installing libgcc (10.2.1_pre1-r3)
(2/20) Installing libstdc++ (10.2.1_pre1-r3)
(3/20) Installing binutils (2.35.1-r1)
(4/20) Installing libgomp (10.2.1_pre1-r3)
(5/20) Installing libatomic (10.2.1_pre1-r3)
(6/20) Installing libgphobos (10.2.1_pre1-r3)
(7/20) Installing gmp (6.2.1-r0)
(8/20) Installing isl22 (0.22-r0)
(9/20) Installing mpfr4 (4.1.0-r0)
(10/20) Installing mpc1 (1.2.0-r0)
(11/20) Installing gcc (10.2.1_pre1-r3)
(12/20) Installing brotli-libs (1.0.9-r3)
(13/20) Installing nghttp2-libs (1.42.0-r1)
(14/20) Installing libcurl (7.74.0-r1)
(15/20) Installing expat (2.2.10-r1)
(16/20) Installing pcre2 (10.36-r0)
(17/20) Installing git (2.30.2-r0)
(18/20) Installing linux-headers (5.7.8-r0)
(19/20) Installing make (4.3-r0)
(20/20) Installing musl-dev (1.2.2-r0)
Executing busybox-1.32.1-r3.trigger
OK: 146 MiB in 35 packages
Removing intermediate container e2411db9549a
 ---> a38f28ed7310
Step 3/11 : WORKDIR /go/src/github.com/ConsenSys/fc-retrieval-register/
 ---> Running in 8dc0c66f97f1
Removing intermediate container 8dc0c66f97f1
 ---> 3af7f0345679
Step 4/11 : COPY . .
 ---> f7deee21d2cc
Step 5/11 : RUN go get -d -v github.com/ConsenSys/fc-retrieval-register/cmd/register-server
 ---> Running in 5084b4da5265
go: downloading github.com/go-openapi/loads v0.20.2
go: downloading github.com/jessevdk/go-flags v1.4.0
go: downloading github.com/go-openapi/runtime v0.19.24
go: downloading github.com/go-openapi/errors v0.19.9
go: downloading github.com/go-openapi/swag v0.19.14
go: downloading github.com/go-openapi/strfmt v0.20.0
go: downloading golang.org/x/net v0.0.0-20210226172049-e18ecbb05110
go: downloading github.com/ConsenSys/fc-retrieval-common v0.0.0-20210312151557-4caead038a43
go: downloading github.com/go-redis/redis/v8 v8.6.0
go: downloading github.com/go-openapi/spec v0.20.3
go: downloading github.com/rs/cors v1.7.0
go: downloading go.mongodb.org/mongo-driver v1.4.6
go: downloading github.com/go-openapi/validate v0.20.2
go: downloading github.com/go-openapi/analysis v0.20.0
go: downloading gopkg.in/natefinch/lumberjack.v2 v2.0.0
go: downloading github.com/cespare/xxhash v1.1.0
go: downloading github.com/mailru/easyjson v0.7.6
go: downloading go.opentelemetry.io/otel v0.17.0
go: downloading github.com/cespare/xxhash/v2 v2.1.1
go: downloading github.com/rs/zerolog v1.20.0
go: downloading github.com/mitchellh/mapstructure v1.4.1
go: downloading go.opentelemetry.io/otel/trace v0.17.0
go: downloading go.opentelemetry.io/otel/metric v0.17.0
go: downloading github.com/spf13/viper v1.7.1
go: downloading github.com/dgryski/go-rendezvous v0.0.0-20200823014737-9f7001d12a5f
go: downloading gopkg.in/yaml.v2 v2.4.0
go: downloading github.com/go-openapi/jsonpointer v0.19.5
go: downloading github.com/pelletier/go-toml v1.7.0
go: downloading github.com/subosito/gotenv v1.2.0
go: downloading github.com/josharian/intern v1.0.0
go: downloading github.com/spf13/jwalterweatherman v1.0.0
go: downloading github.com/hashicorp/hcl v1.0.0
go: downloading github.com/spf13/pflag v1.0.3
go: downloading github.com/go-stack/stack v1.8.0
go: downloading github.com/fsnotify/fsnotify v1.4.9
go: downloading github.com/go-openapi/jsonreference v0.19.5
go: downloading github.com/magiconair/properties v1.8.1
go: downloading github.com/asaskevich/govalidator v0.0.0-20200907205600-7a23bdc65eef
go: downloading github.com/docker/go-units v0.4.0
go: downloading github.com/spf13/afero v1.1.2
go: downloading gopkg.in/ini.v1 v1.51.0
go: downloading github.com/spf13/cast v1.3.0
go: downloading golang.org/x/sys v0.0.0-20210112080510-489259a85091
go: downloading github.com/PuerkitoBio/purell v1.1.1
go: downloading golang.org/x/text v0.3.5
go: downloading github.com/PuerkitoBio/urlesc v0.0.0-20170810143723-de5bf2ad4578
Removing intermediate container 5084b4da5265
 ---> ff6c00392fbd
Step 6/11 : RUN CGO_ENABLED=1 GOOS=linux go build -a -installsuffix cgo -o /go/bin/register-server ./cmd/register-server
 ---> Running in ae008f787090
Removing intermediate container ae008f787090
 ---> d97a0b178d19
Step 7/11 : FROM alpine:latest
latest: Pulling from library/alpine
ba3557a56b15: Already exists 
Digest: sha256:a75afd8b57e7f34e4dad8d65e2c7ba2e1975c795ce1ee22fa34f8cf46f96a3be
Status: Downloaded newer image for alpine:latest
 ---> 28f6e2705743
Step 8/11 : COPY --from=builder /go/bin/register-server /register-server
 ---> 1af863147082
Step 9/11 : WORKDIR /
 ---> Running in e464cc377089
Removing intermediate container e464cc377089
 ---> a4e58c06c2c6
Step 10/11 : CMD ["/register-server", "--host", "0.0.0.0", "--port", "9020"]
 ---> Running in 5603748f2c41
Removing intermediate container 5603748f2c41
 ---> e17e45352f92
Step 11/11 : EXPOSE 9020
 ---> Running in 9322e2eb9f52
Removing intermediate container 9322e2eb9f52
 ---> 948418d69acb
Successfully built 948418d69acb
Successfully tagged consensys/fc-retrieval-register:dev
cd scripts; bash tag.sh dev consensys/fc-retrieval-register:dev
****************************************
*** Push docker image to Docker Hub  ***
****************************************
Register version: dev
v image: consensys/fc-retrieval-register:dev
Register repo branch: 163-poc1-release
TAG: develop-163-poc1-release
docker build -t consensys/fc-retrieval-gateway:dev .
Sending build context to Docker daemon   2.79MB
Step 1/12 : FROM golang:1.15-alpine as builder
 ---> b8d8ad7b4ab7
Step 2/12 : RUN apk update && apk add --no-cache make gcc musl-dev linux-headers git
 ---> Using cache
 ---> a38f28ed7310
Step 3/12 : WORKDIR /go/src/github.com/ConsenSys/fc-retrieval-gateway
 ---> Running in 46b9d408da33
Removing intermediate container 46b9d408da33
 ---> 0510391a7c03
Step 4/12 : COPY . .
 ---> e72fb819dadb
Step 5/12 : RUN go get -d -v github.com/ConsenSys/fc-retrieval-gateway/cmd/gateway
 ---> Running in 3a746bbe1095
go: downloading github.com/ConsenSys/fc-retrieval-common v0.0.0-20210312151557-4caead038a43
go: downloading github.com/spf13/viper v1.7.1
go: downloading github.com/joho/godotenv v1.3.0
go: downloading github.com/ConsenSys/fc-retrieval-register v0.0.0-20210315215728-57ff758e2e2c
go: downloading github.com/spf13/pflag v1.0.5
go: downloading gopkg.in/natefinch/lumberjack.v2 v2.0.0
go: downloading github.com/rs/zerolog v1.20.0
go: downloading golang.org/x/crypto v0.0.0-20210220033148-5ea612d1eb83
go: downloading github.com/ipsn/go-secp256k1 v0.0.0-20180726113642-9d62b9f0bc52
go: downloading github.com/cbergoon/merkletree v0.2.0
go: downloading github.com/davidlazar/go-crypto v0.0.0-20200604182044-b73af7476f6c
go: downloading github.com/spf13/cast v1.3.0
go: downloading github.com/hashicorp/hcl v1.0.0
go: downloading github.com/spf13/jwalterweatherman v1.0.0
go: downloading github.com/subosito/gotenv v1.2.0
go: downloading github.com/fsnotify/fsnotify v1.4.9
go: downloading github.com/pelletier/go-toml v1.7.0
go: downloading gopkg.in/yaml.v2 v2.4.0
go: downloading gopkg.in/ini.v1 v1.51.0
go: downloading github.com/mitchellh/mapstructure v1.4.1
go: downloading github.com/magiconair/properties v1.8.1
go: downloading github.com/spf13/afero v1.1.2
go: downloading github.com/ant0ine/go-json-rest v3.3.2+incompatible
go: downloading golang.org/x/sys v0.0.0-20210112080510-489259a85091
go: downloading golang.org/x/text v0.3.5
Removing intermediate container 3a746bbe1095
 ---> 1efa25ade4a9
Step 6/12 : RUN CGO_ENABLED=1 GOOS=linux go build -a -installsuffix cgo -o /go/bin/gateway ./cmd/gateway
 ---> Running in 52975601e26c
Removing intermediate container 52975601e26c
 ---> acde3028dcef
Step 7/12 : FROM alpine:latest
 ---> 28f6e2705743
Step 8/12 : COPY --from=builder /go/bin/gateway /main
 ---> 78d96b27b7ae
Step 9/12 : COPY docker-entrypoint.sh /docker-entrypoint.sh
 ---> db6d91dea8b4
Step 10/12 : WORKDIR /
 ---> Running in 1766669cdd1d
Removing intermediate container 1766669cdd1d
 ---> 1b311979cefe
Step 11/12 : CMD ["./docker-entrypoint.sh"]
 ---> Running in 373877b05f90
Removing intermediate container 373877b05f90
 ---> 7226d141f43a
Step 12/12 : EXPOSE 9010
 ---> Running in 1d56ea664a87
Removing intermediate container 1d56ea664a87
 ---> 8360536a0059
Successfully built 8360536a0059
Successfully tagged consensys/fc-retrieval-gateway:dev
cd scripts; bash tag.sh dev consensys/fc-retrieval-gateway:dev
****************************************
*** Tag docker image with branch name  ***
****************************************
Gateway version: dev
Gateway image: consensys/fc-retrieval-gateway:dev
Gateway repo branch: 163-poc1-release
TAG: develop-163-poc1-release
docker build -t consensys/fc-retrieval-provider:dev .
Sending build context to Docker daemon  2.742MB
Step 1/11 : FROM golang:1.15-alpine as builder
 ---> b8d8ad7b4ab7
Step 2/11 : RUN apk update && apk add --no-cache make gcc musl-dev linux-headers git
 ---> Using cache
 ---> a38f28ed7310
Step 3/11 : WORKDIR /go/src/github.com/ConsenSys/fc-retrieval-provider/
 ---> Running in f5dd2f8c8abd
Removing intermediate container f5dd2f8c8abd
 ---> 05b9eee8969e
Step 4/11 : COPY . .
 ---> 5b9c6fe3705d
Step 5/11 : RUN go get -d -v github.com/ConsenSys/fc-retrieval-provider/cmd/provider
 ---> Running in d8d4edb58463
go: downloading github.com/ConsenSys/fc-retrieval-common v0.0.0-20210312151557-4caead038a43
go: downloading github.com/ConsenSys/fc-retrieval-register v0.0.0-20210315215728-57ff758e2e2c
go: downloading github.com/joho/godotenv v1.3.0
go: downloading github.com/spf13/pflag v1.0.3
go: downloading github.com/spf13/viper v1.7.1
go: downloading github.com/ant0ine/go-json-rest v3.3.2+incompatible
go: downloading github.com/ipsn/go-secp256k1 v0.0.0-20180726113642-9d62b9f0bc52
go: downloading github.com/rs/zerolog v1.20.0
go: downloading github.com/cbergoon/merkletree v0.2.0
go: downloading github.com/davidlazar/go-crypto v0.0.0-20200604182044-b73af7476f6c
go: downloading golang.org/x/crypto v0.0.0-20210220033148-5ea612d1eb83
go: downloading gopkg.in/natefinch/lumberjack.v2 v2.0.0
go: downloading github.com/magiconair/properties v1.8.1
go: downloading github.com/spf13/afero v1.1.2
go: downloading github.com/hashicorp/hcl v1.0.0
go: downloading github.com/subosito/gotenv v1.2.0
go: downloading github.com/spf13/jwalterweatherman v1.0.0
go: downloading github.com/spf13/cast v1.3.0
go: downloading github.com/mitchellh/mapstructure v1.4.1
go: downloading github.com/pelletier/go-toml v1.7.0
go: downloading gopkg.in/ini.v1 v1.51.0
go: downloading gopkg.in/yaml.v2 v2.4.0
go: downloading golang.org/x/text v0.3.5
go: downloading github.com/fsnotify/fsnotify v1.4.9
go: downloading golang.org/x/sys v0.0.0-20210112080510-489259a85091
Removing intermediate container d8d4edb58463
 ---> 5e2693c0fe19
Step 6/11 : RUN CGO_ENABLED=1 GOOS=linux go build -a -installsuffix cgo -o /go/bin/provider ./cmd/provider
 ---> Running in c09849b464c0
Removing intermediate container c09849b464c0
 ---> 2ed77f14e7f1
Step 7/11 : FROM alpine:latest
 ---> 28f6e2705743
Step 8/11 : COPY --from=builder /go/bin/provider /provider
 ---> a75be0deb412
Step 9/11 : WORKDIR /
 ---> Running in 42f48e5f0c27
Removing intermediate container 42f48e5f0c27
 ---> 484bc787eabf
Step 10/11 : CMD ["/provider"]
 ---> Running in b147efaf685d
Removing intermediate container b147efaf685d
 ---> 27040ceccc10
Step 11/11 : EXPOSE 9030
 ---> Running in 868cd6d2d167
Removing intermediate container 868cd6d2d167
 ---> c7cc8ac646b8
Successfully built c7cc8ac646b8
Successfully tagged consensys/fc-retrieval-provider:dev
cd scripts; bash tag.sh dev consensys/fc-retrieval-provider:dev
****************************************
*** Tag docker image with the branch name  ***
****************************************
Register version: dev
v image: consensys/fc-retrieval-provider:dev
Provider repo branch: 163-poc1-release
TAG: develop-163-poc1-release
docker build -t consensys/fc-retrieval-itest:dev .
Sending build context to Docker daemon  32.91MB
Step 1/6 : FROM golang:1.15-alpine
 ---> b8d8ad7b4ab7
Step 2/6 : RUN apk add --no-cache make gcc musl-dev linux-headers git
 ---> Running in 20248eac925d
fetch https://dl-cdn.alpinelinux.org/alpine/v3.13/main/x86_64/APKINDEX.tar.gz
fetch https://dl-cdn.alpinelinux.org/alpine/v3.13/community/x86_64/APKINDEX.tar.gz
(1/20) Installing libgcc (10.2.1_pre1-r3)
(2/20) Installing libstdc++ (10.2.1_pre1-r3)
(3/20) Installing binutils (2.35.1-r1)
(4/20) Installing libgomp (10.2.1_pre1-r3)
(5/20) Installing libatomic (10.2.1_pre1-r3)
(6/20) Installing libgphobos (10.2.1_pre1-r3)
(7/20) Installing gmp (6.2.1-r0)
(8/20) Installing isl22 (0.22-r0)
(9/20) Installing mpfr4 (4.1.0-r0)
(10/20) Installing mpc1 (1.2.0-r0)
(11/20) Installing gcc (10.2.1_pre1-r3)
(12/20) Installing brotli-libs (1.0.9-r3)
(13/20) Installing nghttp2-libs (1.42.0-r1)
(14/20) Installing libcurl (7.74.0-r1)
(15/20) Installing expat (2.2.10-r1)
(16/20) Installing pcre2 (10.36-r0)
(17/20) Installing git (2.30.2-r0)
(18/20) Installing linux-headers (5.7.8-r0)
(19/20) Installing make (4.3-r0)
(20/20) Installing musl-dev (1.2.2-r0)
Executing busybox-1.32.1-r3.trigger
OK: 146 MiB in 35 packages
Removing intermediate container 20248eac925d
 ---> bc24477859f1
Step 3/6 : WORKDIR /go/src/github.com/ConsenSys/fc-retrieval-itest
 ---> Running in 1a3746c60cb9
Removing intermediate container 1a3746c60cb9
 ---> 860537b28d33
Step 4/6 : COPY . .
 ---> 3a949f30d229
Step 5/6 : RUN go clean -modcache
 ---> Running in 8b2fc9230c78
Removing intermediate container 8b2fc9230c78
 ---> 855b9a2ced4d
Step 6/6 : CMD go test -v ./...
 ---> Running in 808a3fdd43bb
Removing intermediate container 808a3fdd43bb
 ---> a49fef1cc391
Successfully built a49fef1cc391
Successfully tagged consensys/fc-retrieval-itest:dev
cd scripts; bash tag.sh dev consensys/fc-retrieval-itest:dev
****************************************
*** Tag docker image with the branch name  ***
****************************************
Itest version: dev
v image: consensys/fc-retrieval-itest:dev
Repo branch: 163-poc1-release
TAG: develop-163-poc1-release
cd scripts; bash setup-env.sh
*******************************************************************************
*** Set-up the env file  ***
*******************************************************************************
itest repo branch: 163-poc1-release
Found gateway repo: ../fc-retrieval-gateway
gateway repo branch: 163-poc1-release
/dev/clonebuildtest/163-poc1-release/fc-retrieval-itest
Found register repo: ../fc-retrieval-register
register repo branch: 163-poc1-release
/dev/clonebuildtest/163-poc1-release/fc-retrieval-itest
Found provider repo: ../fc-retrieval-provider
provider repo branch: 163-poc1-release
/dev/clonebuildtest/163-poc1-release/fc-retrieval-itest
Found itest repo: ../fc-retrieval-itest
itest repo branch: 163-poc1-release
/dev/clonebuildtest/163-poc1-release/fc-retrieval-itest
GATEWAY_IMAGE=consensys/fc-retrieval-gateway:develop-163-poc1-release
REGISTER_IMAGE=consensys/fc-retrieval-register:develop-163-poc1-release
PROVIDER_IMAGE=consensys/fc-retrieval-provider:develop-163-poc1-release
ITEST_IMAGE=consensys/fc-retrieval-itest:develop-163-poc1-release
docker network create shared || true
Error response from daemon: network with name shared already exists
docker-compose down
Network shared is external, skipping
for file in ./internal/integration/* ; do \
		docker-compose -f docker-compose.yml up -d gateway provider register redis; \
		echo *********************************************; \
		sleep 10; \
		echo REDIS STARTUP *********************************************; \
		docker container logs redis; \
		echo REGISTER STARTUP *********************************************; \
		docker container logs register; \
		echo GATEWAY STARTUP *********************************************; \
		docker container logs gateway; \
		echo PROVIDER STARTUP *********************************************; \
		docker container logs provider; \
		echo *********************************************; \
		docker-compose run itest go test -v $file; \
		echo *********************************************; \
		echo PROVIDER LOGS *********************************************; \
		docker container logs provider; \
		echo GATEWAY LOGS *********************************************; \
		docker container logs gateway; \
		docker-compose down; \
	done
Pulling redis (redis:alpine)...
alpine: Pulling from library/redis
ba3557a56b15: Already exists
dd0c990d86c1: Pull complete
ad7f820ad385: Pull complete
b63501c03b63: Pull complete
e9a2c580f699: Pull complete
d8df53b22447: Pull complete
Digest: sha256:46857d41d722c11b06f66a4006eb77e6c7180a98d35c48562c5a347e9eb4ec54
Status: Downloaded newer image for redis:alpine
Creating redis ... done
Creating register ... done
Creating gateway  ... done
Creating provider ... done
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
REDIS STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
1:C 16 Mar 2021 02:35:32.081 # oO0OoO0OoO0Oo Redis is starting oO0OoO0OoO0Oo
1:C 16 Mar 2021 02:35:32.081 # Redis version=6.2.1, bits=64, commit=00000000, modified=0, pid=1, just started
1:C 16 Mar 2021 02:35:32.081 # Warning: no config file specified, using the default config. In order to specify a config file use redis-server /path/to/redis.conf
1:M 16 Mar 2021 02:35:32.082 * monotonic clock: POSIX clock_gettime
1:M 16 Mar 2021 02:35:32.083 * Running mode=standalone, port=6379.
1:M 16 Mar 2021 02:35:32.083 # WARNING: The TCP backlog setting of 511 cannot be enforced because /proc/sys/net/core/somaxconn is set to the lower value of 128.
1:M 16 Mar 2021 02:35:32.083 # Server initialized
1:M 16 Mar 2021 02:35:32.083 * Ready to accept connections
REGISTER STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
2021/03/16 02:35:32 Serving register at http://[::]:9020
GATEWAY STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Container IP: 172.18.0.4
Starting service ...
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Filecoin Gateway Start-up: Started"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Settings: {BindRestAPI:9010 BindProviderAPI:9011 BindGatewayAPI:9012 BindAdminAPI:9013 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-gateway LogFile:gateway.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true GatewayID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F RegisterAPIURL:http://register:9020 GatewayAddress:f0121345 NetworkInfoGateway:172.18.0.4:9012 GatewayRegionCode:US GatewayRootSigningKey:0xABCDE123456789 GatewaySigningKey:0x987654321EDCBA NetworkInfoClient:172.18.0.4:9010 NetworkInfoProvider:172.18.0.4:9011 NetworkInfoAdmin:172.18.0.4:9013}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"All registered gateways: []"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Running REST API on: 9010"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Listening on 9012 for connections from Gateways"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Listening on 9011 for connections from Providers\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Listening on 9013 for connections from admin clients"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Filecoin Gateway Start-up Complete"}
PROVIDER STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Filecoin Provider Start-up: Started"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Settings: {BindRestAPI:9030 BindGatewayAPI:9032 BindAdminAPI:9033 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-provider LogFile:provider.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true ProviderID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F ProviderSigAlg:1 RegisterAPIURL:http://register:9020 ProviderAddress:f0121345 ProviderRootSigningKey:0xABCDE123456789 ProviderSigningKey:0x987654321EDCBA ProviderRegionCode:US NetworkInfoClient:127.0.0.1: NetworkInfoGateway:127.0.0.1: NetworkInfoAdmin:127.0.0.1:}"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Running REST API on: 9030"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Listening on 9032 for connections from Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Running Admin API on: 9033"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Filecoin Provider Start-up Complete"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Update registered Gateways"}
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Creating fc-retrieval-itest_itest_run ... done
go: downloading github.com/ConsenSys/fc-retrieval-common v0.0.0-20210312151557-4caead038a43
go: downloading github.com/stretchr/testify v1.7.0
go: downloading github.com/ConsenSys/fc-retrieval-client v0.0.0-20210315220115-b5a58266695e
go: downloading github.com/rs/zerolog v1.20.0
go: downloading gopkg.in/natefinch/lumberjack.v2 v2.0.0
go: downloading github.com/ipsn/go-secp256k1 v0.0.0-20180726113642-9d62b9f0bc52
go: downloading github.com/spf13/viper v1.7.1
go: downloading github.com/davidlazar/go-crypto v0.0.0-20200604182044-b73af7476f6c
go: downloading golang.org/x/crypto v0.0.0-20210220033148-5ea612d1eb83
go: downloading gopkg.in/yaml.v3 v3.0.0-20210107192922-496545a6307b
go: downloading github.com/davecgh/go-spew v1.1.1
go: downloading github.com/cbergoon/merkletree v0.2.0
go: downloading github.com/ConsenSys/fc-retrieval-register v0.0.0-20210315215728-57ff758e2e2c
go: downloading github.com/pmezard/go-difflib v1.0.0
go: downloading github.com/tatsushid/go-fastping v0.0.0-20160109021039-d7bb493dee3e
go: downloading github.com/magiconair/properties v1.8.1
go: downloading github.com/hashicorp/hcl v1.0.0
go: downloading github.com/spf13/afero v1.1.2
go: downloading github.com/subosito/gotenv v1.2.0
go: downloading gopkg.in/yaml.v2 v2.4.0
go: downloading gopkg.in/ini.v1 v1.51.0
go: downloading github.com/fsnotify/fsnotify v1.4.9
go: downloading github.com/mitchellh/mapstructure v1.4.1
go: downloading github.com/spf13/cast v1.3.0
go: downloading github.com/spf13/pflag v1.0.5
go: downloading golang.org/x/text v0.3.5
go: downloading golang.org/x/net v0.0.0-20210226172049-e18ecbb05110
go: downloading github.com/spf13/jwalterweatherman v1.0.0
go: downloading golang.org/x/sys v0.0.0-20210301091718-77cc2087c03b
go: downloading github.com/pelletier/go-toml v1.8.1
=== RUN   TestGetClientVersion
--- PASS: TestGetClientVersion (0.00s)
=== RUN   TestInitClientNoRetrievalKey
{"level":"info","service":"client","time":"2021-03-16T02:36:40Z","message":"Settings: No Client ID set. Generating random client ID"}
{"level":"info","service":"client","time":"2021-03-16T02:36:40Z","message":"Filecoin Retrieval Client started"}
--- PASS: TestInitClientNoRetrievalKey (0.00s)
=== RUN   TestNoConfiguredGateways
{"level":"info","service":"client","time":"2021-03-16T02:36:40Z","message":"Get gateways to use"}
--- PASS: TestNoConfiguredGateways (0.00s)
=== RUN   TestUnknownGatewayAdded
{"level":"info","service":"client","time":"2021-03-16T02:36:40Z","message":"Add gateways to use"}
{"level":"warn","service":"client","time":"2021-03-16T02:36:40Z","message":"Gateway registration issue: NodeID not set"}
{"level":"error","service":"client","time":"2021-03-16T02:36:40Z","message":"Register info not valid."}
{"level":"info","service":"client","time":"2021-03-16T02:36:40Z","message":"Get gateways to use"}
{"level":"info","service":"client","time":"2021-03-16T02:36:41Z","message":"Get active gateways"}
--- PASS: TestUnknownGatewayAdded (0.51s)
PASS
ok  	command-line-arguments	0.540s
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
PROVIDER LOGS Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Filecoin Provider Start-up: Started"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Settings: {BindRestAPI:9030 BindGatewayAPI:9032 BindAdminAPI:9033 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-provider LogFile:provider.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true ProviderID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F ProviderSigAlg:1 RegisterAPIURL:http://register:9020 ProviderAddress:f0121345 ProviderRootSigningKey:0xABCDE123456789 ProviderSigningKey:0x987654321EDCBA ProviderRegionCode:US NetworkInfoClient:127.0.0.1: NetworkInfoGateway:127.0.0.1: NetworkInfoAdmin:127.0.0.1:}"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Running REST API on: 9030"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Listening on 9032 for connections from Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Running Admin API on: 9033"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Filecoin Provider Start-up Complete"}
{"level":"info","service":"provider","time":"2021-03-16T02:35:33Z","message":"Update registered Gateways"}
GATEWAY LOGS Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Container IP: 172.18.0.4
Starting service ...
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Filecoin Gateway Start-up: Started"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Settings: {BindRestAPI:9010 BindProviderAPI:9011 BindGatewayAPI:9012 BindAdminAPI:9013 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-gateway LogFile:gateway.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true GatewayID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F RegisterAPIURL:http://register:9020 GatewayAddress:f0121345 NetworkInfoGateway:172.18.0.4:9012 GatewayRegionCode:US GatewayRootSigningKey:0xABCDE123456789 GatewaySigningKey:0x987654321EDCBA NetworkInfoClient:172.18.0.4:9010 NetworkInfoProvider:172.18.0.4:9011 NetworkInfoAdmin:172.18.0.4:9013}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"All registered gateways: []"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Running REST API on: 9010"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Listening on 9012 for connections from Gateways"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Listening on 9011 for connections from Providers\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Listening on 9013 for connections from admin clients"}
{"level":"info","service":"gateway","time":"2021-03-16T02:35:33Z","message":"Filecoin Gateway Start-up Complete"}
Stopping provider ... done
Stopping gateway  ... done
Stopping register ... done
Stopping redis    ... done
Removing fc-retrieval-itest_itest_run_dff7a79d87b3 ... done
Removing provider                                  ... done
Removing gateway                                   ... done
Removing register                                  ... done
Removing redis                                     ... done
Network shared is external, skipping
Creating redis ... done
Creating register ... done
Creating gateway  ... done
Creating provider ... done
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
REDIS STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
1:C 16 Mar 2021 02:36:56.067 # oO0OoO0OoO0Oo Redis is starting oO0OoO0OoO0Oo
1:C 16 Mar 2021 02:36:56.067 # Redis version=6.2.1, bits=64, commit=00000000, modified=0, pid=1, just started
1:C 16 Mar 2021 02:36:56.067 # Warning: no config file specified, using the default config. In order to specify a config file use redis-server /path/to/redis.conf
1:M 16 Mar 2021 02:36:56.068 * monotonic clock: POSIX clock_gettime
1:M 16 Mar 2021 02:36:56.069 * Running mode=standalone, port=6379.
1:M 16 Mar 2021 02:36:56.069 # WARNING: The TCP backlog setting of 511 cannot be enforced because /proc/sys/net/core/somaxconn is set to the lower value of 128.
1:M 16 Mar 2021 02:36:56.069 # Server initialized
1:M 16 Mar 2021 02:36:56.070 * Ready to accept connections
REGISTER STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
2021/03/16 02:36:56 Serving register at http://[::]:9020
GATEWAY STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Container IP: 172.18.0.4
Starting service ...
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Filecoin Gateway Start-up: Started"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Settings: {BindRestAPI:9010 BindProviderAPI:9011 BindGatewayAPI:9012 BindAdminAPI:9013 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-gateway LogFile:gateway.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true GatewayID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F RegisterAPIURL:http://register:9020 GatewayAddress:f0121345 NetworkInfoGateway:172.18.0.4:9012 GatewayRegionCode:US GatewayRootSigningKey:0xABCDE123456789 GatewaySigningKey:0x987654321EDCBA NetworkInfoClient:172.18.0.4:9010 NetworkInfoProvider:172.18.0.4:9011 NetworkInfoAdmin:172.18.0.4:9013}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"All registered gateways: []"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Running REST API on: 9010"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Listening on 9012 for connections from Gateways"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Listening on 9011 for connections from Providers\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Listening on 9013 for connections from admin clients"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Filecoin Gateway Start-up Complete"}
PROVIDER STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Filecoin Provider Start-up: Started"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Settings: {BindRestAPI:9030 BindGatewayAPI:9032 BindAdminAPI:9033 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-provider LogFile:provider.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true ProviderID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F ProviderSigAlg:1 RegisterAPIURL:http://register:9020 ProviderAddress:f0121345 ProviderRootSigningKey:0xABCDE123456789 ProviderSigningKey:0x987654321EDCBA ProviderRegionCode:US NetworkInfoClient:127.0.0.1: NetworkInfoGateway:127.0.0.1: NetworkInfoAdmin:127.0.0.1:}"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Running REST API on: 9030"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Listening on 9032 for connections from Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Running Admin API on: 9033"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Update registered Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Filecoin Provider Start-up Complete"}
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Creating fc-retrieval-itest_itest_run ... done
go: downloading github.com/ConsenSys/fc-retrieval-common v0.0.0-20210312151557-4caead038a43
go: downloading github.com/spf13/viper v1.7.1
go: downloading github.com/ConsenSys/fc-retrieval-register v0.0.0-20210315215728-57ff758e2e2c
go: downloading github.com/stretchr/testify v1.7.0
go: downloading github.com/ConsenSys/fc-retrieval-client v0.0.0-20210315220115-b5a58266695e
go: downloading github.com/ConsenSys/fc-retrieval-gateway-admin v0.0.0-20210315220816-bbffc7dae1f2
go: downloading golang.org/x/crypto v0.0.0-20210220033148-5ea612d1eb83
go: downloading github.com/ipsn/go-secp256k1 v0.0.0-20180726113642-9d62b9f0bc52
go: downloading github.com/rs/zerolog v1.20.0
go: downloading gopkg.in/natefinch/lumberjack.v2 v2.0.0
go: downloading github.com/davidlazar/go-crypto v0.0.0-20200604182044-b73af7476f6c
go: downloading gopkg.in/yaml.v3 v3.0.0-20210107192922-496545a6307b
go: downloading github.com/fsnotify/fsnotify v1.4.9
go: downloading github.com/magiconair/properties v1.8.1
go: downloading github.com/hashicorp/hcl v1.0.0
go: downloading github.com/pelletier/go-toml v1.8.1
go: downloading github.com/spf13/afero v1.1.2
go: downloading golang.org/x/sys v0.0.0-20210301091718-77cc2087c03b
go: downloading gopkg.in/yaml.v2 v2.4.0
go: downloading github.com/davecgh/go-spew v1.1.1
go: downloading github.com/mitchellh/mapstructure v1.4.1
go: downloading github.com/cbergoon/merkletree v0.2.0
go: downloading github.com/spf13/pflag v1.0.5
go: downloading github.com/spf13/jwalterweatherman v1.0.0
go: downloading github.com/subosito/gotenv v1.2.0
go: downloading github.com/pmezard/go-difflib v1.0.0
go: downloading golang.org/x/text v0.3.5
go: downloading gopkg.in/ini.v1 v1.51.0
go: downloading github.com/spf13/cast v1.3.0
go: downloading github.com/tatsushid/go-fastping v0.0.0-20160109021039-d7bb493dee3e
go: downloading github.com/bitly/go-simplejson v0.5.0
go: downloading golang.org/x/net v0.0.0-20210226172049-e18ecbb05110
=== RUN   TestOneGateway
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:37:56Z","message":"Filecoin Retrieval Gateway Admin Client started"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:37:56Z","message":"Filecoin Retrieval Gateway Admin Client: RequestKeyCreation()"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:37:56Z","message":"Filecoin Retrieval Gateway Admin Client: RequestKeyCreation()"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:37:56Z","message":"Filecoin Retrieval Gateway Admin Client: InitializeGateway()"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:37:56Z","message":"Sending message to gateway: 9b8152c8dbd077833ae0c8ef519f5b133776661569d6f9a135cc2977503386c4, message:     0: 7b 22 6d 65  73 73 61 67  65 5f 74 79  70 65 22 3a  32 30 34 2c  22 70 72 6f  74 6f 63 6f  6c 5f 76 65   | {\"message_type\":204,\"protocol_ve\n   32: 72 73 69 6f  6e 22 3a 31  2c 22 70 72  6f 74 6f 63  6f 6c 5f 73  75 70 70 6f  72 74 65 64  22 3a 5b 31   | rsion\":1,\"protocol_supported\":[1\n   64: 2c 31 5d 2c  22 6d 65 73  73 61 67 65  5f 62 6f 64  79 22 3a 22  65 79 4a 75  62 32 52 6c  58 32 6c 6b   | ,1],\"message_body\":\"eyJub2RlX2lk\n   96: 49 6a 6f 69  62 54 52 47  55 33 6c 4f  64 6c 46 6b  4e 45 30 32  4e 45 31 71  64 6c 56 61  4f 57 4a 46   | IjoibTRGU3lOdlFkNE02NE1qdlVaOWJF\n  128: 65 6d 51 79  57 6d 68 57  63 44 46 32  62 57 68 4f  59 33 64 77  5a 44 46 42  65 6d 68 7a  55 54 30 69   | emQyWmhWcDF2bWhOY3dwZDFBemhzUT0i\n  160: 4c 43 4a 77  63 6d 6c 32  59 58 52 6c  61 32 56 35  49 6a 6f 69  4d 44 45 79  4e 7a 68 6d  4e 6a 49 33   | LCJwcml2YXRla2V5IjoiMDEyNzhmNjI3\n  192: 4e 32 55 35  4e 6d 46 6d  5a 57 4a 6c  4e 6a 49 7a  5a 44 45 35  4d 7a 55 77  59 54 52 6a  59 7a 63 7a   | N2U5NmFmZWJlNjIzZDE5MzUwYTRjYzcz\n  224: 4e 44 49 32  4e 32 5a 6c  5a 6d 52 6d  4d 6d 56 6b  4d 6d 4e 6b  4e 44 4e 6c  4d 6a 46 69  4f 47 59 33   | NDI2N2ZlZmRmMmVkMmNkNDNlMjFiOGY3\n  256: 5a 44 42 6c  59 57 51 35  4d 54 4e 6c  49 69 77 69  63 48 4a 70  64 6d 46 30  5a 57 74 6c  65 58 5a 6c   | ZDBlYWQ5MTNlIiwicHJpdmF0ZWtleXZl\n  288: 63 6e 4e 70  62 32 34 69  4f 6a 46 39  22 2c 22 6d  65 73 73 61  67 65 5f 73  69 67 6e 61  74 75 72 65   | cnNpb24iOjF9\",\"message_signature\n  320: 22 3a 22 30  30 30 30 30  30 30 31 64  35 66 64 31  36 64 65 66  32 31 32 36  62 37 37 62  31 34 36 63   | \":\"00000001d5fd16def2126b77b146c\n  352: 39 34 63 65  32 39 36 64  32 36 66 32  64 36 32 66  32 31 38 62  38 38 64 38  65 31 64 39  63 31 63 31   | 94ce296d26f2d62f218b88d8e1d9c1c1\n  384: 64 66 34 62  34 38 63 37  34 32 66 31  35 61 65 34  65 30 66 62  38 34 62 63  39 65 62 38  33 39 30 37   | df4b48c742f15ae4e0fb84bc9eb83907\n  416: 61 31 65 34  65 61 65 33  61 39 31 36  31 33 38 34  38 33 62 66  64 37 64 36  30 64 33 31  37 61 35 61   | a1e4eae3a916138483bfd7d60d317a5a\n  448: 36 34 30 33  38 30 63 36  64 64 33 30  30 22 7d                                         | 640380c6dd300\"}\n"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:37:56Z","message":"Get active connection, nodeID: 9b8152c8dbd077833ae0c8ef519f5b133776661569d6f9a135cc2977503386c4"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:37:56Z","message":"No active connection, connect to peer"}
{"level":"debug","service":"gateway-admin","time":"2021-03-16T02:37:56Z","message":"Got address: gateway:9013"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:37:56Z","message":"Response message: &{MessageType:205 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 101 120 105 115 116 115 34 58 116 114 117 101 125] Signature:0000000174ebda9d1155931f2824a4c311facaefa57c88a1108edf19a567301a1a18ba6566f253bfb9f41c6cec4ac5aa01839022dccc74213b7724fe614094c43c1abe1200}"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:37:56Z","message":"Adding to client config gateway: 9b8152c8dbd077833ae0c8ef519f5b133776661569d6f9a135cc2977503386c4"}
{"level":"info","service":"client","time":"2021-03-16T02:37:56Z","message":"Settings: No Client ID set. Generating random client ID"}
{"level":"info","service":"client","time":"2021-03-16T02:37:56Z","message":"Filecoin Retrieval Client started"}
{"level":"info","service":"client","time":"2021-03-16T02:37:56Z","message":"Add gateways to use"}
{"level":"info","service":"client","time":"2021-03-16T02:37:56Z","message":"Get gateways to use"}
{"level":"info","service":"client","time":"2021-03-16T02:37:56Z","message":"Add active gateways"}
{"level":"info","service":"client","time":"2021-03-16T02:37:56Z","message":"Client Manageer sending JSON: {\"message_type\":0,\"protocol_version\":1,\"protocol_supported\":[1,1],\"message_body\":\"eyJjbGllbnRfaWQiOiI0WWtrS0QvSE83aDlaeGxOY2w0cVN2S2U1MUVRR29LdUJEcWlSK3ROVzVFPSIsImNoYWxsZW5nZSI6IjBWbTFzbW01dk9mSitBdXdHd3VBYno5a2R5UVppYXVZZE9YSzBRb21pd0k9IiwidHRsIjoxNjE1ODYyMzc3fQ==\",\"message_signature\":\"\"} to url: gateway:9010"}
{"level":"info","service":"client","time":"2021-03-16T02:37:56Z","message":"Get active gateways"}
--- PASS: TestOneGateway (0.03s)
PASS
ok  	command-line-arguments	0.056s
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
PROVIDER LOGS Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Filecoin Provider Start-up: Started"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Settings: {BindRestAPI:9030 BindGatewayAPI:9032 BindAdminAPI:9033 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-provider LogFile:provider.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true ProviderID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F ProviderSigAlg:1 RegisterAPIURL:http://register:9020 ProviderAddress:f0121345 ProviderRootSigningKey:0xABCDE123456789 ProviderSigningKey:0x987654321EDCBA ProviderRegionCode:US NetworkInfoClient:127.0.0.1: NetworkInfoGateway:127.0.0.1: NetworkInfoAdmin:127.0.0.1:}"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Running REST API on: 9030"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Listening on 9032 for connections from Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Running Admin API on: 9033"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Update registered Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:36:57Z","message":"Filecoin Provider Start-up Complete"}
GATEWAY LOGS Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Container IP: 172.18.0.4
Starting service ...
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Filecoin Gateway Start-up: Started"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Settings: {BindRestAPI:9010 BindProviderAPI:9011 BindGatewayAPI:9012 BindAdminAPI:9013 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-gateway LogFile:gateway.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true GatewayID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F RegisterAPIURL:http://register:9020 GatewayAddress:f0121345 NetworkInfoGateway:172.18.0.4:9012 GatewayRegionCode:US GatewayRootSigningKey:0xABCDE123456789 GatewaySigningKey:0x987654321EDCBA NetworkInfoClient:172.18.0.4:9010 NetworkInfoProvider:172.18.0.4:9011 NetworkInfoAdmin:172.18.0.4:9013}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"All registered gateways: []"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Running REST API on: 9010"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Listening on 9012 for connections from Gateways"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Listening on 9011 for connections from Providers\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Listening on 9013 for connections from admin clients"}
{"level":"info","service":"gateway","time":"2021-03-16T02:36:57Z","message":"Filecoin Gateway Start-up Complete"}
{"level":"info","service":"gateway","time":"2021-03-16T02:37:56Z","message":"Incoming connection from admin client at :172.18.0.6:35870"}
{"level":"info","service":"gateway","time":"2021-03-16T02:37:56Z","message":"In handleAdminAcceptKeysChallenge"}
{"level":"info","service":"gateway","time":"2021-03-16T02:37:56Z","message":"Message received \n    0: 7b 22 6d 65  73 73 61 67  65 5f 74 79  70 65 22 3a  32 30 34 2c  22 70 72 6f  74 6f 63 6f  6c 5f 76 65   | {\"message_type\":204,\"protocol_ve\n   32: 72 73 69 6f  6e 22 3a 31  2c 22 70 72  6f 74 6f 63  6f 6c 5f 73  75 70 70 6f  72 74 65 64  22 3a 5b 31   | rsion\":1,\"protocol_supported\":[1\n   64: 2c 31 5d 2c  22 6d 65 73  73 61 67 65  5f 62 6f 64  79 22 3a 22  65 79 4a 75  62 32 52 6c  58 32 6c 6b   | ,1],\"message_body\":\"eyJub2RlX2lk\n   96: 49 6a 6f 69  62 54 52 47  55 33 6c 4f  64 6c 46 6b  4e 45 30 32  4e 45 31 71  64 6c 56 61  4f 57 4a 46   | IjoibTRGU3lOdlFkNE02NE1qdlVaOWJF\n  128: 65 6d 51 79  57 6d 68 57  63 44 46 32  62 57 68 4f  59 33 64 77  5a 44 46 42  65 6d 68 7a  55 54 30 69   | emQyWmhWcDF2bWhOY3dwZDFBemhzUT0i\n  160: 4c 43 4a 77  63 6d 6c 32  59 58 52 6c  61 32 56 35  49 6a 6f 69  4d 44 45 79  4e 7a 68 6d  4e 6a 49 33   | LCJwcml2YXRla2V5IjoiMDEyNzhmNjI3\n  192: 4e 32 55 35  4e 6d 46 6d  5a 57 4a 6c  4e 6a 49 7a  5a 44 45 35  4d 7a 55 77  59 54 52 6a  59 7a 63 7a   | N2U5NmFmZWJlNjIzZDE5MzUwYTRjYzcz\n  224: 4e 44 49 32  4e 32 5a 6c  5a 6d 52 6d  4d 6d 56 6b  4d 6d 4e 6b  4e 44 4e 6c  4d 6a 46 69  4f 47 59 33   | NDI2N2ZlZmRmMmVkMmNkNDNlMjFiOGY3\n  256: 5a 44 42 6c  59 57 51 35  4d 54 4e 6c  49 69 77 69  63 48 4a 70  64 6d 46 30  5a 57 74 6c  65 58 5a 6c   | ZDBlYWQ5MTNlIiwicHJpdmF0ZWtleXZl\n  288: 63 6e 4e 70  62 32 34 69  4f 6a 46 39  22 2c 22 6d  65 73 73 61  67 65 5f 73  69 67 6e 61  74 75 72 65   | cnNpb24iOjF9\",\"message_signature\n  320: 22 3a 22 30  30 30 30 30  30 30 31 64  35 66 64 31  36 64 65 66  32 31 32 36  62 37 37 62  31 34 36 63   | \":\"00000001d5fd16def2126b77b146c\n  352: 39 34 63 65  32 39 36 64  32 36 66 32  64 36 32 66  32 31 38 62  38 38 64 38  65 31 64 39  63 31 63 31   | 94ce296d26f2d62f218b88d8e1d9c1c1\n  384: 64 66 34 62  34 38 63 37  34 32 66 31  35 61 65 34  65 30 66 62  38 34 62 63  39 65 62 38  33 39 30 37   | df4b48c742f15ae4e0fb84bc9eb83907\n  416: 61 31 65 34  65 61 65 33  61 39 31 36  31 33 38 34  38 33 62 66  64 37 64 36  30 64 33 31  37 61 35 61   | a1e4eae3a916138483bfd7d60d317a5a\n  448: 36 34 30 33  38 30 63 36  64 64 33 30  30 22 7d                                         | 640380c6dd300\"}\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:37:56Z","message":"Admin action: Key installation complete"}
16/Mar/2021:02:37:56 +0000 200 609μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
{"level":"error","service":"gateway","time":"2021-03-16T02:37:56Z","message":"Error: EOF"}
Stopping provider ... done
Stopping gateway  ... done
Stopping register ... done
Stopping redis    ... done
Removing fc-retrieval-itest_itest_run_6dfe03825da5 ... done
Removing provider                                  ... done
Removing gateway                                   ... done
Removing register                                  ... done
Removing redis                                     ... done
Network shared is external, skipping
Creating redis ... done
Creating register ... done
Creating gateway  ... done
Creating provider ... done
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
REDIS STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
1:C 16 Mar 2021 02:38:10.122 # oO0OoO0OoO0Oo Redis is starting oO0OoO0OoO0Oo
1:C 16 Mar 2021 02:38:10.122 # Redis version=6.2.1, bits=64, commit=00000000, modified=0, pid=1, just started
1:C 16 Mar 2021 02:38:10.122 # Warning: no config file specified, using the default config. In order to specify a config file use redis-server /path/to/redis.conf
1:M 16 Mar 2021 02:38:10.123 * monotonic clock: POSIX clock_gettime
1:M 16 Mar 2021 02:38:10.123 * Running mode=standalone, port=6379.
1:M 16 Mar 2021 02:38:10.123 # WARNING: The TCP backlog setting of 511 cannot be enforced because /proc/sys/net/core/somaxconn is set to the lower value of 128.
1:M 16 Mar 2021 02:38:10.123 # Server initialized
1:M 16 Mar 2021 02:38:10.124 * Ready to accept connections
REGISTER STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
2021/03/16 02:38:10 Serving register at http://[::]:9020
GATEWAY STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Container IP: 172.18.0.4
Starting service ...
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Filecoin Gateway Start-up: Started"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Settings: {BindRestAPI:9010 BindProviderAPI:9011 BindGatewayAPI:9012 BindAdminAPI:9013 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-gateway LogFile:gateway.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true GatewayID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F RegisterAPIURL:http://register:9020 GatewayAddress:f0121345 NetworkInfoGateway:172.18.0.4:9012 GatewayRegionCode:US GatewayRootSigningKey:0xABCDE123456789 GatewaySigningKey:0x987654321EDCBA NetworkInfoClient:172.18.0.4:9010 NetworkInfoProvider:172.18.0.4:9011 NetworkInfoAdmin:172.18.0.4:9013}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"All registered gateways: []"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Running REST API on: 9010"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Listening on 9012 for connections from Gateways"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Listening on 9011 for connections from Providers\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Listening on 9013 for connections from admin clients"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Filecoin Gateway Start-up Complete"}
PROVIDER STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Filecoin Provider Start-up: Started"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Settings: {BindRestAPI:9030 BindGatewayAPI:9032 BindAdminAPI:9033 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-provider LogFile:provider.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true ProviderID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F ProviderSigAlg:1 RegisterAPIURL:http://register:9020 ProviderAddress:f0121345 ProviderRootSigningKey:0xABCDE123456789 ProviderSigningKey:0x987654321EDCBA ProviderRegionCode:US NetworkInfoClient:127.0.0.1: NetworkInfoGateway:127.0.0.1: NetworkInfoAdmin:127.0.0.1:}"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Running REST API on: 9030"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Listening on 9032 for connections from Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Running Admin API on: 9033"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Update registered Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Filecoin Provider Start-up Complete"}
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Creating fc-retrieval-itest_itest_run ... done
go: downloading github.com/ConsenSys/fc-retrieval-register v0.0.0-20210315215728-57ff758e2e2c
go: downloading github.com/stretchr/testify v1.7.0
go: downloading github.com/ConsenSys/fc-retrieval-provider-admin v0.0.0-20210315220609-1fe0ee54f441
go: downloading github.com/ConsenSys/fc-retrieval-gateway-admin v0.0.0-20210315220816-bbffc7dae1f2
go: downloading github.com/ConsenSys/fc-retrieval-common v0.0.0-20210312151557-4caead038a43
go: downloading github.com/ConsenSys/fc-retrieval-client v0.0.0-20210315220115-b5a58266695e
go: downloading github.com/spf13/viper v1.7.1
go: downloading github.com/davecgh/go-spew v1.1.1
go: downloading github.com/pmezard/go-difflib v1.0.0
go: downloading gopkg.in/yaml.v3 v3.0.0-20210107192922-496545a6307b
go: downloading github.com/tatsushid/go-fastping v0.0.0-20160109021039-d7bb493dee3e
go: downloading github.com/rs/zerolog v1.20.0
go: downloading github.com/cbergoon/merkletree v0.2.0
go: downloading golang.org/x/crypto v0.0.0-20210220033148-5ea612d1eb83
go: downloading github.com/spf13/pflag v1.0.5
go: downloading github.com/mitchellh/mapstructure v1.4.1
go: downloading github.com/fsnotify/fsnotify v1.4.9
go: downloading github.com/hashicorp/hcl v1.0.0
go: downloading gopkg.in/yaml.v2 v2.4.0
go: downloading github.com/magiconair/properties v1.8.1
go: downloading golang.org/x/net v0.0.0-20210226172049-e18ecbb05110
go: downloading github.com/davidlazar/go-crypto v0.0.0-20200604182044-b73af7476f6c
go: downloading github.com/spf13/cast v1.3.0
go: downloading github.com/pelletier/go-toml v1.8.1
go: downloading gopkg.in/ini.v1 v1.51.0
go: downloading github.com/spf13/afero v1.1.2
go: downloading golang.org/x/sys v0.0.0-20210301091718-77cc2087c03b
go: downloading github.com/bitly/go-simplejson v0.5.0
go: downloading github.com/subosito/gotenv v1.2.0
go: downloading github.com/ipsn/go-secp256k1 v0.0.0-20180726113642-9d62b9f0bc52
go: downloading gopkg.in/natefinch/lumberjack.v2 v2.0.0
go: downloading github.com/spf13/jwalterweatherman v1.0.0
go: downloading golang.org/x/text v0.3.5
=== RUN   TestInitialiseGateway
{"level":"info","time":"2021-03-16T02:39:21Z","message":"/*******************************************************/"}
{"level":"info","time":"2021-03-16T02:39:21Z","message":"/*             Start TestInitialiseGateway\t         */"}
{"level":"info","time":"2021-03-16T02:39:21Z","message":"/*******************************************************/"}
{"level":"error","time":"2021-03-16T02:39:21Z","message":"Wait two seconds for the gateway to deploy and be ready for requests"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:23Z","message":"Filecoin Retrieval Gateway Admin Client started"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:23Z","message":"Filecoin Retrieval Gateway Admin Client: RequestKeyCreation()"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:23Z","message":"Filecoin Retrieval Gateway Admin Client: RequestKeyCreation()"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:23Z","message":"Filecoin Retrieval Gateway Admin Client: InitializeGateway()"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:23Z","message":"Sending message to gateway: a2be680de11fff612a583258754a4a9f0cea86f5488613717dd9f692bf6d8d68, message:     0: 7b 22 6d 65  73 73 61 67  65 5f 74 79  70 65 22 3a  32 30 34 2c  22 70 72 6f  74 6f 63 6f  6c 5f 76 65   | {\"message_type\":204,\"protocol_ve\n   32: 72 73 69 6f  6e 22 3a 31  2c 22 70 72  6f 74 6f 63  6f 6c 5f 73  75 70 70 6f  72 74 65 64  22 3a 5b 31   | rsion\":1,\"protocol_supported\":[1\n   64: 2c 31 5d 2c  22 6d 65 73  73 61 67 65  5f 62 6f 64  79 22 3a 22  65 79 4a 75  62 32 52 6c  58 32 6c 6b   | ,1],\"message_body\":\"eyJub2RlX2lk\n   96: 49 6a 6f 69  62 33 49 31  62 30 52 6c  52 57 59 76  4d 6b 56 78  56 30 52 4b  57 57 52 56  63 45 74 75   | Ijoib3I1b0RlRWYvMkVxV0RKWWRVcEtu\n  128: 64 33 70 78  61 48 5a 57  53 57 68 6f  54 6e 68 6d  5a 47 34 79  61 33 49 35  64 47 70 58  5a 7a 30 69   | d3pxaHZWSWhoTnhmZG4ya3I5dGpXZz0i\n  160: 4c 43 4a 77  63 6d 6c 32  59 58 52 6c  61 32 56 35  49 6a 6f 69  4d 44 46 6b  4e 7a 55 79  4d 32 45 31   | LCJwcml2YXRla2V5IjoiMDFkNzUyM2E1\n  192: 4d 57 4d 7a  5a 44 49 78  4f 57 4a 6c  59 7a 46 6c  4d 47 4a 69  5a 44 68 6d  4f 47 46 6c  4e 44 45 34   | MWMzZDIxOWJlYzFlMGJiZDhmOGFlNDE4\n  224: 4d 44 52 6b  4e 6a 56 68  59 7a 45 32  4e 54 52 68  4e 7a 5a 6b  4e 54 59 33  4e 7a 59 33  5a 57 49 35   | MDRkNjVhYzE2NTRhNzZkNTY3NzY3ZWI5\n  256: 4f 57 4d 30  4f 47 55 77  59 6a 63 7a  49 69 77 69  63 48 4a 70  64 6d 46 30  5a 57 74 6c  65 58 5a 6c   | OWM0OGUwYjczIiwicHJpdmF0ZWtleXZl\n  288: 63 6e 4e 70  62 32 34 69  4f 6a 46 39  22 2c 22 6d  65 73 73 61  67 65 5f 73  69 67 6e 61  74 75 72 65   | cnNpb24iOjF9\",\"message_signature\n  320: 22 3a 22 30  30 30 30 30  30 30 31 65  38 33 63 39  33 30 66 63  64 30 65 64  39 66 65 31  32 37 34 63   | \":\"00000001e83c930fcd0ed9fe1274c\n  352: 64 32 63 33  36 32 35 61  65 35 38 38  64 33 39 66  34 62 32 66  62 37 63 35  64 63 62 65  36 31 38 38   | d2c3625ae588d39f4b2fb7c5dcbe6188\n  384: 61 32 33 31  33 35 33 38  34 34 36 31  61 32 30 31  38 34 31 65  37 32 39 38  30 62 66 38  61 63 33 39   | a23135384461a201841e72980bf8ac39\n  416: 30 62 35 39  63 62 66 35  39 31 63 64  65 34 66 34  66 64 62 37  61 39 63 35  39 30 33 64  39 30 30 64   | 0b59cbf591cde4f4fdb7a9c5903d900d\n  448: 63 33 32 30  31 34 66 61  61 31 34 30  31 22 7d                                         | c32014faa1401\"}\n"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:23Z","message":"Get active connection, nodeID: a2be680de11fff612a583258754a4a9f0cea86f5488613717dd9f692bf6d8d68"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:23Z","message":"No active connection, connect to peer"}
{"level":"debug","service":"gateway-admin","time":"2021-03-16T02:39:23Z","message":"Got address: gateway:9013"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:23Z","message":"Response message: &{MessageType:205 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 101 120 105 115 116 115 34 58 116 114 117 101 125] Signature:000000013f3e233482a0a5dde68f973d6de514ab54a36a35e7fc88f3f512a4bfde8ca0a615861e5f637f846be6d27c8283f77020c2a8d58480243edb2264eca4a08b492601}"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:23Z","message":"Wait five seconds for the gateway to initialise"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:28Z","message":"/*******************************************************/"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:28Z","message":"/*               End TestInitialiseGateway\t         */"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:28Z","message":"/*******************************************************/"}
--- PASS: TestInitialiseGateway (7.02s)
=== RUN   TestInitialiseProvider
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:28Z","message":"/*******************************************************/"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:28Z","message":"/*             Start TestInitialiseProvider\t         */"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:39:28Z","message":"/*******************************************************/"}
{"level":"error","service":"gateway-admin","time":"2021-03-16T02:39:28Z","message":"Wait two seconds for the provider to deploy and be ready for requests"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:30Z","message":"Sending JSON to url: http://provider:9033/v1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:30Z","message":"Wait ten seconds for the provider to initialise"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:40Z","message":"/*******************************************************/"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:40Z","message":"/*              End TestInitialiseProvider\t         */"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:40Z","message":"/*******************************************************/"}
--- PASS: TestInitialiseProvider (12.02s)
=== RUN   TestPublishGroupCID
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:40Z","message":"/*******************************************************/"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:40Z","message":"/*      Start TestProviderPublishGroupCIDOffer\t     */"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:40Z","message":"/*******************************************************/"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:40Z","message":"Provider Manager sending message to providerID: ca72c59b0821c13a60beb67e4645b66582ba74a220f49870722d9ee63b2a73b6"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:40Z","message":"Sending JSON to url: http://provider:9033/v1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:40Z","message":"Wait 10 seconds"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"Get all offers"}
EncodeProviderAdminGetGroupCIDRequest
Body: [123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 93 125]
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"Provider Manager sending message to providerID: ca72c59b0821c13a60beb67e4645b66582ba74a220f49870722d9ee63b2a73b6"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"Sending JSON to url: http://provider:9033/v1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"Get offers by gatewayID=a2be680de11fff612a583258754a4a9f0cea86f5488613717dd9f692bf6d8d68"}
EncodeProviderAdminGetGroupCIDRequest
Body: [123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 34 111 114 53 111 68 101 69 102 47 50 69 113 87 68 74 89 100 85 112 75 110 119 122 113 104 118 86 73 104 104 78 120 102 100 110 50 107 114 57 116 106 87 103 61 34 93 125]
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"Provider Manager sending message to providerID: ca72c59b0821c13a60beb67e4645b66582ba74a220f49870722d9ee63b2a73b6"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"Sending JSON to url: http://provider:9033/v1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"Get offers by gatewayID=101112131415161718191a1b1c1d1e1f202122232425262728292a2b2c2dfa43"}
EncodeProviderAdminGetGroupCIDRequest
Body: [123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 34 69 66 69 83 69 120 81 86 70 104 99 89 71 82 111 98 72 66 48 101 72 121 65 104 73 105 77 107 74 83 89 110 75 67 107 113 75 121 119 116 43 107 77 61 34 93 125]
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"Provider Manager sending message to providerID: ca72c59b0821c13a60beb67e4645b66582ba74a220f49870722d9ee63b2a73b6"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"Sending JSON to url: http://provider:9033/v1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"/*       End TestProviderPublishGroupCIDOffer\t         */"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
--- PASS: TestPublishGroupCID (10.03s)
=== RUN   TestInitClient
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"/*                Start TestInitClient        \t     */"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Settings: No Client ID set. Generating random client ID"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Filecoin Retrieval Client started"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*                 End TestInitClient      \t         */"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
--- PASS: TestInitClient (0.00s)
=== RUN   TestClientAddGateway
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*             Start TestClientAddGateway     \t     */"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Add gateways to use"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Add active gateways"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Client Manageer sending JSON: {\"message_type\":0,\"protocol_version\":1,\"protocol_supported\":[1,1],\"message_body\":\"eyJjbGllbnRfaWQiOiJraE9DVWpCMVd2ejRlbE5pcERFYjJQdkV0WWg5cFd5SWdzZFV6VExkdkhZPSIsImNoYWxsZW5nZSI6Im1WRWFHbVJCdGhndGYwbTZmRlNPRWFyWjB5cEJGSWt4dVZHaVZSN1AzSzA9IiwidHRsIjoxNjE1ODYyNDkxfQ==\",\"message_signature\":\"\"} to url: gateway:9010"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*              End TestClientAddGateway      \t     */"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
--- PASS: TestClientAddGateway (0.02s)
=== RUN   TestClientStdContentDiscover
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*        Start TestClientStdContentDiscover     \t     */"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Find offers std discovery"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Client Manageer sending JSON: {\"message_type\":2,\"protocol_version\":1,\"protocol_supported\":[1,1],\"message_body\":\"eyJwaWVjZV9jaWQiOiIrdjZrV2x5ako2YndKb01xeVV4cmpZTlZIZGgvM3BUNkhKTXl6cGtqZUpNPSIsIm5vbmNlIjoxOTc2MjM1NDEwODg0NDkxNTc0LCJ0dGwiOjE2MTU4NjI0OTF9\",\"message_signature\":\"\"} to url: gateway:9010"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Offer pass every verification, added to result"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Total received offer: 1, total verified offer: 1"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Find offers std discovery"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Client Manageer sending JSON: {\"message_type\":2,\"protocol_version\":1,\"protocol_supported\":[1,1],\"message_body\":\"eyJwaWVjZV9jaWQiOiIyTkZEVDI5eXJqWkJ3ZnFqUlUrUDNoRTA3ME53UTNuN1pHTzJYbHFMY3Q4PSIsIm5vbmNlIjozNTEwOTQyODc1NDE0NDU4ODM2LCJ0dGwiOjE2MTU4NjI0OTF9\",\"message_signature\":\"\"} to url: gateway:9010"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Offer pass every verification, added to result"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Total received offer: 1, total verified offer: 1"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Find offers std discovery"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Client Manageer sending JSON: {\"message_type\":2,\"protocol_version\":1,\"protocol_supported\":[1,1],\"message_body\":\"eyJwaWVjZV9jaWQiOiJ1S05HbGl1VE1GSFpZU3grU3hUS3M4Y2hhWWwzT0x4ZDZ0QkI1b1VDTW1BPSIsIm5vbmNlIjoyOTMzNTY4ODcxMjExNDQ1NTE1LCJ0dGwiOjE2MTU4NjI0OTF9\",\"message_signature\":\"\"} to url: gateway:9010"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Offer pass every verification, added to result"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Total received offer: 1, total verified offer: 1"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Find offers std discovery"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Client Manageer sending JSON: {\"message_type\":2,\"protocol_version\":1,\"protocol_supported\":[1,1],\"message_body\":\"eyJwaWVjZV9jaWQiOiJLbGJMd0gzZTJrNmR2VVhPRENQSmYxWmliZzQ0VDNTVVZvUTNGa3NLd29nPSIsIm5vbmNlIjo0MzI0NzQ1NDgzODM4MTgyODczLCJ0dGwiOjE2MTU4NjI0OTF9\",\"message_signature\":\"\"} to url: gateway:9010"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"Total received offer: 0, total verified offer: 0"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*        End TestClientStdContentDiscover     \t     */"}
{"level":"info","service":"client","time":"2021-03-16T02:39:50Z","message":"/*******************************************************/"}
--- PASS: TestClientStdContentDiscover (0.04s)
PASS
ok  	command-line-arguments	29.151s
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
PROVIDER LOGS Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Filecoin Provider Start-up: Started"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Settings: {BindRestAPI:9030 BindGatewayAPI:9032 BindAdminAPI:9033 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-provider LogFile:provider.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true ProviderID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F ProviderSigAlg:1 RegisterAPIURL:http://register:9020 ProviderAddress:f0121345 ProviderRootSigningKey:0xABCDE123456789 ProviderSigningKey:0x987654321EDCBA ProviderRegionCode:US NetworkInfoClient:127.0.0.1: NetworkInfoGateway:127.0.0.1: NetworkInfoAdmin:127.0.0.1:}"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Running REST API on: 9030"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Listening on 9032 for connections from Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Running Admin API on: 9033"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Update registered Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:38:11Z","message":"Filecoin Provider Start-up Complete"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:26Z","message":"Add to registered gateways map: nodeID=a2be680de11fff612a583258754a4a9f0cea86f5488613717dd9f692bf6d8d68"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:30Z","message":"handle key management."}
{"level":"info","service":"provider","time":"2021-03-16T02:39:30Z","message":"Check if c is nil :false"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:30Z","message":"Setting node id"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:30Z","message":"Signing response."}
16/Mar/2021:02:39:30 +0000 200 986μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
{"level":"info","service":"provider","time":"2021-03-16T02:39:40Z","message":"handleProviderPublishGroupCID: &{MessageType:302 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 99 105 100 115 34 58 91 34 43 118 54 107 87 108 121 106 74 54 98 119 74 111 77 113 121 85 120 114 106 89 78 86 72 100 104 47 51 112 84 54 72 74 77 121 122 112 107 106 101 74 77 61 34 44 34 50 78 70 68 84 50 57 121 114 106 90 66 119 102 113 106 82 85 43 80 51 104 69 48 55 48 78 119 81 51 110 55 90 71 79 50 88 108 113 76 99 116 56 61 34 44 34 117 75 78 71 108 105 117 84 77 70 72 90 89 83 120 43 83 120 84 75 115 56 99 104 97 89 108 51 79 76 120 100 54 116 66 66 53 111 85 67 77 109 65 61 34 93 44 34 112 114 105 99 101 34 58 52 50 44 34 101 120 112 105 114 121 34 58 49 54 49 53 57 52 56 55 56 48 44 34 113 111 115 34 58 52 50 125] Signature:0000000107d91b9d1b9f16b7788b4edd072b0619785c06baefc1e1e887d7a1e2a14e7b843a31d5dce69d66d9230104189be573dccfc247ecc0347b6b147497b0c09bbcb001}"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:40Z","message":"Get active connection, nodeID: a2be680de11fff612a583258754a4a9f0cea86f5488613717dd9f692bf6d8d68"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:40Z","message":"No active connection, connect to peer"}
{"level":"debug","service":"provider","time":"2021-03-16T02:39:40Z","message":"Got address: gateway:9011"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:40Z","message":"Got reponse from gateway=a2be680de11fff612a583258754a4a9f0cea86f5488613717dd9f692bf6d8d68: &{MessageType:302 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 112 114 111 118 105 100 101 114 95 105 100 34 58 34 111 114 53 111 68 101 69 102 47 50 69 113 87 68 74 89 100 85 112 75 110 119 122 113 104 118 86 73 104 104 78 120 102 100 110 50 107 114 57 116 106 87 103 61 34 44 34 100 105 103 101 115 116 34 58 91 51 53 44 49 52 52 44 49 56 52 44 50 53 52 44 49 48 57 44 55 56 44 49 50 44 50 44 49 56 49 44 49 56 50 44 49 49 52 44 50 48 57 44 49 54 54 44 49 48 51 44 50 52 44 50 50 49 44 50 53 52 44 51 53 44 49 48 48 44 49 52 57 44 49 51 50 44 56 49 44 49 57 52 44 49 49 49 44 51 51 44 50 52 56 44 51 49 44 49 52 53 44 49 51 48 44 49 54 55 44 49 51 54 44 49 53 51 93 125] Signature:000000013f3e233482a0a5dde68f973d6de514ab54a36a35e7fc88f3f512a4bfde8ca0a615861e5f637f846be6d27c8283f77020c2a8d58480243edb2264eca4a08b492601}"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:40Z","message":"Received digest: [35 144 184 254 109 78 12 2 181 182 114 209 166 103 24 221 254 35 100 149 132 81 194 111 33 248 31 145 130 167 136 153]"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:40Z","message":"Digest is OK! Add offer to storage"}
16/Mar/2021:02:39:40 +0000 200 9836μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
{"level":"info","service":"provider","time":"2021-03-16T02:39:50Z","message":"handleProviderGetGroupCID: &{MessageType:300 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 93 125] Signature:0000000107d91b9d1b9f16b7788b4edd072b0619785c06baefc1e1e887d7a1e2a14e7b843a31d5dce69d66d9230104189be573dccfc247ecc0347b6b147497b0c09bbcb001}"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:50Z","message":"Find offers: gatewayIDs=[]"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:50Z","message":"Found offers: 1"}
16/Mar/2021:02:39:50 +0000 200 1187μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
{"level":"info","service":"provider","time":"2021-03-16T02:39:50Z","message":"handleProviderGetGroupCID: &{MessageType:300 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 34 111 114 53 111 68 101 69 102 47 50 69 113 87 68 74 89 100 85 112 75 110 119 122 113 104 118 86 73 104 104 78 120 102 100 110 50 107 114 57 116 106 87 103 61 34 93 125] Signature:0000000107d91b9d1b9f16b7788b4edd072b0619785c06baefc1e1e887d7a1e2a14e7b843a31d5dce69d66d9230104189be573dccfc247ecc0347b6b147497b0c09bbcb001}"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:50Z","message":"Find offers: gatewayIDs=[{id:[162 190 104 13 225 31 255 97 42 88 50 88 117 74 74 159 12 234 134 245 72 134 19 113 125 217 246 146 191 109 141 104]}]"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:50Z","message":"Found offers: 1"}
16/Mar/2021:02:39:50 +0000 200 395μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
{"level":"info","service":"provider","time":"2021-03-16T02:39:50Z","message":"handleProviderGetGroupCID: &{MessageType:300 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 34 69 66 69 83 69 120 81 86 70 104 99 89 71 82 111 98 72 66 48 101 72 121 65 104 73 105 77 107 74 83 89 110 75 67 107 113 75 121 119 116 43 107 77 61 34 93 125] Signature:0000000107d91b9d1b9f16b7788b4edd072b0619785c06baefc1e1e887d7a1e2a14e7b843a31d5dce69d66d9230104189be573dccfc247ecc0347b6b147497b0c09bbcb001}"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:50Z","message":"Find offers: gatewayIDs=[{id:[16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 250 67]}]"}
{"level":"info","service":"provider","time":"2021-03-16T02:39:50Z","message":"Found offers: 0"}
16/Mar/2021:02:39:50 +0000 200 565μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
GATEWAY LOGS Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Container IP: 172.18.0.4
Starting service ...
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Filecoin Gateway Start-up: Started"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Settings: {BindRestAPI:9010 BindProviderAPI:9011 BindGatewayAPI:9012 BindAdminAPI:9013 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-gateway LogFile:gateway.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true GatewayID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F RegisterAPIURL:http://register:9020 GatewayAddress:f0121345 NetworkInfoGateway:172.18.0.4:9012 GatewayRegionCode:US GatewayRootSigningKey:0xABCDE123456789 GatewaySigningKey:0x987654321EDCBA NetworkInfoClient:172.18.0.4:9010 NetworkInfoProvider:172.18.0.4:9011 NetworkInfoAdmin:172.18.0.4:9013}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"All registered gateways: []"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Running REST API on: 9010"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Listening on 9012 for connections from Gateways"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Listening on 9011 for connections from Providers\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Listening on 9013 for connections from admin clients"}
{"level":"info","service":"gateway","time":"2021-03-16T02:38:11Z","message":"Filecoin Gateway Start-up Complete"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:23Z","message":"Incoming connection from admin client at :172.18.0.6:36002"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:23Z","message":"In handleAdminAcceptKeysChallenge"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:23Z","message":"Message received \n    0: 7b 22 6d 65  73 73 61 67  65 5f 74 79  70 65 22 3a  32 30 34 2c  22 70 72 6f  74 6f 63 6f  6c 5f 76 65   | {\"message_type\":204,\"protocol_ve\n   32: 72 73 69 6f  6e 22 3a 31  2c 22 70 72  6f 74 6f 63  6f 6c 5f 73  75 70 70 6f  72 74 65 64  22 3a 5b 31   | rsion\":1,\"protocol_supported\":[1\n   64: 2c 31 5d 2c  22 6d 65 73  73 61 67 65  5f 62 6f 64  79 22 3a 22  65 79 4a 75  62 32 52 6c  58 32 6c 6b   | ,1],\"message_body\":\"eyJub2RlX2lk\n   96: 49 6a 6f 69  62 33 49 31  62 30 52 6c  52 57 59 76  4d 6b 56 78  56 30 52 4b  57 57 52 56  63 45 74 75   | Ijoib3I1b0RlRWYvMkVxV0RKWWRVcEtu\n  128: 64 33 70 78  61 48 5a 57  53 57 68 6f  54 6e 68 6d  5a 47 34 79  61 33 49 35  64 47 70 58  5a 7a 30 69   | d3pxaHZWSWhoTnhmZG4ya3I5dGpXZz0i\n  160: 4c 43 4a 77  63 6d 6c 32  59 58 52 6c  61 32 56 35  49 6a 6f 69  4d 44 46 6b  4e 7a 55 79  4d 32 45 31   | LCJwcml2YXRla2V5IjoiMDFkNzUyM2E1\n  192: 4d 57 4d 7a  5a 44 49 78  4f 57 4a 6c  59 7a 46 6c  4d 47 4a 69  5a 44 68 6d  4f 47 46 6c  4e 44 45 34   | MWMzZDIxOWJlYzFlMGJiZDhmOGFlNDE4\n  224: 4d 44 52 6b  4e 6a 56 68  59 7a 45 32  4e 54 52 68  4e 7a 5a 6b  4e 54 59 33  4e 7a 59 33  5a 57 49 35   | MDRkNjVhYzE2NTRhNzZkNTY3NzY3ZWI5\n  256: 4f 57 4d 30  4f 47 55 77  59 6a 63 7a  49 69 77 69  63 48 4a 70  64 6d 46 30  5a 57 74 6c  65 58 5a 6c   | OWM0OGUwYjczIiwicHJpdmF0ZWtleXZl\n  288: 63 6e 4e 70  62 32 34 69  4f 6a 46 39  22 2c 22 6d  65 73 73 61  67 65 5f 73  69 67 6e 61  74 75 72 65   | cnNpb24iOjF9\",\"message_signature\n  320: 22 3a 22 30  30 30 30 30  30 30 31 65  38 33 63 39  33 30 66 63  64 30 65 64  39 66 65 31  32 37 34 63   | \":\"00000001e83c930fcd0ed9fe1274c\n  352: 64 32 63 33  36 32 35 61  65 35 38 38  64 33 39 66  34 62 32 66  62 37 63 35  64 63 62 65  36 31 38 38   | d2c3625ae588d39f4b2fb7c5dcbe6188\n  384: 61 32 33 31  33 35 33 38  34 34 36 31  61 32 30 31  38 34 31 65  37 32 39 38  30 62 66 38  61 63 33 39   | a23135384461a201841e72980bf8ac39\n  416: 30 62 35 39  63 62 66 35  39 31 63 64  65 34 66 34  66 64 62 37  61 39 63 35  39 30 33 64  39 30 30 64   | 0b59cbf591cde4f4fdb7a9c5903d900d\n  448: 63 33 32 30  31 34 66 61  61 31 34 30  31 22 7d                                         | c32014faa1401\"}\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:23Z","message":"Admin action: Key installation complete"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:31Z","message":"Add to registered providers map: nodeID=ca72c59b0821c13a60beb67e4645b66582ba74a220f49870722d9ee63b2a73b6"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:40Z","message":"Incoming connection from provider at :172.18.0.5:51470\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:40Z","message":"Message received: &{MessageType:8 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 110 111 110 99 101 34 58 49 44 34 112 114 111 118 105 100 101 114 95 105 100 34 58 34 121 110 76 70 109 119 103 104 119 84 112 103 118 114 90 43 82 107 87 50 90 89 75 54 100 75 73 103 57 74 104 119 99 105 50 101 53 106 115 113 99 55 89 61 34 44 34 112 114 105 99 101 95 112 101 114 95 98 121 116 101 34 58 52 50 44 34 101 120 112 105 114 121 95 100 97 116 101 34 58 49 54 49 53 57 52 56 55 56 48 44 34 113 111 115 34 58 52 50 44 34 112 105 101 99 101 95 99 105 100 115 34 58 91 34 43 118 54 107 87 108 121 106 74 54 98 119 74 111 77 113 121 85 120 114 106 89 78 86 72 100 104 47 51 112 84 54 72 74 77 121 122 112 107 106 101 74 77 61 34 44 34 50 78 70 68 84 50 57 121 114 106 90 66 119 102 113 106 82 85 43 80 51 104 69 48 55 48 78 119 81 51 110 55 90 71 79 50 88 108 113 76 99 116 56 61 34 44 34 117 75 78 71 108 105 117 84 77 70 72 90 89 83 120 43 83 120 84 75 115 56 99 104 97 89 108 51 79 76 120 100 54 116 66 66 53 111 85 67 77 109 65 61 34 93 44 34 115 105 103 110 97 116 117 114 101 34 58 34 48 48 48 48 48 48 48 49 54 48 51 55 100 98 99 48 56 57 55 99 50 101 48 98 52 54 53 53 56 55 53 51 54 49 102 50 56 52 53 55 56 102 51 102 50 97 97 57 49 99 99 48 57 100 54 55 100 98 97 97 99 102 51 51 98 53 53 57 100 57 54 101 48 54 52 52 49 98 101 52 100 50 50 100 53 101 49 102 57 100 99 53 98 97 50 102 50 57 100 55 50 48 54 48 49 52 56 99 101 101 52 51 98 97 53 53 51 98 54 97 53 51 101 56 56 97 48 55 98 53 54 49 101 48 56 53 48 49 34 125] Signature:0000000111b3a5d4a1a3c096bae2db322f7b6cb433eb093dae0651bb9ca292bf5a7d243516c06ecf3e95291ee4899ad6eec87f2fc44fdff6854e23e7185420236c3d662701}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:40Z","message":"GatewayPrivateKey: 01d7523a51c3d219bec1e0bbd8f8ae41804d65ac1654a76d567767eb99c48e0b73"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:40Z","message":"handleProviderPublishGroupCIDRequest: &{MessageType:8 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 110 111 110 99 101 34 58 49 44 34 112 114 111 118 105 100 101 114 95 105 100 34 58 34 121 110 76 70 109 119 103 104 119 84 112 103 118 114 90 43 82 107 87 50 90 89 75 54 100 75 73 103 57 74 104 119 99 105 50 101 53 106 115 113 99 55 89 61 34 44 34 112 114 105 99 101 95 112 101 114 95 98 121 116 101 34 58 52 50 44 34 101 120 112 105 114 121 95 100 97 116 101 34 58 49 54 49 53 57 52 56 55 56 48 44 34 113 111 115 34 58 52 50 44 34 112 105 101 99 101 95 99 105 100 115 34 58 91 34 43 118 54 107 87 108 121 106 74 54 98 119 74 111 77 113 121 85 120 114 106 89 78 86 72 100 104 47 51 112 84 54 72 74 77 121 122 112 107 106 101 74 77 61 34 44 34 50 78 70 68 84 50 57 121 114 106 90 66 119 102 113 106 82 85 43 80 51 104 69 48 55 48 78 119 81 51 110 55 90 71 79 50 88 108 113 76 99 116 56 61 34 44 34 117 75 78 71 108 105 117 84 77 70 72 90 89 83 120 43 83 120 84 75 115 56 99 104 97 89 108 51 79 76 120 100 54 116 66 66 53 111 85 67 77 109 65 61 34 93 44 34 115 105 103 110 97 116 117 114 101 34 58 34 48 48 48 48 48 48 48 49 54 48 51 55 100 98 99 48 56 57 55 99 50 101 48 98 52 54 53 53 56 55 53 51 54 49 102 50 56 52 53 55 56 102 51 102 50 97 97 57 49 99 99 48 57 100 54 55 100 98 97 97 99 102 51 51 98 53 53 57 100 57 54 101 48 54 52 52 49 98 101 52 100 50 50 100 53 101 49 102 57 100 99 53 98 97 50 102 50 57 100 55 50 48 54 48 49 52 56 99 101 101 52 51 98 97 53 53 51 98 54 97 53 51 101 56 56 97 48 55 98 53 54 49 101 48 56 53 48 49 34 125] Signature:0000000111b3a5d4a1a3c096bae2db322f7b6cb433eb093dae0651bb9ca292bf5a7d243516c06ecf3e95291ee4899ad6eec87f2fc44fdff6854e23e7185420236c3d662701}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:40Z","message":"Decode provider publish group CID request: &{MessageType:8 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 110 111 110 99 101 34 58 49 44 34 112 114 111 118 105 100 101 114 95 105 100 34 58 34 121 110 76 70 109 119 103 104 119 84 112 103 118 114 90 43 82 107 87 50 90 89 75 54 100 75 73 103 57 74 104 119 99 105 50 101 53 106 115 113 99 55 89 61 34 44 34 112 114 105 99 101 95 112 101 114 95 98 121 116 101 34 58 52 50 44 34 101 120 112 105 114 121 95 100 97 116 101 34 58 49 54 49 53 57 52 56 55 56 48 44 34 113 111 115 34 58 52 50 44 34 112 105 101 99 101 95 99 105 100 115 34 58 91 34 43 118 54 107 87 108 121 106 74 54 98 119 74 111 77 113 121 85 120 114 106 89 78 86 72 100 104 47 51 112 84 54 72 74 77 121 122 112 107 106 101 74 77 61 34 44 34 50 78 70 68 84 50 57 121 114 106 90 66 119 102 113 106 82 85 43 80 51 104 69 48 55 48 78 119 81 51 110 55 90 71 79 50 88 108 113 76 99 116 56 61 34 44 34 117 75 78 71 108 105 117 84 77 70 72 90 89 83 120 43 83 120 84 75 115 56 99 104 97 89 108 51 79 76 120 100 54 116 66 66 53 111 85 67 77 109 65 61 34 93 44 34 115 105 103 110 97 116 117 114 101 34 58 34 48 48 48 48 48 48 48 49 54 48 51 55 100 98 99 48 56 57 55 99 50 101 48 98 52 54 53 53 56 55 53 51 54 49 102 50 56 52 53 55 56 102 51 102 50 97 97 57 49 99 99 48 57 100 54 55 100 98 97 97 99 102 51 51 98 53 53 57 100 57 54 101 48 54 52 52 49 98 101 52 100 50 50 100 53 101 49 102 57 100 99 53 98 97 50 102 50 57 100 55 50 48 54 48 49 52 56 99 101 101 52 51 98 97 53 53 51 98 54 97 53 51 101 56 56 97 48 55 98 53 54 49 101 48 56 53 48 49 34 125] Signature:0000000111b3a5d4a1a3c096bae2db322f7b6cb433eb093dae0651bb9ca292bf5a7d243516c06ecf3e95291ee4899ad6eec87f2fc44fdff6854e23e7185420236c3d662701}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:40Z","message":"Stored offers: &{cidMap:map[b8a346962b933051d9612c7e4b14cab3c72169897738bc5dead041e685023260:[[35 144 184 254 109 78 12 2 181 182 114 209 166 103 24 221 254 35 100 149 132 81 194 111 33 248 31 145 130 167 136 153]] d8d1434f6f72ae3641c1faa3454f8fde1134ef43704379fb6463b65e5a8b72df:[[35 144 184 254 109 78 12 2 181 182 114 209 166 103 24 221 254 35 100 149 132 81 194 111 33 248 31 145 130 167 136 153]] fafea45a5ca327a6f026832ac94c6b8d83551dd87fde94fa1c9332ce99237893:[[35 144 184 254 109 78 12 2 181 182 114 209 166 103 24 221 254 35 100 149 132 81 194 111 33 248 31 145 130 167 136 153]]] cidMapLock:{w:{state:0 sema:0} writerSem:0 readerSem:0 readerCount:0 readerWait:0} cidOffers:map[[35 144 184 254 109 78 12 2 181 182 114 209 166 103 24 221 254 35 100 149 132 81 194 111 33 248 31 145 130 167 136 153]:0xc000402660] cidOffersLock:{w:{state:0 sema:0} writerSem:0 readerSem:0 readerCount:0 readerWait:0} offerExpiry:0xc00017a0c0 offerExpiryLock:{w:{state:0 sema:0} writerSem:0 readerSem:0 readerCount:0 readerWait:0}}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:39:40Z","message":"Encode provider publish group CID response: &{NodeID:0xc0004025a8 Cids:[{id:[250 254 164 90 92 163 39 166 240 38 131 42 201 76 107 141 131 85 29 216 127 222 148 250 28 147 50 206 153 35 120 147]} {id:[216 209 67 79 111 114 174 54 65 193 250 163 69 79 143 222 17 52 239 67 112 67 121 251 100 99 182 94 90 139 114 223]} {id:[184 163 70 150 43 147 48 81 217 97 44 126 75 20 202 179 199 33 105 137 119 56 188 93 234 208 65 230 133 2 50 96]}] Price:42 Expiry:1615948780 QoS:42 MerkleRoot:0f6eef2a012bddef80e79e570cff329f9ebff88afb63b49988cb7f8f51c0adf9 MerkleTrie:0xc0000102f0 Signature:000000016037dbc0897c2e0b4655875361f284578f3f2aa91cc09d67dbaacf33b559d96e06441be4d22d5e1f9dc5ba2f29d72060148cee43ba553b6a53e88a07b561e08501}"}
16/Mar/2021:02:39:50 +0000 200 519μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
16/Mar/2021:02:39:50 +0000 200 556μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
16/Mar/2021:02:39:50 +0000 200 443μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
16/Mar/2021:02:39:50 +0000 200 296μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
16/Mar/2021:02:39:50 +0000 200 924μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
{"level":"error","service":"gateway","time":"2021-03-16T02:39:50Z","message":"Error: read tcp 172.18.0.4:9013->172.18.0.6:36002: read: connection reset by peer"}
Stopping provider ... done
Stopping gateway  ... done
Stopping register ... done
Stopping redis    ... done
Removing fc-retrieval-itest_itest_run_cd905dad0468 ... done
Removing provider                                  ... done
Removing gateway                                   ... done
Removing register                                  ... done
Removing redis                                     ... done
Network shared is external, skipping
Creating redis ... done
Creating register ... done
Creating gateway  ... done
Creating provider ... done
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
REDIS STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
1:C 16 Mar 2021 02:40:04.712 # oO0OoO0OoO0Oo Redis is starting oO0OoO0OoO0Oo
1:C 16 Mar 2021 02:40:04.712 # Redis version=6.2.1, bits=64, commit=00000000, modified=0, pid=1, just started
1:C 16 Mar 2021 02:40:04.712 # Warning: no config file specified, using the default config. In order to specify a config file use redis-server /path/to/redis.conf
1:M 16 Mar 2021 02:40:04.713 * monotonic clock: POSIX clock_gettime
1:M 16 Mar 2021 02:40:04.714 * Running mode=standalone, port=6379.
1:M 16 Mar 2021 02:40:04.714 # WARNING: The TCP backlog setting of 511 cannot be enforced because /proc/sys/net/core/somaxconn is set to the lower value of 128.
1:M 16 Mar 2021 02:40:04.714 # Server initialized
1:M 16 Mar 2021 02:40:04.715 * Ready to accept connections
REGISTER STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
2021/03/16 02:40:05 Serving register at http://[::]:9020
GATEWAY STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Container IP: 172.18.0.4
Starting service ...
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Filecoin Gateway Start-up: Started"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Settings: {BindRestAPI:9010 BindProviderAPI:9011 BindGatewayAPI:9012 BindAdminAPI:9013 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-gateway LogFile:gateway.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true GatewayID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F RegisterAPIURL:http://register:9020 GatewayAddress:f0121345 NetworkInfoGateway:172.18.0.4:9012 GatewayRegionCode:US GatewayRootSigningKey:0xABCDE123456789 GatewaySigningKey:0x987654321EDCBA NetworkInfoClient:172.18.0.4:9010 NetworkInfoProvider:172.18.0.4:9011 NetworkInfoAdmin:172.18.0.4:9013}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"All registered gateways: []"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Running REST API on: 9010"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Listening on 9012 for connections from Gateways"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Listening on 9011 for connections from Providers\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Listening on 9013 for connections from admin clients"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Filecoin Gateway Start-up Complete"}
PROVIDER STARTUP Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Filecoin Provider Start-up: Started"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Settings: {BindRestAPI:9030 BindGatewayAPI:9032 BindAdminAPI:9033 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-provider LogFile:provider.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true ProviderID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F ProviderSigAlg:1 RegisterAPIURL:http://register:9020 ProviderAddress:f0121345 ProviderRootSigningKey:0xABCDE123456789 ProviderSigningKey:0x987654321EDCBA ProviderRegionCode:US NetworkInfoClient:127.0.0.1: NetworkInfoGateway:127.0.0.1: NetworkInfoAdmin:127.0.0.1:}"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Running REST API on: 9030"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Listening on 9032 for connections from Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Running Admin API on: 9033"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Update registered Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Filecoin Provider Start-up Complete"}
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Creating fc-retrieval-itest_itest_run ... done
go: downloading github.com/stretchr/testify v1.7.0
go: downloading github.com/ConsenSys/fc-retrieval-gateway-admin v0.0.0-20210315220816-bbffc7dae1f2
go: downloading github.com/ConsenSys/fc-retrieval-provider-admin v0.0.0-20210315220609-1fe0ee54f441
go: downloading github.com/ConsenSys/fc-retrieval-client v0.0.0-20210315220115-b5a58266695e
go: downloading github.com/spf13/viper v1.7.1
go: downloading github.com/ConsenSys/fc-retrieval-common v0.0.0-20210312151557-4caead038a43
go: downloading github.com/ConsenSys/fc-retrieval-register v0.0.0-20210315215728-57ff758e2e2c
go: downloading github.com/bitly/go-simplejson v0.5.0
go: downloading gopkg.in/yaml.v3 v3.0.0-20210107192922-496545a6307b
go: downloading github.com/rs/zerolog v1.20.0
go: downloading github.com/cbergoon/merkletree v0.2.0
go: downloading gopkg.in/natefinch/lumberjack.v2 v2.0.0
go: downloading github.com/davecgh/go-spew v1.1.1
go: downloading golang.org/x/crypto v0.0.0-20210220033148-5ea612d1eb83
go: downloading github.com/pmezard/go-difflib v1.0.0
go: downloading gopkg.in/ini.v1 v1.51.0
go: downloading github.com/spf13/cast v1.3.0
go: downloading github.com/subosito/gotenv v1.2.0
go: downloading github.com/davidlazar/go-crypto v0.0.0-20200604182044-b73af7476f6c
go: downloading github.com/hashicorp/hcl v1.0.0
go: downloading github.com/fsnotify/fsnotify v1.4.9
go: downloading gopkg.in/yaml.v2 v2.4.0
go: downloading github.com/spf13/afero v1.1.2
go: downloading github.com/spf13/pflag v1.0.5
go: downloading github.com/pelletier/go-toml v1.8.1
go: downloading github.com/magiconair/properties v1.8.1
go: downloading github.com/ipsn/go-secp256k1 v0.0.0-20180726113642-9d62b9f0bc52
go: downloading github.com/spf13/jwalterweatherman v1.0.0
go: downloading github.com/mitchellh/mapstructure v1.4.1
go: downloading golang.org/x/sys v0.0.0-20210301091718-77cc2087c03b
go: downloading golang.org/x/text v0.3.5
go: downloading github.com/tatsushid/go-fastping v0.0.0-20160109021039-d7bb493dee3e
go: downloading golang.org/x/net v0.0.0-20210226172049-e18ecbb05110
=== RUN   TestGetProviderAdminVersion
--- PASS: TestGetProviderAdminVersion (0.00s)
=== RUN   TestInitProviderAdminNoRetrievalKey
{"level":"info","time":"2021-03-16T02:41:19Z","message":"/*******************************************************/"}
{"level":"info","time":"2021-03-16T02:41:19Z","message":"/*      Start TestInitProviderAdminNoRetrievalKey\t     */"}
{"level":"info","time":"2021-03-16T02:41:19Z","message":"/*******************************************************/"}
{"level":"error","time":"2021-03-16T02:41:19Z","message":"Wait two seconds for the provider to deploy and be ready for requests"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"Filecoin Retrieval Gateway Admin Client started"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"Filecoin Retrieval Gateway Admin Client: RequestKeyCreation()"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"gatewayRootKey: &{[8 214 16 200 18 149 246 168 110 156 50 239 133 244 98 147 87 173 157 178 190 116 168 21 2 228 230 75 17 120 6 5] [] {1}}"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"gatewayRootSigningKey: 0104caa4783460bf8a7313052ff6c211c2aa2afb57f6c1bcfc347ffd7423ff8b9029f27fcae46380ce4b1832607a2517c6e3345342b7974a77fa0cd029b3bf4e5453"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"Filecoin Retrieval Gateway Admin Client: RequestKeyCreation()"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"gatewayRetrievalPrivateKey: &{[160 207 175 187 195 203 188 63 128 61 36 250 96 21 66 104 86 18 183 98 0 46 200 144 50 74 181 153 186 197 74 153] [] {1}}"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"gatewayRetrievalSigningKey: 01044532a4e1d6a1f41a959b4d5f33529d0877c4fb5a755dbdc0ba34b9917c33f45d5658a7447fca03520ebc531b50ae797f2d9f2a8432e0f851e08134ef36028bc7"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"Filecoin Retrieval Gateway Admin Client: InitializeGateway()"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"Sending message to gateway: ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518, message:     0: 7b 22 6d 65  73 73 61 67  65 5f 74 79  70 65 22 3a  32 30 34 2c  22 70 72 6f  74 6f 63 6f  6c 5f 76 65   | {\"message_type\":204,\"protocol_ve\n   32: 72 73 69 6f  6e 22 3a 31  2c 22 70 72  6f 74 6f 63  6f 6c 5f 73  75 70 70 6f  72 74 65 64  22 3a 5b 31   | rsion\":1,\"protocol_supported\":[1\n   64: 2c 31 5d 2c  22 6d 65 73  73 61 67 65  5f 62 6f 64  79 22 3a 22  65 79 4a 75  62 32 52 6c  58 32 6c 6b   | ,1],\"message_body\":\"eyJub2RlX2lk\n   96: 49 6a 6f 69  4e 6a 68 46  4d 48 42 44  62 54 5a 6d  59 31 4e 43  52 79 39 61  54 58 6b 79  59 30 5a 6d   | IjoiNjhFMHBDbTZmY1NCRy9aTXkyY0Zm\n  128: 4d 58 5a 57  5a 6b 74 53  62 6d 46 42  52 47 6b 35  65 47 4e 34  65 54 68 34  5a 58 52 53  5a 7a 30 69   | MXZWZktSbmFBRGk5eGN4eTh4ZXRSZz0i\n  160: 4c 43 4a 77  63 6d 6c 32  59 58 52 6c  61 32 56 35  49 6a 6f 69  4d 44 46 68  4d 47 4e 6d  59 57 5a 69   | LCJwcml2YXRla2V5IjoiMDFhMGNmYWZi\n  192: 59 6d 4d 7a  59 32 4a 69  59 7a 4e 6d  4f 44 41 7a  5a 44 49 30  5a 6d 45 32  4d 44 45 31  4e 44 49 32   | YmMzY2JiYzNmODAzZDI0ZmE2MDE1NDI2\n  224: 4f 44 55 32  4d 54 4a 69  4e 7a 59 79  4d 44 41 79  5a 57 4d 34  4f 54 41 7a  4d 6a 52 68  59 6a 55 35   | ODU2MTJiNzYyMDAyZWM4OTAzMjRhYjU5\n  256: 4f 57 4a 68  59 7a 55 30  59 54 6b 35  49 69 77 69  63 48 4a 70  64 6d 46 30  5a 57 74 6c  65 58 5a 6c   | OWJhYzU0YTk5IiwicHJpdmF0ZWtleXZl\n  288: 63 6e 4e 70  62 32 34 69  4f 6a 46 39  22 2c 22 6d  65 73 73 61  67 65 5f 73  69 67 6e 61  74 75 72 65   | cnNpb24iOjF9\",\"message_signature\n  320: 22 3a 22 30  30 30 30 30  30 30 31 61  34 37 63 61  62 36 33 31  64 66 34 64  30 38 61 37  36 64 31 64   | \":\"00000001a47cab631df4d08a76d1d\n  352: 63 36 37 31  33 64 62 61  31 31 37 34  37 62 65 37  61 36 30 34  34 65 38 37  32 32 38 61  34 34 33 33   | c6713dba11747be7a6044e87228a4433\n  384: 38 66 38 64  36 61 61 32  37 39 66 34  38 33 32 39  63 38 31 35  38 65 39 33  35 36 35 37  39 32 62 37   | 8f8d6aa279f48329c8158e93565792b7\n  416: 66 66 65 36  64 35 61 37  37 33 66 62  63 63 37 65  63 32 64 63  33 32 61 39  36 36 39 34  30 38 35 35   | ffe6d5a773fbcc7ec2dc32a966940855\n  448: 39 34 65 30  34 64 65 39  39 38 62 30  30 22 7d                                         | 94e04de998b00\"}\n"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"Get active connection, nodeID: ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"No active connection, connect to peer"}
{"level":"debug","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"Got address: gateway:9013"}
{"level":"info","service":"gateway-admin","time":"2021-03-16T02:41:21Z","message":"Response message: &{MessageType:205 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 101 120 105 115 116 115 34 58 116 114 117 101 125] Signature:00000001d7368db0cdc4f48f7e81149811c14031a9f215a1ef7b9e56b212e324d8c12b2119d700f9ec9e91e464cc4816a8be38cca390fcd5792b238b01cee5d85b57983c00}"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:21Z","message":"providerRootKey: &{[64 3 89 17 144 238 210 247 207 158 132 76 151 241 22 14 186 189 144 197 47 45 246 189 210 120 202 142 131 211 61 104] [] {1}}"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:21Z","message":"providerRootSigningKey: 010436277f37cd9bf209f64ede7d71b41bf6dd32e8a4612a7bc49dd47db7389c480397d979cfb266ab0e72fda89abbf5beb79709e34a6346cca69ecc88c168785edc"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:21Z","message":"providerPrivKey: &{[108 163 148 171 104 189 225 238 60 31 242 71 180 34 5 78 109 172 38 126 151 168 247 99 189 206 57 127 141 105 38 160] [] {1}}"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:21Z","message":"providerSigningKey: 010472cccaaaa22bfa1d1f7334ff91cfd549a2c8f261f136ac648bfe04285225af32c0ea1e0eea15f39a02f964efffcd35abcfa25d92753c099b5c77e0a3fd1ad8fe"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:21Z","message":"Sending JSON to url: http://provider:9033/v1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:21Z","message":"Wait 5 seconds for the provider to initialise"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:41Z","message":"Provider Manager sending message to providerID: ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:41Z","message":"Sending JSON to url: http://provider:9033/v1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:41Z","message":"Wait 5 seconds for the provider to publish"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Get all offers"}
EncodeProviderAdminGetGroupCIDRequest
Body: [123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 93 125]
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Provider Manager sending message to providerID: ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Sending JSON to url: http://provider:9033/v1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Get all offers: 1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Registered gateways: [{NodeID:ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518 Address:f0121345 RootSigningKey:0104caa4783460bf8a7313052ff6c211c2aa2afb57f6c1bcfc347ffd7423ff8b9029f27fcae46380ce4b1832607a2517c6e3345342b7974a77fa0cd029b3bf4e5453 SigningKey:01044532a4e1d6a1f41a959b4d5f33529d0877c4fb5a755dbdc0ba34b9917c33f45d5658a7447fca03520ebc531b50ae797f2d9f2a8432e0f851e08134ef36028bc7 RegionCode:US NetworkInfoGateway:gateway:9012 NetworkInfoProvider:gateway:9011 NetworkInfoClient:gateway:9010 NetworkInfoAdmin:gateway:9013}]"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Get offers by real gatewayID=ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518"}
EncodeProviderAdminGetGroupCIDRequest
Body: [123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 34 54 56 69 48 112 67 109 54 102 99 83 66 71 47 90 77 121 50 99 70 102 49 118 86 102 75 82 110 97 65 68 105 57 120 99 120 121 56 120 101 116 82 103 61 34 93 125]
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Provider Manager sending message to providerID: ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Sending JSON to url: http://provider:9033/v1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Get offers by real gatewayID=ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518: 1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Get offers by fake gatewayID=101112131415161718191a1b1c1d1e1f202122232425262728292a2b2c2dfa43"}
EncodeProviderAdminGetGroupCIDRequest
Body: [123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 34 69 66 69 83 69 120 81 86 70 104 99 89 71 82 111 98 72 66 48 101 72 121 65 104 73 105 77 107 74 83 89 110 75 67 107 113 75 121 119 116 43 107 77 61 34 93 125]
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Provider Manager sending message to providerID: ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Sending JSON to url: http://provider:9033/v1"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"Get offers by fake gatewayID=101112131415161718191a1b1c1d1e1f202122232425262728292a2b2c2dfa43: 0"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"/*******************************************************/"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"/*      End TestInitProviderAdminNoRetrievalKey\t       */"}
{"level":"info","service":"provider-admin","time":"2021-03-16T02:41:46Z","message":"/*******************************************************/"}
--- PASS: TestInitProviderAdminNoRetrievalKey (27.09s)
PASS
ok  	command-line-arguments	27.120s
Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
PROVIDER LOGS Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Filecoin Provider Start-up: Started"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Settings: {BindRestAPI:9030 BindGatewayAPI:9032 BindAdminAPI:9033 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-provider LogFile:provider.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true ProviderID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F ProviderSigAlg:1 RegisterAPIURL:http://register:9020 ProviderAddress:f0121345 ProviderRootSigningKey:0xABCDE123456789 ProviderSigningKey:0x987654321EDCBA ProviderRegionCode:US NetworkInfoClient:127.0.0.1: NetworkInfoGateway:127.0.0.1: NetworkInfoAdmin:127.0.0.1:}"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Running REST API on: 9030"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Listening on 9032 for connections from Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Running Admin API on: 9033"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Update registered Gateways"}
{"level":"info","service":"provider","time":"2021-03-16T02:40:06Z","message":"Filecoin Provider Start-up Complete"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:21Z","message":"handle key management."}
{"level":"info","service":"provider","time":"2021-03-16T02:41:21Z","message":"Check if c is nil :false"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:21Z","message":"Setting node id"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:21Z","message":"Signing response."}
16/Mar/2021:02:41:21 +0000 200 2248μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
{"level":"info","service":"provider","time":"2021-03-16T02:41:21Z","message":"Add to registered gateways map: nodeID=ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:41Z","message":"handleProviderPublishGroupCID: &{MessageType:302 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 99 105 100 115 34 58 91 34 83 69 104 107 73 48 67 55 89 76 122 51 66 106 52 104 107 102 110 111 57 77 110 107 84 75 90 110 109 53 66 76 73 121 75 57 82 77 112 54 67 55 107 61 34 93 44 34 112 114 105 99 101 34 58 52 50 44 34 101 120 112 105 114 121 34 58 49 54 49 53 57 52 56 57 48 49 44 34 113 111 115 34 58 52 50 125] Signature:000000018d6fa7d230f001d0b70de382820acea7a7ca815c58f78ad72b51647836a34f83513d5c62362130af327cb40a15bb2dc8988f13c7763dae1c63c091518640be0500}"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:41Z","message":"Get active connection, nodeID: ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:41Z","message":"No active connection, connect to peer"}
{"level":"debug","service":"provider","time":"2021-03-16T02:41:41Z","message":"Got address: gateway:9011"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:41Z","message":"Got reponse from gateway=ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518: &{MessageType:302 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 112 114 111 118 105 100 101 114 95 105 100 34 58 34 54 56 69 48 112 67 109 54 102 99 83 66 71 47 90 77 121 50 99 70 102 49 118 86 102 75 82 110 97 65 68 105 57 120 99 120 121 56 120 101 116 82 103 61 34 44 34 100 105 103 101 115 116 34 58 91 53 44 55 52 44 49 49 48 44 50 49 54 44 49 51 50 44 49 54 53 44 49 50 49 44 49 51 49 44 50 48 44 50 49 54 44 50 48 49 44 49 55 44 50 50 50 44 55 48 44 49 49 48 44 50 51 57 44 49 57 52 44 49 56 51 44 50 49 48 44 50 50 52 44 49 57 55 44 49 50 44 57 52 44 50 49 56 44 49 57 49 44 55 53 44 50 50 49 44 50 51 50 44 49 57 54 44 50 52 53 44 53 55 44 53 50 93 125] Signature:00000001d7368db0cdc4f48f7e81149811c14031a9f215a1ef7b9e56b212e324d8c12b2119d700f9ec9e91e464cc4816a8be38cca390fcd5792b238b01cee5d85b57983c00}"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:41Z","message":"Received digest: [5 74 110 216 132 165 121 131 20 216 201 17 222 70 110 239 194 183 210 224 197 12 94 218 191 75 221 232 196 245 57 52]"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:41Z","message":"Digest is OK! Add offer to storage"}
16/Mar/2021:02:41:41 +0000 200 6720μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
{"level":"info","service":"provider","time":"2021-03-16T02:41:46Z","message":"handleProviderGetGroupCID: &{MessageType:300 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 93 125] Signature:000000018d6fa7d230f001d0b70de382820acea7a7ca815c58f78ad72b51647836a34f83513d5c62362130af327cb40a15bb2dc8988f13c7763dae1c63c091518640be0500}"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:46Z","message":"Find offers: gatewayIDs=[]"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:46Z","message":"Found offers: 1"}
16/Mar/2021:02:41:46 +0000 200 1079μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
{"level":"info","service":"provider","time":"2021-03-16T02:41:46Z","message":"handleProviderGetGroupCID: &{MessageType:300 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 34 54 56 69 48 112 67 109 54 102 99 83 66 71 47 90 77 121 50 99 70 102 49 118 86 102 75 82 110 97 65 68 105 57 120 99 120 121 56 120 101 116 82 103 61 34 93 125] Signature:000000018d6fa7d230f001d0b70de382820acea7a7ca815c58f78ad72b51647836a34f83513d5c62362130af327cb40a15bb2dc8988f13c7763dae1c63c091518640be0500}"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:46Z","message":"Find offers: gatewayIDs=[{id:[235 193 52 164 41 186 125 196 129 27 246 76 203 103 5 127 91 213 124 164 103 104 0 226 247 23 49 203 204 94 181 24]}]"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:46Z","message":"Found offers: 1"}
16/Mar/2021:02:41:46 +0000 200 651μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
{"level":"info","service":"provider","time":"2021-03-16T02:41:46Z","message":"handleProviderGetGroupCID: &{MessageType:300 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 103 97 116 101 119 97 121 95 105 100 34 58 91 34 69 66 69 83 69 120 81 86 70 104 99 89 71 82 111 98 72 66 48 101 72 121 65 104 73 105 77 107 74 83 89 110 75 67 107 113 75 121 119 116 43 107 77 61 34 93 125] Signature:000000018d6fa7d230f001d0b70de382820acea7a7ca815c58f78ad72b51647836a34f83513d5c62362130af327cb40a15bb2dc8988f13c7763dae1c63c091518640be0500}"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:46Z","message":"Find offers: gatewayIDs=[{id:[16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 250 67]}]"}
{"level":"info","service":"provider","time":"2021-03-16T02:41:46Z","message":"Found offers: 0"}
16/Mar/2021:02:41:46 +0000 200 451μs "POST /v1 HTTP/1.1" - "Go-http-client/1.1"
GATEWAY LOGS Dockerfile Dockerfile.dev LICENSE Makefile README.md config docker-compose.dev.yml docker-compose.yml docs go.local.mod go.mod go.sum internal scripts
Container IP: 172.18.0.4
Starting service ...
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Filecoin Gateway Start-up: Started"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Settings: {BindRestAPI:9010 BindProviderAPI:9011 BindGatewayAPI:9012 BindAdminAPI:9013 LogLevel:debug LogTarget:STDOUT LogDir:/var/log/fc-retrieval/fc-retrieval-gateway LogFile:gateway.log LogMaxBackups:3 LogMaxAge:28 LogMaxSize:500 LogCompress:true GatewayID:101112131415161718191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F RegisterAPIURL:http://register:9020 GatewayAddress:f0121345 NetworkInfoGateway:172.18.0.4:9012 GatewayRegionCode:US GatewayRootSigningKey:0xABCDE123456789 GatewaySigningKey:0x987654321EDCBA NetworkInfoClient:172.18.0.4:9010 NetworkInfoProvider:172.18.0.4:9011 NetworkInfoAdmin:172.18.0.4:9013}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"All registered gateways: []"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Running REST API on: 9010"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Listening on 9012 for connections from Gateways"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Listening on 9011 for connections from Providers\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Listening on 9013 for connections from admin clients"}
{"level":"info","service":"gateway","time":"2021-03-16T02:40:05Z","message":"Filecoin Gateway Start-up Complete"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:21Z","message":"Incoming connection from admin client at :172.18.0.6:36174"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:21Z","message":"In handleAdminAcceptKeysChallenge"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:21Z","message":"Message received \n    0: 7b 22 6d 65  73 73 61 67  65 5f 74 79  70 65 22 3a  32 30 34 2c  22 70 72 6f  74 6f 63 6f  6c 5f 76 65   | {\"message_type\":204,\"protocol_ve\n   32: 72 73 69 6f  6e 22 3a 31  2c 22 70 72  6f 74 6f 63  6f 6c 5f 73  75 70 70 6f  72 74 65 64  22 3a 5b 31   | rsion\":1,\"protocol_supported\":[1\n   64: 2c 31 5d 2c  22 6d 65 73  73 61 67 65  5f 62 6f 64  79 22 3a 22  65 79 4a 75  62 32 52 6c  58 32 6c 6b   | ,1],\"message_body\":\"eyJub2RlX2lk\n   96: 49 6a 6f 69  4e 6a 68 46  4d 48 42 44  62 54 5a 6d  59 31 4e 43  52 79 39 61  54 58 6b 79  59 30 5a 6d   | IjoiNjhFMHBDbTZmY1NCRy9aTXkyY0Zm\n  128: 4d 58 5a 57  5a 6b 74 53  62 6d 46 42  52 47 6b 35  65 47 4e 34  65 54 68 34  5a 58 52 53  5a 7a 30 69   | MXZWZktSbmFBRGk5eGN4eTh4ZXRSZz0i\n  160: 4c 43 4a 77  63 6d 6c 32  59 58 52 6c  61 32 56 35  49 6a 6f 69  4d 44 46 68  4d 47 4e 6d  59 57 5a 69   | LCJwcml2YXRla2V5IjoiMDFhMGNmYWZi\n  192: 59 6d 4d 7a  59 32 4a 69  59 7a 4e 6d  4f 44 41 7a  5a 44 49 30  5a 6d 45 32  4d 44 45 31  4e 44 49 32   | YmMzY2JiYzNmODAzZDI0ZmE2MDE1NDI2\n  224: 4f 44 55 32  4d 54 4a 69  4e 7a 59 79  4d 44 41 79  5a 57 4d 34  4f 54 41 7a  4d 6a 52 68  59 6a 55 35   | ODU2MTJiNzYyMDAyZWM4OTAzMjRhYjU5\n  256: 4f 57 4a 68  59 7a 55 30  59 54 6b 35  49 69 77 69  63 48 4a 70  64 6d 46 30  5a 57 74 6c  65 58 5a 6c   | OWJhYzU0YTk5IiwicHJpdmF0ZWtleXZl\n  288: 63 6e 4e 70  62 32 34 69  4f 6a 46 39  22 2c 22 6d  65 73 73 61  67 65 5f 73  69 67 6e 61  74 75 72 65   | cnNpb24iOjF9\",\"message_signature\n  320: 22 3a 22 30  30 30 30 30  30 30 31 61  34 37 63 61  62 36 33 31  64 66 34 64  30 38 61 37  36 64 31 64   | \":\"00000001a47cab631df4d08a76d1d\n  352: 63 36 37 31  33 64 62 61  31 31 37 34  37 62 65 37  61 36 30 34  34 65 38 37  32 32 38 61  34 34 33 33   | c6713dba11747be7a6044e87228a4433\n  384: 38 66 38 64  36 61 61 32  37 39 66 34  38 33 32 39  63 38 31 35  38 65 39 33  35 36 35 37  39 32 62 37   | 8f8d6aa279f48329c8158e93565792b7\n  416: 66 66 65 36  64 35 61 37  37 33 66 62  63 63 37 65  63 32 64 63  33 32 61 39  36 36 39 34  30 38 35 35   | ffe6d5a773fbcc7ec2dc32a966940855\n  448: 39 34 65 30  34 64 65 39  39 38 62 30  30 22 7d                                         | 94e04de998b00\"}\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:21Z","message":"Admin action: Key installation complete"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:25Z","message":"Add to registered providers map: nodeID=ebc134a429ba7dc4811bf64ccb67057f5bd57ca4676800e2f71731cbcc5eb518"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:41Z","message":"Incoming connection from provider at :172.18.0.5:51650\n"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:41Z","message":"Message received: &{MessageType:8 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 110 111 110 99 101 34 58 49 44 34 112 114 111 118 105 100 101 114 95 105 100 34 58 34 54 56 69 48 112 67 109 54 102 99 83 66 71 47 90 77 121 50 99 70 102 49 118 86 102 75 82 110 97 65 68 105 57 120 99 120 121 56 120 101 116 82 103 61 34 44 34 112 114 105 99 101 95 112 101 114 95 98 121 116 101 34 58 52 50 44 34 101 120 112 105 114 121 95 100 97 116 101 34 58 49 54 49 53 57 52 56 57 48 49 44 34 113 111 115 34 58 52 50 44 34 112 105 101 99 101 95 99 105 100 115 34 58 91 34 83 69 104 107 73 48 67 55 89 76 122 51 66 106 52 104 107 102 110 111 57 77 110 107 84 75 90 110 109 53 66 76 73 121 75 57 82 77 112 54 67 55 107 61 34 93 44 34 115 105 103 110 97 116 117 114 101 34 58 34 48 48 48 48 48 48 48 49 101 53 50 97 48 54 54 54 49 50 99 55 50 55 98 48 57 98 52 98 102 99 101 55 50 100 53 48 101 50 56 53 57 49 50 98 100 54 100 97 49 100 102 49 57 99 49 55 55 53 52 100 51 100 55 97 55 56 54 99 53 101 99 48 51 99 101 101 100 48 56 100 49 55 97 102 48 56 97 97 53 49 98 102 98 57 55 97 51 55 52 51 52 98 50 55 98 50 48 48 49 99 50 50 51 98 50 54 99 49 56 51 98 51 101 102 48 57 99 51 51 48 51 100 48 57 52 49 48 49 34 125] Signature:00000001d7368db0cdc4f48f7e81149811c14031a9f215a1ef7b9e56b212e324d8c12b2119d700f9ec9e91e464cc4816a8be38cca390fcd5792b238b01cee5d85b57983c00}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:41Z","message":"GatewayPrivateKey: 01a0cfafbbc3cbbc3f803d24fa601542685612b762002ec890324ab599bac54a99"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:41Z","message":"handleProviderPublishGroupCIDRequest: &{MessageType:8 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 110 111 110 99 101 34 58 49 44 34 112 114 111 118 105 100 101 114 95 105 100 34 58 34 54 56 69 48 112 67 109 54 102 99 83 66 71 47 90 77 121 50 99 70 102 49 118 86 102 75 82 110 97 65 68 105 57 120 99 120 121 56 120 101 116 82 103 61 34 44 34 112 114 105 99 101 95 112 101 114 95 98 121 116 101 34 58 52 50 44 34 101 120 112 105 114 121 95 100 97 116 101 34 58 49 54 49 53 57 52 56 57 48 49 44 34 113 111 115 34 58 52 50 44 34 112 105 101 99 101 95 99 105 100 115 34 58 91 34 83 69 104 107 73 48 67 55 89 76 122 51 66 106 52 104 107 102 110 111 57 77 110 107 84 75 90 110 109 53 66 76 73 121 75 57 82 77 112 54 67 55 107 61 34 93 44 34 115 105 103 110 97 116 117 114 101 34 58 34 48 48 48 48 48 48 48 49 101 53 50 97 48 54 54 54 49 50 99 55 50 55 98 48 57 98 52 98 102 99 101 55 50 100 53 48 101 50 56 53 57 49 50 98 100 54 100 97 49 100 102 49 57 99 49 55 55 53 52 100 51 100 55 97 55 56 54 99 53 101 99 48 51 99 101 101 100 48 56 100 49 55 97 102 48 56 97 97 53 49 98 102 98 57 55 97 51 55 52 51 52 98 50 55 98 50 48 48 49 99 50 50 51 98 50 54 99 49 56 51 98 51 101 102 48 57 99 51 51 48 51 100 48 57 52 49 48 49 34 125] Signature:00000001d7368db0cdc4f48f7e81149811c14031a9f215a1ef7b9e56b212e324d8c12b2119d700f9ec9e91e464cc4816a8be38cca390fcd5792b238b01cee5d85b57983c00}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:41Z","message":"Decode provider publish group CID request: &{MessageType:8 ProtocolVersion:1 ProtocolSupported:[1 1] MessageBody:[123 34 110 111 110 99 101 34 58 49 44 34 112 114 111 118 105 100 101 114 95 105 100 34 58 34 54 56 69 48 112 67 109 54 102 99 83 66 71 47 90 77 121 50 99 70 102 49 118 86 102 75 82 110 97 65 68 105 57 120 99 120 121 56 120 101 116 82 103 61 34 44 34 112 114 105 99 101 95 112 101 114 95 98 121 116 101 34 58 52 50 44 34 101 120 112 105 114 121 95 100 97 116 101 34 58 49 54 49 53 57 52 56 57 48 49 44 34 113 111 115 34 58 52 50 44 34 112 105 101 99 101 95 99 105 100 115 34 58 91 34 83 69 104 107 73 48 67 55 89 76 122 51 66 106 52 104 107 102 110 111 57 77 110 107 84 75 90 110 109 53 66 76 73 121 75 57 82 77 112 54 67 55 107 61 34 93 44 34 115 105 103 110 97 116 117 114 101 34 58 34 48 48 48 48 48 48 48 49 101 53 50 97 48 54 54 54 49 50 99 55 50 55 98 48 57 98 52 98 102 99 101 55 50 100 53 48 101 50 56 53 57 49 50 98 100 54 100 97 49 100 102 49 57 99 49 55 55 53 52 100 51 100 55 97 55 56 54 99 53 101 99 48 51 99 101 101 100 48 56 100 49 55 97 102 48 56 97 97 53 49 98 102 98 57 55 97 51 55 52 51 52 98 50 55 98 50 48 48 49 99 50 50 51 98 50 54 99 49 56 51 98 51 101 102 48 57 99 51 51 48 51 100 48 57 52 49 48 49 34 125] Signature:00000001d7368db0cdc4f48f7e81149811c14031a9f215a1ef7b9e56b212e324d8c12b2119d700f9ec9e91e464cc4816a8be38cca390fcd5792b238b01cee5d85b57983c00}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:41Z","message":"Stored offers: &{cidMap:map[4848642340bb60bcf7063e2191f9e8f4c9e44ca6679b904b2322bd44ca7a0bb9:[[5 74 110 216 132 165 121 131 20 216 201 17 222 70 110 239 194 183 210 224 197 12 94 218 191 75 221 232 196 245 57 52]]] cidMapLock:{w:{state:0 sema:0} writerSem:0 readerSem:0 readerCount:0 readerWait:0} cidOffers:map[[5 74 110 216 132 165 121 131 20 216 201 17 222 70 110 239 194 183 210 224 197 12 94 218 191 75 221 232 196 245 57 52]:0xc0003e42a0] cidOffersLock:{w:{state:0 sema:0} writerSem:0 readerSem:0 readerCount:0 readerWait:0} offerExpiry:0xc0000fa0c0 offerExpiryLock:{w:{state:0 sema:0} writerSem:0 readerSem:0 readerCount:0 readerWait:0}}"}
{"level":"info","service":"gateway","time":"2021-03-16T02:41:41Z","message":"Encode provider publish group CID response: &{NodeID:0xc0003e41e8 Cids:[{id:[72 72 100 35 64 187 96 188 247 6 62 33 145 249 232 244 201 228 76 166 103 155 144 75 35 34 189 68 202 122 11 185]}] Price:42 Expiry:1615948901 QoS:42 MerkleRoot:a81d650576c166e6abba251b93ffa091dfe3e2f26cd84d466bdbc1a79bb58d33 MerkleTrie:0xc0001a2158 Signature:00000001e52a066612c727b09b4bfce72d50e285912bd6da1df19c17754d3d7a786c5ec03ceed08d17af08aa51bfb97a37434b27b2001c223b26c183b3ef09c3303d094101}"}
{"level":"error","service":"gateway","time":"2021-03-16T02:41:46Z","message":"Error: read tcp 172.18.0.4:9013->172.18.0.6:36174: read: connection reset by peer"}
Stopping provider ... done
Stopping gateway  ... done
Stopping register ... done
Stopping redis    ... done
Removing fc-retrieval-itest_itest_run_235f13dc2daf ... done
Removing provider                                  ... done
Removing gateway                                   ... done
Removing register                                  ... done
Removing redis                                     ... done
Network shared is external, skipping
scripts % 
```