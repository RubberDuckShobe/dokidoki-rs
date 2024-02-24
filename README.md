# dokidoki

Custom server for [loic2665](https://github.com/loic2665)'s [HeartRateToWeb](https://github.com/loic2665/HeartRateToWeb).

## Usage

A lot of the instructions from the HeartRateToWeb repo still apply here. Get the client app on your watch and connect by entering your PC's IP and the default port (6547).

But, to use the data in another program, you need a WebSocket client.
Any heart rate updates sent by the watch get sent to all connected WebSocket clients **immediately,** which makes this server a lot more responsive than the original one.

## Credits

- [The original HeartRateToWeb](https://github.com/loic2665/HeartRateToWeb)
- [axum](https://github.com/tokio-rs/axum) ``chat`` and ``websockets`` examples