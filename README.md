# [jsonrpc2websocket](https://github.com/Hxgh/jsonrpc2websocket)

基于WebSocket+JSONRPC+msgpack+TypeScript封装的实时通讯函数
- [msgpack-lite](https://github.com/kawanet/msgpack-lite/)
- [JSON-RPC 2.0](http://wiki.geekdream.com/Specification/json-rpc_2.0.html)

### 安装

```sh
$ npm install jsonrpc2websocket
# or
yarn add jsonrpc2websocket
```
### 使用
```
import Socket, { SocketType } from 'jsonrpc2websocket';

const socket: SocketType = new Socket({ url: 'ws://url' });

socket.communicate({
    method: 'sayhellosync',
    callback: e => {
      console.log(e);
    },
});

```