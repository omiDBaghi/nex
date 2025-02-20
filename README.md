```javascript
setInterval(() => {
    let button = document.querySelector("div.relative.w-24.h-16.rounded-full.cursor-pointer");

    if (button) {
        let text = button.innerText || button.textContent;
        if (text.includes("Disconnected")) { // اگر دکمه در حالت دیسکانکت بود
            button.click();
            console.log("🔄 Reconnecting...");
        } else {
            console.log("✅ Already connected!");
        }
    } else {
        console.log("⚠️ Button not found!");
    }
}, 3000);

