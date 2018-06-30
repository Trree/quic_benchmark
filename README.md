# 测试quic协议的caddy服务器的性能

原始的quic benchmark从 [proto-quic](https://github.com/google/proto-quic/tree/master/src/net/tools/quic/benchmark)复制过来。
测试的过程是用python执行quic\_client的脚本

但是因为需要测试caddy服务器的性能，所以在测试的时候加入多线程。这样带来的后果是性能瓶颈在测试机cpu上面，所以后期需要改进测试程序。
