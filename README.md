<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Xylophone App README</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            line-height: 1.6;
        }
        h1, h2, h3, h4 {
            color: #333;
        }
        code {
            background-color: #f4f4f4;
            padding: 2px 4px;
            border-radius: 4px;
        }
        pre {
            background-color: #f4f4f4;
            padding: 10px;
            border-radius: 4px;
            overflow-x: auto;
        }
    </style>
</head>
<body>

<h1>🎶 Xylophone App</h1>

<p>A simple xylophone app built using HTML, CSS, and JavaScript. Users can tap buttons to play different musical notes, making it a fun and interactive way to explore sound.</p>

<h2>🚀 Features</h2>
<ul>
    <li><strong>Play musical notes</strong>: Each button corresponds to a different note.</li>
    <li><strong>Color-coded buttons</strong>: Seven colored buttons, each linked to a specific sound.</li>
    <li><strong>Responsive design</strong>: Buttons are designed to fit different screen sizes.</li>
</ul>

<h2>🖼️ Screenshots</h2>
<img src="screenshots/app_ui.png" alt="Xylophone App UI" style="width:300px;">

<h2>🛠️ Technologies Used</h2>
<ul>
    <li><strong>HTML</strong>: For structuring the app.</li>
    <li><strong>CSS</strong>: For styling the app.</li>
    <li><strong>JavaScript</strong>: For handling audio playback.</li>
</ul>

<h2>📂 Project Structure</h2>
<pre>
.
├── assets
│   ├── note1.wav
│   ├── note2.wav
│   ├── note3.wav
│   ├── note4.wav
│   ├── note5.wav
│   ├── note6.wav
│   └── note7.wav
├── index.html
├── styles.css
├── script.js
└── README.md
</pre>

<h2>⚙️ Installation</h2>
<p>To run the Xylophone app locally, follow these steps:</p>
<pre>
1. Clone the repository:
    git clone https://github.com/yourusername/xylophone_app.git
    cd xylophone_app

2. Open the HTML file:
    Open index.html in your web browser.
</pre>

<h2>📦 Dependencies</h2>
<p>No additional libraries or frameworks are required. Just a web browser!</p>

<h2>📝 Usage</h2>
<p>Once the app is running, click on any of the colored buttons to play the corresponding xylophone note. Each button represents a different musical note:</p>
<ul>
    <li>Red button (Note 1)</li>
    <li>Green button (Note 2)</li>
    <li>Yellow button (Note 3)</li>
    <li>Blue button (Note 4)</li>
    <li>Orange button (Note 5)</li>
    <li>Purple button (Note 6)</li>
    <li>Teal button (Note 7)</li>
</ul>

<h2>🎨 Customization</h2>
<h3>Adding New Notes:</h3>
<ol>
    <li>Add new sound files to the <code>assets</code> directory.</li>
    <li>Update the <code>playSound</code> function in <code>script.js</code> to handle the new sound files.</li>
</ol>

<h3>Changing Button Colors:</h3>
<p>Modify the CSS classes in <code>styles.css</code> to customize the button colors and styles.</p>

<h2>🔧 Troubleshooting</h2>
<p>If you encounter issues with sound not playing:</p>
<ol>
    <li>Ensure that the audio files are correctly placed in the <code>assets</code> folder.</li>
    <li>Check the file paths in the <code>script.js</code> file to make sure they match the audio files.</li>
</ol>

<h2>🤝 Contributing</h2>
<p>Contributions are welcome! If you find bugs or have feature requests, feel free to open an issue or submit a pull request.</p>

<h2>📄 License</h2>
<p>This project is licensed under the MIT License. See the <code><a href="LICENSE">LICENSE</a></code> file for details.</p>

</body>
</html>
