<script>
    import { onMount } from 'svelte';

    
    $: innerHeight = 0;
    $: innerWidth = 0;

    let canva;
    let context;
    let columns;

    const rainDrops = [];
    const fontsize = 16;
    const katakana = 'アァカサタナハマヤャラワガザダバパイィキシチニヒミリヰギジヂビピウゥクスツヌフムユュルグズブヅプエェケセテネヘメレヱゲゼデベペオォコソトノホモヨョロヲゴゾドボポヴッン';
    const latin = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
    const nums = '0123456789';
    const alphabet = katakana + latin + nums;

    onMount(() =>{
        context = canva.getContext('2d');

        canva.width = innerWidth;
        canva.height = innerHeight;


        columns = (canva.getBoundingClientRect().width)/fontsize;
        
        
        
        for (let index = 0; index < columns; index++) {
            rainDrops[index] = 1;
        
        }
    });


    const draw = () => {
        // console.log(innerHeight)
        if (typeof context === "undefined" || canva == null){
            return;
        }

        context.fillStyle = 'rgba(0, 0, 0, 0.05)';
	    context.fillRect(0, 0, canva.width, canva.height);


        context.fillStyle = '#0F0';
        context.font = fontsize + 'px monospace';

        for (let i = 0; i < rainDrops.length; i++) {

            const text = alphabet.charAt(Math.floor(Math.random() * alphabet.length));
            context.fillText(text, i * fontsize, rainDrops[i] * fontsize)
            
            if(rainDrops[i] * fontsize > Math.floor(canva.getBoundingClientRect().height) && Math.random() > 0.975) {
                
                rainDrops[i] = 0;
                
            }

            rainDrops[i]++;
        }

    };

    setInterval(draw,30);

</script>

<svelte:window bind:innerWidth bind:innerHeight />

<canvas

bind:this={canva}
class="bg-black fixed left-0 top-0 -z-10 w-full h-full" 
>
</canvas>