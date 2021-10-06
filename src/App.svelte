<script>
	import Table from './Table.svelte';
	import Table2 from './Table2.svelte';
	import Table4 from './Table4.svelte';
	import Table5 from './Table5.svelte';
	import Table6 from './Table6.svelte';
	import Uljp from './Uljp.svelte';

	import { studentsArray, colors } from './data-store.js';

	let redStyle = "redTable";
	let blueStyle = "blueTable";
</script>

<!--<Table tableData={$studentsArray} style={redStyle}/>
<Table tableData={$colors} style={blueStyle}/> -->
<Table5 />
<Table2 />
<Table4 />
<Table6 />
<Uljp />