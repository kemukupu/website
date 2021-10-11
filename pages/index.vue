<template>
	<div>
		<div class="landingImage"></div>
		<section class="section container column is-10 welcomeCard">
			<div class="columns is-desktop ">
				<div class="column desktop-only is-half" />
				<div class="card column">
					<div class="card-content content">
						<h1 class="title is-1 extended">Kia Ora, We Are Kēmu Kupu</h1>
						<p class="content is-size-4">Welcome! We are an aspiring development organisation focussing on the development of language learning tools for Te Reo Maori. We believe that all members of New Zealand should engage with the vibrant culture of Maori life, to better understand the roots of our beautiful Aotearoa! </p>
					</div>
					<div class="card-footer">
						<a class="card-footer-item is-primary is-light button m-2" href="#about">
							Learn More
						</a>
						<a class="card-footer-item is-primary button m-2" href="https://github.com/SOFTENG206-2021/assignment-3-and-project-team-11">
							Download
						</a>
					</div>
				</div>
			</div>
		</section>
		<section class="section container column is-10">
			<ContentPane
				title="Revolutionising Design!"
				body="With our revolutionary fun and interesting design, we find that kids are quickly sucked in to Kēmu Kupu! We have accomplished this through joyful music, bright colors, and an entertaining game loop. We hope that you'll download Kēmu Kupu and give it a try!"
				image="game/title.png"
				:left="true"
				id="about"
			/>
			<div class="spacer-desktop" />
			<div class="spacer-desktop" />
			<ContentPane
				title="Large Topic Selection!"
				body="We here at Kēmu Kupu believe in offering a wide selection of topics to choose from in our spelling application, to cater to children from all walks of life - and aid in progression as they become more skilled at spelling. Topics such as weather, colors, and feelings are all included!"
				image="game/topic.png"
				:left="false"
			/>
			<div class="spacer-desktop" />
			<div class="spacer-desktop" />
			<ContentPane
				title="The Perfect Challenge!"
				body="Kēmu Kupu scales with the abilities of the student! Students can compete against one another on the global leaderboard, or just work to become faster generally and increase their score. This encourages rapid learning and iteration!"
				image="game/quiz.png"
				:left="true"
			/>
			<div class="spacer-desktop" />
			<div class="spacer-desktop" />
			<span id="team"></span>
			<div class="columns">
				<ProfileCard
					class="column"
					name="Josiah Bull"
					image="profiles/jo.jpeg"
					github="https://github.com/JosiahBull"
					linkedin="https://www.linkedin.com/in/josiah-bull/"
					blurb="Backend developer, enjoys tinkering with electronics in his free time."
				/>
				<ProfileCard
					class="column"
					name="John Chen"
					image="profiles/john.jpeg"
					github="https://github.com/johnchen383"
					linkedin="https://www.linkedin.com/in/johnc383/"
					blurb="An avid learner, excited by the potential that the technology of tomorrow holds."
				/>
				<ProfileCard
					class="column"
					name="Serena Lau"
					image="profiles/serena.jpeg"
					github="https://github.com/serenalau272"
					linkedin="https://www.linkedin.com/in/serena-lau-2166111a0/"
					blurb="Loves having fun with software projects and always curious to keep learning more about this big wide world 😀. Also passionate about Chopin and tiramisu macarons."
				/>
			</div>
		</section>
	</div>
</template>

<script>
import ContentPane from '~/components/ContentPane';
import ProfileCard from '~/components/ProfileCard';

export default {
	name: 'HomePage',

	components: {
		ContentPane,
		ProfileCard
	}
}
</script>


<style>

.landingImage {
	height: 100vh;
	width: 100vw;
	background-image: url("~assets/cartoon-landscape.png");
	background-size: cover;                      
    background-repeat: no-repeat;
    background-position: center center;
}

.welcomeCard {
	position: absolute;
	top: 10vh;
	left: 8.35%;
}

.desktop-only {
	display: none;
}

@media only screen and (min-width: 1024px) {
	.spacer-desktop {
		width: 100%;
		margin-top: 5em;
		height:1px;
	}

	.welcomeCard {
		position: absolute;
		top: 20vh;
		right: 5vw;
	}

	.desktop-only {
		display:block;
	}
}

</style>