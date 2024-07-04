<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HeyGen Streaming Avatar</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            background-color: black;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        #heygen-streaming-embed {
            z-index: 9999;
            width: 80%;
            max-width: 400px;
            height: auto;
            border-radius: 10px;
            border: 2px solid #fff;
            box-shadow: 0px 8px 24px 0px rgba(0, 0, 0, 0.12);
            overflow: hidden;
        }
        #heygen-streaming-container {
            width: 100%;
            height: 100%;
        }
        #heygen-streaming-container iframe {
            width: 100%;
            height: 100%;
            border: 0;
        }
    </style>
</head>
<body>
    <div id="heygen-streaming-embed">
        <div id="heygen-streaming-container">
            <iframe allowfullscreen="false" title="Streaming Embed" role="dialog" src="https://labs.heygen.com/guest/streaming-embed?share=eyJxdWFsaXR5IjoiaGlnaCIsImF2YXRhck5hbWUiOiJkZWZhdWx0Iiwidm9pY2UiOnsidm9pY2Vf%0D%0AaWQiOiI2ZDliZTYxZjZlMDY0NmY0YjY3NTBkM2ViMDNiMTE4ZiJ9LCJwcmV2aWV3SW1nIjoiaHR0%0D%0AcHM6Ly9maWxlczIuaGV5Z2VuLmFpL2F2YXRhci92My8xYzRmYTllOTk0MDg0ODc0OGFmMmNiNzlm%0D%0ANTc3MTY2ZF8xMDg1L3ByZXZpZXdfdGFsa181LndlYnAiLCJuZWVkUmVtb3ZlQmFja2dyb3VuZCI6%0D%0AdHJ1ZSwidXNlcm5hbWUiOiI1NTZkYjQ1NmMwODE0Njc2YTc4YWNkYzBhMWMxZWEyMSJ9&inIFrame=1"></iframe>
        </div>
    </div>
</script>
</body>
</html>
