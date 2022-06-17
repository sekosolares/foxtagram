<script>
	// import { onMount } from 'svelte';
	import Header from '../components/Header.svelte';
	import Main from '../components/Main.svelte';
	import Sidebar from '../components/Sidebar.svelte';
	import TimeLine from '../components/TimeLine.svelte';
	import '../css/index.css';

	let data = {
		posts: [
			{
				username: 'Lance',
				location: 'Foxemala',
				postComment: 'Now and then I like to take pictures.',
				comments: [
					{
						id: '38829l',
						username: 'FrodoFox',
						text: 'Good pic you have there!'
					},
					{
						id: 'll33290',
						username: 'Londrov',
						text: 'Amazing! Congrats!'
					},
				],
			},
			{
				username: 'Foxandra',
				location: 'France Fox',
				postComment: 'Wish you were here! ',
				comments: [
					{
						id: '324',
						username: 'Colofox',
						text: 'Awww... I love it!'
					},
				],
			},
			{
				username: 'Rogers',
				location: 'New Foxland',
				postComment: 'Aqui pasandola cool',
				comments: [
					{
						id: 'e39290sa',
						username: 'CrazyFox',
						text: 'Wow! That is so cool!'
					},
					{
						id: '399200-1',
						username: 'ConnerFox',
						text: 'I thought it was you on the picture!'
					},
					{
						id: '23222i3',
						username: 'FroggyFoxy',
						text: 'Jump on your next pic! I think it would be nice although I haven\'t tried it yet.'
					},
				],
			},
		]
	};
</script>
<div>
<Header />
<Main>
	<TimeLine posts={data.posts} />
	<Sidebar />
</Main>
</div>

