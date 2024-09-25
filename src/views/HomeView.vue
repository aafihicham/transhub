<template>
  <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Social Profile Page</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
</head>
<body class="bg-gray-100 flex items-center justify-center min-h-screen">

    <div class="max-w-md mx-auto bg-white rounded-lg shadow-lg overflow-hidden">
        <!-- Profile Header -->
        <div class="relative">
            <img class="w-full h-32 object-cover" src="https://via.placeholder.com/800x200" alt="Cover Photo">
            <div class="absolute top-24 left-1/2 transform -translate-x-1/2">
                <img class="w-32 h-32 rounded-full border-4 border-white" src="https://via.placeholder.com/150" alt="Profile Photo">
            </div>
        </div>

        <!-- Profile Content -->
        <div class="p-6 text-center">
            <h1 class="text-2xl font-bold text-gray-900">John Doe</h1>
            <p class="text-gray-600">Web Developer | Designer | Content Creator</p>
            <div class="mt-4">
                <a href="#" class="text-blue-500 hover:underline">www.johndoe.com</a>
            </div>

            <!-- Social Links -->
            <div class="mt-6 flex justify-center space-x-4">
                <a href="#" class="text-gray-600 hover:text-gray-800">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><path d="M22.23 12.44c0-.44-.04-.88-.1-1.3H12v2.53h5.71c-1.4 7.41-6.02 12.67-11.73 12.67-7.1 0-12.91-5.85-12.91-13s5.81-13 12.91-13c2.55 0 4.97.75 7 2.06l-2.87 2.82c-1.43-1.32-3.27-2.14-5.13-2.14-4.35 0-7.88 3.53-7.88 7.88s3.53 7.88 7.88 7.88c4.35 0 7.88-3.53 7.88-7.88z"/></svg>
                </a>
                <a href="#" class="text-gray-600 hover:text-gray-800">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><path d="M23.49 4.56c-.88-.39-1.83-.66-2.82-.77-1.09-1.15-2.5-1.86-4.02-1.86-3.05 0-5.52 2.47-5.52 5.52 0 .43.05.85.13 1.26-4.6-.23-8.69-2.44-11.43-5.8-.48.83-.76 1.79-.76 2.83 0 1.95 1 3.66 2.5 4.66-.92-.03-1.8-.28-2.56-.69v.07c0 2.71 1.93 4.96 4.49 5.48-.47.13-.96.2-1.46.2-.36 0-.71-.03-1.06-.1.71 2.23 2.78 3.86 5.23 3.91-1.92 1.5-4.34 2.39-6.97 2.39-.45 0-.9-.03-1.34-.08 2.48 1.59 5.43 2.52 8.6 2.52 10.33 0 16.01-8.56 16.01-16 0-.25-.01-.5-.02-.75 1.1-.8 2.06-1.81 2.83-2.97z"/></svg>
                </a>
                <a href="#" class="text-gray-600 hover:text-gray-800">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><path d="M12 12.1c-2.07 0-3.94-1.68-3.94-3.74s1.87-3.74 3.94-3.74 3.94 1.68 3.94 3.74-1.87 3.74-3.94 3.74zm0-8.43c-2.59 0-4.69 2.1-4.69 4.69 0 2.59 2.1 4.69 4.69 4.69 2.59 0 4.69-2.1 4.69-4.69 0-2.59-2.1-4.69-4.69-4.69zM12 15.47c-3.41 0-6.64-1.47-8.88-3.76-.24-.24-.23-.64.01-.88 1.11-.96 2.37-1.8 3.7-2.52.27-.14.6-.02.73.25 1.43 2.58 4.05 4.43 7.44 4.43 3.39 0 6.02-1.85 7.44-4.43.14-.27.46-.39.73-.25 1.33.72 2.59 1.56 3.7 2.52.24.24.25.64.01.88-2.24 2.29-5.48 3.76-8.89 3.76z"/></svg>
                </a>
            </div>
        </div>
    </div>

</body>
</html>

</template>
