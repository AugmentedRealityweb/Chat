
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">">
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
            width: 100%;
            max-width: 600px;
            height: 500px;
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
   <script>
!function(window){
    const host="https://labs.heygen.com",
    url=host+"/guest/streaming-embed?share=eyJxdWFsaXR5IjoiaGlnaCIsImF2YXRhck5hbWUiOiI4YTYxYTQ2ODEyZjA0NjE0ODQ0YWI4MjZk%0D%0AM2IzNWI3MyIsInZvaWNlIjp7InZvaWNlX2lkIjoiODZhMzMwNjY4NDdlNGIxMTkyZjFjMzNiODQ1%0D%0ANjU3YzUifSwicHJldmlld0ltZyI6Imh0dHBzOi8vZmlsZXMyLmhleWdlbi5haS9hdmF0YXIvdjMv%0D%0AOGE2MWE0NjgxMmYwNDYxNDg0NGFiODI2ZDNiMzViNzMvZnVsbC8yLjIvcHJldmlld190YXJnZXQu%0D%0Ad2VicCIsIm5lZWRSZW1vdmVCYWNrZ3JvdW5kIjpmYWxzZSwidXNlcm5hbWUiOiI1NTZkYjQ1NmMw%0D%0AODE0Njc2YTc4YWNkYzBhMWMxZWEyMSJ9&inIFrame=1",
    clientWidth=document.body.clientWidth,
    wrapDiv=document.createElement("div");
    wrapDiv.id="heygen-streaming-embed";
    const container=document.createElement("div");
    container.id="heygen-streaming-container";
    const stylesheet=document.createElement("style");
    stylesheet.innerHTML=`
      #heygen-streaming-embed {
        z-index: 9999;
        position: fixed;
        left: 40px;
        bottom: 40px;
        width: 200px;
        height: 400px; /* Modificat pentru a dubla înălțimea */
        border-radius: 50%;
        border: 2px solid #fff;
        box-shadow: 0px 8px 24px 0px rgba(0, 0, 0, 0.12);
        transition: all linear 0.1s;
        overflow: hidden;

        opacity: 0;
        visibility: hidden;
      }
      #heygen-streaming-embed.show {
        opacity: 1;
        visibility: visible;
      }
      #heygen-streaming-embed.expand {
        ${clientWidth<540?"height: 532px; width: 96%; left: 50%; transform: translateX(-50%);":"height: 732px; width: calc(732px * 16 / 9);"} /* Modificat pentru a dubla înălțimea */
        border: 0;
        border-radius: 8px;
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
      `;
    const iframe=document.createElement("iframe");
    iframe.allowFullscreen=!1,
    iframe.title="Streaming Embed",
    iframe.role="dialog",
    iframe.allow="microphone",
    iframe.src=url;
    let visible=!1,initial=!1;
    window.addEventListener("message",(e=>{
        e.origin===host&&e.data&&e.data.type&&"streaming-embed"===e.data.type&&("init"===e.data.action?(initial=!0,wrapDiv.classList.toggle("show",initial)):"show"===e.data.action?(visible=!0,wrapDiv.classList.toggle("expand",visible)):"hide"===e.data.action&&(visible=!1,wrapDiv.classList.toggle("expand",visible)))
    }));
    container.appendChild(iframe),
    wrapDiv.appendChild(stylesheet),
    wrapDiv.appendChild(container),
    document.body.appendChild(wrapDiv)
}(globalThis);
</script>

</body>
</html>
