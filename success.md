# binaries installation output - sucess

jaz@jaz-ThinkBook-14-G2-ITL:~/Documents/ACADEMICS/BLOCKCHAIN/FABRIC-2.0-NET$ sudo ./install-fabric.sh --fabric-version 2.
5.0 binary d s
[sudo] password for jaz:

Clone hyperledger/fabric-samples repo

===> Changing directory to fabric-samples
fabric-samples v2.5.0 does not exist, defaulting to main. fabric-samples main branch is intended to work with recent versions of fabric.

Pull Hyperledger Fabric binaries

===> Downloading version 2.5.0 platform specific fabric binaries
===> Downloading:  <https://github.com/hyperledger/fabric/releases/download/v2.5.0/hyperledger-fabric-linux-amd64-2.5.0.tar.gz>

===> Will unpack to: /home/jaz/Documents/ACADEMICS/BLOCKCHAIN/FABRIC-2.0-NET/fabric-samples
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100 99.3M  100 99.3M    0     0  4746k      0  0:00:21  0:00:21 --:--:-- 5436k
==> Done.
===> Downloading version 1.5.10 platform specific fabric-ca-client binary
===> Downloading:  <https://github.com/hyperledger/fabric-ca/releases/download/v1.5.10/hyperledger-fabric-ca-linux-amd64-1.5.10.tar.gz>

===> Will unpack to: /home/jaz/Documents/ACADEMICS/BLOCKCHAIN/FABRIC-2.0-NET/fabric-samples
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100 28.6M  100 28.6M    0     0  3558k      0  0:00:08  0:00:08 --:--:-- 6481k
==> Done.

Pull Hyperledger Fabric docker images

FABRIC_IMAGES: peer orderer ccenv baseos
===> Pulling fabric Images
====>  docker.io/hyperledger/fabric-peer:2.5.0
2.5.0: Pulling from hyperledger/fabric-peer
06d39c85623a: Pull complete
3d265a486208: Pull complete
a2120d0078ca: Pull complete
faa5f851501c: Pull complete
d3d4a3bbe808: Pull complete
e029282af2d0: Pull complete
Digest: sha256:d79a6ce784f5f68d96e0eccb19ee74f742c8bbc75b22db230112937983b6b52c
Status: Downloaded newer image for hyperledger/fabric-peer:2.5.0
docker.io/hyperledger/fabric-peer:2.5.0
====>  docker.io/hyperledger/fabric-orderer:2.5.0
2.5.0: Pulling from hyperledger/fabric-orderer
06d39c85623a: Already exists
9d825e712cf1: Pull complete
3515837e95f6: Pull complete
279927cdc50a: Pull complete
be2a8264820d: Pull complete
c84d45795828: Pull complete
Digest: sha256:eee99d70a62336adea6b6eb0bc905c67ea3c7cb8260ab84b880e94d250c889ba
Status: Downloaded newer image for hyperledger/fabric-orderer:2.5.0
docker.io/hyperledger/fabric-orderer:2.5.0
====>  docker.io/hyperledger/fabric-ccenv:2.5.0
2.5.0: Pulling from hyperledger/fabric-ccenv
06d39c85623a: Already exists
32b5242d3b9f: Pull complete
8a8fb5b785c8: Pull complete
c565813f64d4: Pull complete
1fbc11649090: Pull complete
a4c7e616ab97: Pull complete
a7b43f338b5c: Pull complete
Digest: sha256:8a5db6f2181a681fbda0d66ad884bbaa2a1266b5bc6fb9e608982deaa74a4fe5
Status: Downloaded newer image for hyperledger/fabric-ccenv:2.5.0
docker.io/hyperledger/fabric-ccenv:2.5.0
====>  docker.io/hyperledger/fabric-baseos:2.5.0
2.5.0: Pulling from hyperledger/fabric-baseos
06d39c85623a: Already exists
c8a44e77f433: Pull complete
a5cda75c31bc: Pull complete
2430da07214f: Pull complete
Digest: sha256:c6648cbaa846dcee3bce3004ff85074f9d525dbbf8ad18b0e809b38eb4335a4e
Status: Downloaded newer image for hyperledger/fabric-baseos:2.5.0
docker.io/hyperledger/fabric-baseos:2.5.0
===> Pulling fabric ca Image
====>  docker.io/hyperledger/fabric-ca:1.5.10
1.5.10: Pulling from hyperledger/fabric-ca
17d0386c2fff: Pull complete
e34750fbc60d: Pull complete
694860b29955: Pull complete
be49257713f2: Pull complete
Digest: sha256:09a67ee71cfdb2861475d37cfcc822f00545dc6852a43a6326e608b5926da1b5
Status: Downloaded newer image for hyperledger/fabric-ca:1.5.10
docker.io/hyperledger/fabric-ca:1.5.10
===> List out hyperledger images
hyperledger/fabric-ca        1.5       da516cafd70e   4 weeks ago     206MB
hyperledger/fabric-ca        1.5.10    da516cafd70e   4 weeks ago     206MB
hyperledger/fabric-ca        latest    da516cafd70e   4 weeks ago     206MB
hyperledger/fabric-orderer   2.5       6c3b8eae207f   13 months ago   106MB
hyperledger/fabric-orderer   2.5.0     6c3b8eae207f   13 months ago   106MB
hyperledger/fabric-orderer   latest    6c3b8eae207f   13 months ago   106MB
hyperledger/fabric-peer      2.5       3d131d2433b1   13 months ago   135MB
hyperledger/fabric-peer      2.5.0     3d131d2433b1   13 months ago   135MB
hyperledger/fabric-peer      latest    3d131d2433b1   13 months ago   135MB
hyperledger/fabric-ccenv     2.5       84c7e32cc1fe   13 months ago   650MB
hyperledger/fabric-ccenv     2.5.0     84c7e32cc1fe   13 months ago   650MB
hyperledger/fabric-ccenv     latest    84c7e32cc1fe   13 months ago   650MB
hyperledger/fabric-baseos    2.5       082924a105c1   13 months ago   119MB
hyperledger/fabric-baseos    2.5.0     082924a105c1   13 months ago   119MB
hyperledger/fabric-baseos    latest    082924a105c1   13 months ago   119MB
