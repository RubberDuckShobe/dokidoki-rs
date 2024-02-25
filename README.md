# dokidoki

Very simple custom server for [loic2665](https://github.com/loic2665)'s [HeartRateToWeb](https://github.com/loic2665/HeartRateToWeb) that bridges the data to WebSocket.

This is mainly intended for myself so I can have a custom, near-real-time heart rate display in [Resonite](https://store.steampowered.com/app/2519830/Resonite/). It works really well!

![grafik](https://github.com/RubberDuckShobe/dokidoki-rs/assets/42943070/e46b86ec-4d4a-4998-8d10-afc62aa123c2)
![grafik](https://github.com/RubberDuckShobe/dokidoki-rs/assets/42943070/c944a76e-7a78-4138-b0f8-add022ee072d)

## Usage

A lot of the instructions from the HeartRateToWeb repo still apply here. Get the client app on your watch and connect by entering your PC's IP and the default port (6547).

But, to use the data in another program, you need a WebSocket client.
Any heart rate updates sent by the watch get sent to all connected WebSocket clients **immediately,** which makes this server a lot more responsive than the original one.

## Credits

- [The original HeartRateToWeb](https://github.com/loic2665/HeartRateToWeb)
- [axum](https://github.com/tokio-rs/axum) ``chat`` and ``websockets`` examples
