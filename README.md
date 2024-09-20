<!DOCTYPE html>
<html lang="en">
<head>

<title>Xylophone App</title>
<style>
    body {
        font-family: Arial, sans-serif;
        line-height: 1.6;
        margin: 20px;
        background-color: #f4f4f4;
    }
    h1, h2 {
        color: #333;
    }
    pre {
        background-color: #eaeaea;
        padding: 10px;
        border-radius: 5px;
    }
</style>
</head>
<body>

<h1>Xylophone App</h1>
<p>This is a simple Flutter app that simulates a xylophone. Pressing the buttons plays different musical notes.</p>

<h2>Features</h2>
<ul>
    <li>Seven colorful buttons representing different musical notes.</li>
    <li>Play sounds when buttons are pressed.</li>
    <li>Responsive design for various screen sizes.</li>
</ul>

<h2>Technologies Used</h2>
<ul>
    <li>Flutter</li>
    <li>Dart</li>
    <li>just_audio package for sound playback</li>
</ul>

<h2>Installation</h2>
<pre>
# Clone the repository
git clone https://github.com/yourusername/xylophone_app.git

# Navigate to the project directory
cd xylophone_app

# Install dependencies
flutter pub get

# Run the app
flutter run
</pre>

<h2>Usage</h2>
<p>Press the colored buttons to play different notes. Make sure you have the sound files in the <code>assets</code> folder.</p>

<h2>Code Overview</h2>
<p>The main functionality is implemented in the <code>main.dart</code> file:</p>
<pre>
import 'dart:math';
import 'package:flutter/material.dart';
import 'package:just_audio/just_audio.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return const MaterialApp(home: Xylophone());
  }
}

class Xylophone extends StatefulWidget {
  const Xylophone({super.key});

  @override
  State<Xylophone> createState() => _XylophoneState();
}

class _XylophoneState extends State<Xylophone> {
  Future<void> playSound(int soundAsset) async {
    final player = AudioPlayer();
    player.setAsset("assets/note$soundAsset.wav");
    await player.play();
  }

  Widget buildButton(int num, Color buttonColor) {
    return Expanded(
      child: ElevatedButton(
        style: ElevatedButton.styleFrom(
          shape: const RoundedRectangleBorder(borderRadius: BorderRadius.zero),
          backgroundColor: buttonColor,
        ),
        onPressed: () => playSound(num),
        child: const Text(''),
      ),
    );
  }

  @override
  Widget build(BuildContext context) {
    return Center(
      child: Column(
        crossAxisAlignment: CrossAxisAlignment.stretch,
        children: [
          buildButton(1, Colors.red),
          buildButton(2, Colors.green),
          buildButton(3, Colors.yellow),
          buildButton(4, Colors.blue),
          buildButton(5, Colors.orange),
          buildButton(6, Colors.purple),
          buildButton(7, Colors.teal),
        ],
      ),
    );
  }
}
</pre>

<h2>License</h2>
<p>This project is licensed under the MIT License.</p>

<h2>Contributors</h2>
<p>Feel free to contribute to this project by forking the repository and submitting a pull request.</p>

</body>
</html>
