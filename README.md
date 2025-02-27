<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>App Redirect</title>
    <script>
        window.onload = function() {
            var userAgent = navigator.userAgent || navigator.vendor || window.opera;
            if (/android/i.test(userAgent)) {
                window.location.href = "https://play.google.com/store/apps/details?id=com.bharatcarcab_customer.customer";
            } else if (/iPad|iPhone|iPod/.test(userAgent) && !window.MSStream) {
                window.location.href = "https://apps.apple.com/in/app/bharat-self-drive/id6740058759";
            } else {
                window.location.href = "https://bharatselfdrive.com/index.html"; // Optional fallback
            }
        };
    </script>
</head>
<body>
    <p>Redirecting to the appropriate app store...</p>
</body>
</html>
