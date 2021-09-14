<script>
	import Table from './Table.svelte';
	import { studentsArray, colors } from './data-store.js';
	
	let redStyle = "redTable";
	let blueStyle = "blueTable";
</script>

<Table tableData={$studentsArray} style={redStyle}/>
<Table tableData={$colors} style={blueStyle}/>
