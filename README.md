# background-image-scroll-effect

```javascript
const bgImg = document.getElementById('bg-image');

window.addEventListener('scroll',()=>{
    updateImage();
})

function updateImage(){
    bgImg.style.opacity = 1 - window.pageYOffset/900;
    console.log(1 - window.pageYOffset/900);
    bgImg.style.backgroundSize = 160 - window.pageYOffset / 12 + ('%');
}
```
