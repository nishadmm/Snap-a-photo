# Snap-a-photo
## Snap a photo using vanila Javascript
  ##### Javascript code :medal_sports:
```javascript
const video = document.getElementById("video"),
button = document.querySelector(".btn"),
canvas = document.getElementById("canvas"),
context = canvas.getContext("2d")

navigator.getUserMedia(
{ video: true },
stream => video.srcObject = stream,
err => console.error(err)
)

button.addEventListener("click", () => {
context.drawImage(video, 0, 0, 480, 320)
})
```
 
