<script>

    
    export let tableDB = [
        {
            "Name" : "Maria",
            "Favorite Subject" : "Math",
            "Age" : 14
        },
        {
            "Name" : "Jose",
            "Favorite Subject" : "Science",
            "Age" : 13
        },
    ];
    
    </script>
    
    
    <table>
        <thead>
            <tr>
                {#each Object.keys(tableDB[0]) as columnHeading}
                    <th>{columnHeading}</th>
                {/each}
            <tr/>
        </thead>
        <tbody>
            {#each Object.values(tableDB) as row}
                <tr>
                    {#each Object.values(row) as cell}
                        <td>{cell}</td>
                    {/each}
                </tr>
            {/each}
        </tbody>
    </table>
    