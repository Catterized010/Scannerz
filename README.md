-Scannerz :

A lightweight, browser-based metadata viewer and prompt browser for AI-generated images.
Scannerz lets you drag and drop AI-generated images into your browser, automatically read embedded metadata, and browse prompts, tags, generation settings, models, and LoRAs in a clean, searchable interface. There is no backend and no uploads — everything runs directly in your browser.

-Features :

    ~Drag and drop images — Add multiple AI-generated images by dragging them into the app or selecting them from your computer.

    ~Search and filtering — Search across prompts, negative prompts, tags, models, and LoRAs.

    ~Filter or highlight mode — Choose to show only matching images, or keep the full collection visible with matches highlighted.
 
    ~Metadata parsing — Reads embedded metadata from supported PNG images and extracts generation information automatically.
 
    ~Model and LoRA detection — Detects model names and LoRA references from generation metadata and displays them with each image.
 
    ~Prompt viewer — View and copy positive and negative prompts from the image details panel.

    ~Generation parameters — Displays available settings, including steps, CFG scale, sampler, scheduler, seed, denoise, image size, and model.

    ~ComfyUI support — Extracts prompts, generation parameters, checkpoints, and LoRA information from ComfyUI workflow metadata.
 
    ~Raw metadata viewer — Inspect the original metadata stored inside an image.

    ~Responsive interface — Works on desktop and smaller screens.

    ~Client-side only — Images are processed locally in the browser; there is no server-side upload or database.


-Supported metadata : 

    Scannerz is built around metadata commonly embedded in AI-generated PNG files, including the tEXt, iTXt, and zTXt chunk types. It can parse metadata produced by:

        -Stable Diffusion / AUTOMATIC1111-style metadata
        -ComfyUI workflows
        -Other AI image generators that embed compatible PNG metadata

    Parsed metadata includes prompts, negative prompts, generation parameters, models, and LoRAs, where the required information is available.

-How it works : 
    
    Open Scannerz in your browser.
    Drag and drop your AI-generated images into the application.
    Scannerz reads available PNG metadata directly in the browser.
    Metadata is parsed into prompts, tags, models, LoRAs, and generation parameters.
    Browse your images in a searchable grid.
    Click an image to open its detailed metadata panel.
    Copy prompts or raw metadata with one click.
    
-Searching : 

The search bar matches against:

    Positive prompts
    Negative prompts
    Tags
    Model names
    LoRA names

Two search modes are available:

    Filter only — displays only images matching your search.
    Highlight all — keeps all images visible while highlighting matches.

Results update automatically as you type.

-Technologies :

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

_Limitations : 
    Metadata can only be displayed when it is embedded in the image and stored in a format scannerz recognizes.
    Images without compatible metadata will still display, but prompts and generation information may not be available.
    Metadata parsing may vary between different AI image generation tools and versions.
    The application currently focuses primarily on PNG metadata.

Privacy

scannerz is a local, browser-based tool. Images are processed in your browser and are not automatically uploaded to a remote server by the application.
