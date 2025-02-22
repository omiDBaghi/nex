```javascript
setInterval(() => {
    let button = document.querySelector("div.relative.w-24.h-16.rounded-full.cursor-pointer");

    if (button) {
        let text = button.innerText || button.textContent;
        if (text.includes("Disconnected")) {
            button.click();
            console.log("🔄 Reconnecting...");
        } else {
            console.log("✅ Already connected!");
        }
    } else {
        console.log("⚠️ Button not found!");
    }
}, 10000);
```
```javascript
setInterval(() => {
    let button = document.querySelector('.relative.w-24.h-16');

    if (button) {
        let isOff = button.classList.contains('border-gray-400');

        if (isOff) {
            button.click();
            console.log("Button turned ON!");
        }
    }
}, 1000);
