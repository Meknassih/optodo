<script>
	import Button, { Label } from "@smui/button";
	import Card from "@smui/card";
	import Textfield from "@smui/textfield";
	import HelperText from "@smui/textfield/helper-text";
	import LayoutGrid, { Cell } from "@smui/layout-grid";

	let username = "", password = "";
</script>

<h1>OPtodo</h1>

<Card padded style="width: 460px; margin: 0 auto;">
	<h3>Authenticate</h3>
	<Textfield
		class="shaped-filled textfield"
		variant="filled"
		style="margin: 8px 4px;"
		bind:value={username}
		label="Username"
	>
		<HelperText slot="helper">At least 3 characters</HelperText>
	</Textfield>
	<Textfield
		class="shaped-filled textfield"
		variant="filled"
		style="margin: 8px 4px;"
		type="password"
		bind:value={password}
		label="Password"
	>
		<HelperText slot="helper">At least 3 characters</HelperText>
	</Textfield>

	<LayoutGrid>
		<Cell span={6}>
			<Button>
				<Label>Sign up</Label>
			</Button>
		</Cell>
		<Cell span={6}>
			<Button variant="raised">
				<Label>Sign in</Label>
			</Button>
		</Cell>
	</LayoutGrid>
</Card>
