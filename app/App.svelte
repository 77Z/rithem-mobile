<script lang="typescript">
	import Leaderboard from "./Leaderboard.svelte";
	import { navigate } from "svelte-native";

	let message: string = "Blank Svelte Native App";
</script>

<page>
	<!-- <actionBar title="Rithem" /> -->
	<actionBar title="ActionBar Title">
		<gridLayout>
			<button
				class="material-icons action-bar-button"
				on:tap={() => navigate({ page: Leaderboard })}
				>leaderboard</button
			>
			<label
				text="RithemBoards"
				fontSize="24"
				verticalAlignment="center"
			/>
			<!-- <button class="material-icons action-bar-button">search</button> -->
		</gridLayout>
	</actionBar>

	<gridLayout>
		<!-- svelte-ignore a11y-label-has-associated-control -->
		<!-- <a href="yes">Yo</a> -->
		<label text="Main" fontSize="50" verticalAlignment="center" />
	</gridLayout>
</page>

<style>
	.info .fas {
		color: #3a53ff;
	}
	.info {
		font-size: 20;
	}

	.action-bar-button {
		font-size: 24;
		/* background: red; */
		width: 90px;
		height: 90px;
		border-radius: 80px;
	}
</style>
