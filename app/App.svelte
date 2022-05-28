<script lang="typescript">
	import Leaderboard from "./Leaderboard.svelte";
	import { navigate } from "svelte-native";

	let message: string = "Blank Svelte Native App";
</script>

<page>
	<!-- <actionBar title="Rithem" /> -->
	<!-- <actionBar title="ActionBar Title">
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
		</gridLayout>
	</actionBar> -->

	<actionBar title="RithemBoards">
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
		</gridLayout>
		<button
			android.position="actionBar"
			class="material-icons action-bar-button"
			fontFamily="MaterialIcons">more_vert</button
		>
		<button
			android.position="actionBar"
			class="material-icons action-bar-button"
			fontFamily="MaterialIcons">account_circle</button
		>
	</actionBar>

	<scrollView>
		<stackLayout>
			<label>Welcome to the offical Rithem leaderboards app</label>
		</stackLayout>
	</scrollView>
</page>

<style>
	.action-bar-button {
		font-size: 24;
		/* background: red; */
		width: 90px;
		height: 90px;
		border-radius: 80px;
	}
</style>
