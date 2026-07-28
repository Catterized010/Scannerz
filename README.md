scannerz

A lightweight, browser-based AI image metadata viewer and prompt browser.

scannerz lets you drag and drop AI-generated images into your browser, automatically read embedded metadata, and browse prompts, tags, generation settings, models, and LoRAs in a clean, searchable interface.

No backend. No uploads. Everything runs directly in your browser.

✨ Features
🖼️ Drag & Drop Images
Easily add multiple AI-generated images by dragging them into the app or selecting them from your computer.
🔍 Fast Search & Filtering
Search across image prompts, negative prompts, tags, models, and LoRAs.
🎯 Filter or Highlight Mode
Choose between showing only matching images or keeping the entire collection visible while highlighting matches.
🤖 AI Metadata Parsing
Reads embedded metadata from supported PNG images and attempts to extract useful generation information automatically.
🧩 Model & LoRA Detection
Detects model names and LoRA references from generation metadata and displays them alongside each image.
📝 Prompt Viewer
View and copy positive and negative prompts directly from the image details panel.
⚙️ Generation Parameters
Displays available generation settings such as:
Steps
CFG Scale
Sampler
Scheduler
Seed
Denoise
Image Size
Model
🛠️ ComfyUI Support
Attempts to extract prompts, generation parameters, checkpoints, and LoRA information from ComfyUI workflow metadata.
📋 Raw Metadata Viewer
Inspect the original metadata stored inside an image when available.
📱 Responsive Interface
Designed to work on both desktop and smaller screens.
🔒 Client-Side Only
Images are processed locally in your browser. There is no server-side image upload or database required.
🧠 Supported Metadata

scannerz is designed primarily around metadata commonly embedded in AI-generated PNG files.

It can recognize metadata formats including:

tEXt
iTXt
zTXt

The application can then attempt to parse metadata from formats commonly produced by tools such as:

Stable Diffusion / AUTOMATIC1111-style metadata
ComfyUI workflows
Other AI image generators that embed compatible PNG metadata

Metadata parsing includes prompts, negative prompts, generation parameters, models, and LoRAs when the required information is available.

🖥️ How It Works
Open scannerz in your browser.
Drag and drop your AI-generated images into the application.
scannerz reads available PNG metadata directly in the browser.
Metadata is parsed into prompts, tags, models, LoRAs, and generation parameters.
Browse your images in a searchable grid.
Click an image to open its detailed metadata panel.
Copy prompts or raw metadata with one click.
🔎 Searching

The search bar can find images based on:

Positive prompts
Negative prompts
Tags
Model names
LoRA names

You can either:

Filter Only — display only images matching your search.

Highlight All — keep all images visible while highlighting matching images and tags.

Search results update automatically as you type.

🧰 Technologies

Built with:

HTML5
CSS3
Vanilla JavaScript
PNG metadata parsing
Browser File API
DecompressionStream API
Font Awesome
Google Fonts

No framework or build system is required.



⚠️ Limitations
Metadata can only be displayed when it is embedded in the image and stored in a format scannerz recognizes.
Images without compatible metadata will still be displayed, but their prompts and generation information may not be available.
Metadata parsing may vary between different AI image generation tools and versions.
The application currently focuses primarily on PNG metadata.
🔐 Privacy

scannerz is designed as a local, browser-based tool.

Your images are processed in your browser and are not automatically uploaded to a remote server by the application.


