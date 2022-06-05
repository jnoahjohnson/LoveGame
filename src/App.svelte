<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Style+Script&display=swap" rel="stylesheet"> 

<script>
	let questions = [
		"What is your dream holiday destination?",
		"What scares you the most?",
		"If you could get a free round-trip around the world where would you go?",
		"If you were given a superpower what would that be?",
		"What your idea of an ideal romantic getaway?",
		"Who is one person from your past you wish to be in touch with and why?",
		"What is the best part of our relationship?",
		"If you could relive 3 top memories in this relationship what would that be?",
		"What is my most beautiful physical feature?",
		"If money werent an issue where would you like to be right now?",
		"What is one thing you always wanted to try but never did?",
		"What do you remember from our first meeting?",
		"What is your definition of a successful life?",
		"When was that moment when you knew you were in love with me/or I was the one for you?",
		"What are some traditions you would like us to start as a family?",
		"What is my most attractive feature?",
		"What is your favorite activity with me?",
		"What do you think after you receive a super romantic message from me?",
		"What was your first thought after our first real date together?",
		"What is something you always wanted try with me?",
		"When do you feel closest to me?",
		"What is one thing we must do more often?",
		"Favorite movie and song that reminds you of me",
		"Which Disney prince and princess are we? Which superheroes best represent us?",
		"Dinner at a fancy restaurant or scrumptious home-cooked meal or yummiest take-out at home.",
		"What's your favorite part of my body? ",
		"What kind of outfit would look best on me?",
		"Where do you like being touched the most? (Show, dont tell)",
		"Where would you like to have sex together?",
		"Whats the ultimate role play for you?",
		"What kind of talk do you like, if any, in bed?",
		"Whats your favorite foreplay?",
		"What position do you like the most?",
		"Whats your favorite sexual memory of us?",
		"Would you like me to send you dirty texts at work?",
		"Whats the sexiest thing youve thought about doing to me?",
		"How do I show you that Im attracted to you?",
		"Would you like to be tied up or tie me up?",
		"What types of games gave you the most joy as a child?",
		"Are there types of clothing that you find highly erotic?",
		"Do you remember the best orgasm youve ever had?",
		"Can you describe the last time you got turned on in public?",
		"Would you rather have sex on a plane, or on a moving train?",
		"What's something you want more of in our sex life?",
		"Whats the most unusual place you'd like to have sex with me?",
		"Can I try to make you orgasm without using my hands?",
		"What makes you feel the most loved?",
		"Whats your favorite romance movie?",
		"Is there anything about me you might not know but want to know?",
		"If you could describe me in only one word, what would it be?",
		"Whats been one of the funniest times weve had together?",
		"What could I do to improve our relationship?"
		
	]
	
	let questionNum = 0
	
	function getRandomInt(max) {
		console.log(Math.floor(Math.random() * max))
  	return Math.floor(Math.random() * max);
	}
	
	function newPrompt() {
		questionNum = getRandomInt(questions.length)
	}
</script>

<style>
	body {
		background: #ac3561;
		margin: 0;
		padding: 0;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	
	h1 {
		font-family: 'Style Script', cursive;
		color: white;
		font-size: 3.5rem;
		text-align: center;
	}
	
	button {
		color: #5C0A3C;
		background: white;
		font-size: 1.25rem;
		font-family: 'Style Script', cursive;
		
	}
</style>

<body>
	<h1>{questions[questionNum]}</h1>
<button on:click={newPrompt}>
	Next Question
</button>
	
</body>

