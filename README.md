<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Share Button</title>
    <style>
        .share-button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <button class="share-button">Share</button>

    <script>
        const shareButton = document.querySelector('.share-button');

        shareButton.addEventListener('click', () => {
            // Get the current page URL
            const url = window.location.href;

            // Create a shareable link for social media
            const shareLink = https://www.facebook.com/sharer/sharer.php?u=${encodeURIComponent(url)}; 

            // Open the share link in a new window or tab
            window.open(shareLink, '_blank');
        });
    </script>
</body>
</html>
