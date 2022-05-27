<script lang="typescript">
	let message: string = "Blank Svelte Native App";
</script>

<page>
	<!-- <actionBar title="Rithem" /> -->
	<actionBar title="ActionBar Title">
		<gridLayout>
			<label
				text="RithemBoards"
				fontSize="24"
				verticalAlignment="center"
			/>
			<button class="material-icons action-bar-button">leaderboard</button
			>
		</gridLayout>
	</actionBar>

	<gridLayout>
		<!-- svelte-ignore a11y-label-has-associated-control -->
		<label
			class="info"
			horizontalAlignment="center"
			verticalAlignment="middle"
			textWrap="true"
		>
			<formattedString>
				<span class="fas" text="&#xf135;" />
				<span text=" {message}" />
			</formattedString>
		</label>
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
		background: red;
		width: 90px;
		height: 90px;
		border-radius: 80px;
	}
</style>
