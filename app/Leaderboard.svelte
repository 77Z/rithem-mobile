<script>
	import { goBack } from "svelte-native";
</script>

<page>
	<actionBar title="ActionBar Title">
		<gridLayout>
			<navigationButton on:tap={goBack} class="material-icons"
				>arrow_back</navigationButton
			>
			<label
				text="RithemBoards"
				fontSize="24"
				verticalAlignment="center"
			/>
			<!-- <button class="material-icons action-bar-button">search</button> -->
		</gridLayout>
	</actionBar>
	<label text="Leaderboard" fontSize="50" verticalAlignment="center" />
</page>
