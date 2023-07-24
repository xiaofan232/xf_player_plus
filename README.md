# xf_player_plus

flutter video player with ui package.
Now you can setup video player UI by yourself!

## Getting Started

```dart
import 'package:flutter/material.dart';
import 'package:xf_player_plus/xf_player_plus.dart';
class Demo extends StatelessWidget {
  const Demo({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    final url = "http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ElephantsDream.mp4";
    return Scaffold(
      backgroundColor: Colors.white70,
      body: Center(
        // 该组件宽高默认填充父控件，你也可以自己设置宽高
        child: SizedBox(
          height: 300,
          width: 300,
          child: VideoPlayerUI(opts: PlayerOpts(url)),
        ),
      ),
    );
  }
}
