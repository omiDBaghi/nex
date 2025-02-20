setInterval(() => {
    let button = document.querySelector("div.relative.w-24.h-16.rounded-full.cursor-pointer");

    if (button) {
        if (button.classList.contains("border-gray-400")) {
            button.click();
            console.log("🔄 Reconnecting...");
        } else {
            console.log("✅ Already connected!");
        }
    } else {
        console.log("⚠️ Button not found!");
    }
}, 3000);
