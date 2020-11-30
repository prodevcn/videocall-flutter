import 'package:flutter/material.dart';
import 'dart:core';
import 'call_sample.dart';
import 'call_sample.dart';

class CallSettings extends StatefulWidget {
  static String tag = 'call_settings';
  final bool videoSetting;
  final bool audioSetting;
  CallSettings({Key key, @required this.videoSetting, @required this.audioSetting}) : super(key: key);
  @override
  _CallSettingsState createState() => new _CallSettingsState(video: videoSetting,audio: audioSetting);
}

class _CallSettingsState extends State<CallSettings> {
  bool video;
  bool audio;
  CallSample _callSample;
  _CallSettingsState({Key key, @required this.video,@required this.audio});
  @override
  initState() {
    super.initState();
  }

  @override
  deactivate() {
    super.deactivate();

  }


  @override
  Widget build(BuildContext context) {
    return new Scaffold(
      appBar: new AppBar(
        title: new Text('Settings'),
      ),
      body: ListView(
        padding: const EdgeInsets.all(8),
        children: <Widget>[
          Container(
            child: SwitchListTile(
              contentPadding: EdgeInsets.fromLTRB(40, 20, 40, 0),
              title: const Text('Video Call'),
              value: video,
              onChanged: (bool value) { setState(() { video = value; video = _callSample.setVideoSetting(); }); },
              secondary: const Icon(Icons.video_label),
            ),
          ),
          Container(
            child: SwitchListTile(
              contentPadding: EdgeInsets.fromLTRB(40, 20, 40, 0),
              title: const Text('Audio Call'),
              value: audio,
              onChanged: (bool value) { setState(() { audio = value; audio = _callSample.setAudioSetting();}); },
              secondary: const Icon(Icons.call),
            ),
          ),
        ],
      )
    );
  }

  
}


