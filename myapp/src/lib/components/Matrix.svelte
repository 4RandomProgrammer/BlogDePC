

<canvas class="bg-black w-full h-full" id='Matrix'></canvas>

<script>
    let canva = document.getElementById('Matrix')
    const context = canva.getContext('2d');

    canva.width = window.innerWidth;
    canva.height = window.innerHeight; 

    const katakana = 'アァカサタナハマヤャラワガザダバパイィキシチニヒミリヰギジヂビピウゥクスツヌフムユュルグズブヅプエェケセテネヘメレヱゲゼデベペオォコソトノホモヨョロヲゴゾドボポヴッン';
    const latin = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
    const nums = '0123456789';

    const alphabet = katakana + latin + nums;

    const fontsize = 16;
    const columns = canva.width/fontsize;

    const rainDrops = [];

    for (let index = 0; index < columns; index++) {
        rainDrops[index] = 1;
        
    }

    const draw = () => {
        context.fillStyle = '#0F0';
        context.font = fontsize + 'px monospace';

        for (let i = 0; i < rainDrops.length; i++) {
            const text = alphabet.charAt(Math.floor(Math.random() * alphabet.length));
            context.fillText(text, i * fontsize, rainDrops[i] * fontsize)

            if(rainDrops[i] * fontsize > canva.height && Math.random() > 0.975) {
                rainDrops[i] = 0;
            }

            rainDrops[i]++;
        }

    };


    setInterval(draw,30);
</script>