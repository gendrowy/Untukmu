# Untukmu

Halo, Sayang! ❤️

Ada pesan spesial buat kamu! Klik tombol di bawah!

<button class="btn" onclick="tampilkanPesan()">Klik Aku</button>
<p id="pesan"></p>

<script>
    function tampilkanPesan() {
        let pesan = [
            "Aku cinta kamu selamanya! 💖",
            "Kamu adalah cahaya dalam hidupku! ✨",
            "Hari ini indah karena ada kamu! 🌸",
            "Kamu adalah alasan aku tersenyum! 😊"
        ];
        let randomPesan = pesan[Math.floor(Math.random() * pesan.length)];
        document.getElementById("pesan").innerText = randomPesan;
        document.getElementById("pesan").style.display = "block";
    }
</script>

<style>
    body {
        font-family: 'Poppins', sans-serif;
        text-align: center;
        background: linear-gradient(to right, #ff758c, #ff7eb3);
        color: white;
        padding: 50px;
    }
    h1 {
        font-size: 3em;
        animation: fadeIn 2s;
    }
    .container {
        background: rgba(255, 255, 255, 0.2);
        padding: 20px;
        border-radius: 15px;
        display: inline-block;
        margin-top: 20px;
    }
    .btn {
        background: white;
        color: #ff758c;
        font-size: 20px;
        padding: 15px 30px;
        border: none;
        border-radius: 25px;
        cursor: pointer;
        transition: 0.3s;
    }
    .btn:hover {
        background: #ffb3c1;
        color: white;
    }
    #pesan {
        font-size: 1.5em;
        margin-top: 20px;
        display: none;
    }
    @keyframes fadeIn {
        from { opacity: 0; }
        to { opacity: 1; }
    }
</style>
