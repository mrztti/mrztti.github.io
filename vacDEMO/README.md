<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
    <title>vactcha</title>
    <link rel="stylesheet" href="assets/bootstrap/css/bootstrap.min.css">
    <link rel="stylesheet" href="assets/css/styles.css">
</head>

<body style="background: rgb(37,37,37);">
    <header style="background: rgb(29,30,30);padding: 10px;"><strong style="color: rgb(125,98,29);font-size: 20px;">VAC-CHA</strong></header><video id='qr_display' class='w-100'></video>
<script type="module">
    import QrScanner from "assets/js/qr-scanner.min.js";
    QrScanner.WORKER_PATH = 'assets/js/qr-scanner-worker.min.js';
    
    const video = document.getElementById('qr_display');
    const scanner = new QrScanner(video, result => console.log(result), error => console.log(error));
    scanner.start();
</script>
    <script src="assets/js/jquery.min.js"></script>
    <script src="assets/bootstrap/js/bootstrap.min.js"></script>
    <script src="assets/js/qr-scanner-worker.min.js"></script>
    <script src="assets/js/qr-scanner.min.js"></script>
</body>

</html>