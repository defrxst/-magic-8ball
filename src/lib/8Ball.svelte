<script>

  let ball

  let replies = [ // replies
    "It is certain",
    "It is decidedly so",
    "Without a doubt",
    "Yes definetly",
    "You may rely on it",
    "As i see it, yes",
    "Most likely",
    "Outlook good",
    "Yes",
    "Signs point to yes",
    "Reply hazy, try again",
    "Ask again later",
    "Better not tell you now",
    "Cannot predict now",
    "Concentrate and ask again",
    "Don't count on it",
    "My reply is no",
    "My sources say no",
    "Outlook not so good",
    "Very doubtful"
  ]

  function roll() {
    let randomNumber = Math.floor(Math.random() * replies.length)
    ball.style.fontSize = '20px'
    ball.innerHTML = replies[randomNumber]
  }

</script>

<div on:click={()=>roll()} class="w-96 h-96 bg-black left-1/2 -translate-x-1/2 rounded-full m-auto text-center mt-48 absolute flex justify-center items-center">
  <div class="w-64 h-64 bg-white rounded-full flex justify-center items-center">
    <h1 bind:this={ball} class="text-[130px] text-black">8</h1>
  </div>
</div>

