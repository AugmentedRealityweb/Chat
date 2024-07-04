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
            <script>!function(window){const host="https://app.heygen.com",url=host+"/guest/streaming-embed?share=eyJxdWFsaXR5IjoiaGlnaCIsImF2YXRhck5hbWUiOiJMaWx5X3B1YmxpY19wcm8xXzIwMjMwNjE0%0D%0AIiwidm9pY2UiOnsidm9pY2VfaWQiOiIyMzJlM2JiMjlmM2I0NWQ2OTVmODczNTAzYWY3MDY4YyJ9%0D%0ALCJwcmV2aWV3SW1nIjoiaHR0cHM6Ly9maWxlcy5oZXlnZW4uYWkvYXZhdGFyL3YzLzUxMjY3YzBm%0D%0AMGYyMDQ1NTE4YThjNjZiYjE3MDliZjJhXzI2NTQvcHJldmlld190YXJnZXQud2VicCIsIm5lZWRS%0D%0AZW1vdmVCYWNrZ3JvdW5kIjp0cnVlLCJ1c2VybmFtZSI6IjU1NmRiNDU2YzA4MTQ2NzZhNzhhY2Rj%0D%0AMGExYzFlYTIxIn0%3D&inIFrame=1",clientWidth=document.body.clientWidth,wrapDiv=document.createElement("div");wrapDiv.id="heygen-streaming-embed";const container=document.createElement("div");container.id="heygen-streaming-container";const stylesheet=document.createElement("style");stylesheet.innerHTML=\n  #heygen-streaming-embed {\n    z-index: 9999;\n    position: fixed;\n    left: 40px;\n    bottom: 40px;\n    width: 200px;\n    height: 200px;\n    border-radius: 50%;\n    border: 2px solid #fff;\n    box-shadow: 0px 8px 24px 0px rgba(0, 0, 0, 0.12);\n    transition: all linear 0.1s;\n    overflow: hidden;\n\n    opacity: 0;\n    visibility: hidden;\n  }\n  #heygen-streaming-embed.show {\n    opacity: 1;\n    visibility: visible;\n  }\n  #heygen-streaming-embed.expand {\n    ${clientWidth<540?"height: 266px; width: 96%; left: 50%; transform: translateX(-50%);":"height: 366px; width: calc(366px * 16 / 9);"}\n    border: 0;\n    border-radius: 8px;\n  }\n  #heygen-streaming-container {\n    width: 100%;\n    height: 100%;\n  }\n  #heygen-streaming-container iframe {\n    width: 100%;\n    height: 100%;\n    border: 0;\n  }\n  ;const iframe=document.createElement("iframe");iframe.allowFullscreen=!1,iframe.title="Streaming Embed",iframe.role="dialog",iframe.src=url;let visible=!1,initial=!1;window.addEventListener("message",(e=>{e.origin===host&&e.data&&e.data.type&&"streaming-embed"===e.data.type&&("init"===e.data.action?(initial=!0,wrapDiv.classList.toggle("show",initial)):"show"===e.data.action?(visible=!0,wrapDiv.classList.toggle("expand",visible)):"hide"===e.data.action&&(visible=!1,wrapDiv.classList.toggle("expand",visible)))})),container.appendChild(iframe),wrapDiv.appendChild(stylesheet),wrapDiv.appendChild(container),document.body.appendChild(wrapDiv)}(globalThis);</script>
        </div>
    </div>
</script>
</body>
</html>
