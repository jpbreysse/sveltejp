<script>

import { writable } from 'svelte/store';

export let tableDB = writable([
	{
		"Name" : "Maria",
		"Favorite Subject" : "Math",
		"Age" : 14,
		"Action": 1
	},
	{
		"Name" : "JPB",
		"Favorite Subject" : "Math",
		"Age" : 28,
		"Action": 1
	},
	{
		"Name" : "Jose",
		"Favorite Subject" : "Science",
		"Age" : 13,
		"Action" : 2
	},
]);

</script>


<table>
	<thead>
		<tr>
			{#each Object.keys($tableDB[0]) as columnHeading}
				<th>{columnHeading}</th>
			{/each}
		<tr/>
	</thead>
	<tbody>
			<tr>	
					<td>1</td>
					<td>2</td>
					<td>3</td>
					<td>4</td>	
			</tr>
	</tbody>
</table>



