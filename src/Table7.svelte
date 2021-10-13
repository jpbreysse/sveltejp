<script>

    
    

    export let tableDB = [
        {
            "Name": "gregdb",
            "State": "started",
            "TypeDB": "Mysql",
            "TypeInfra": "single",
            "creationDate": "555 Freeman Street, Winesburg, New Jersey, 8986",
            "Action": "NoAction"

        },
        {

            "Name": "jeanphidb",
            "state": "stop",
            "TypeDB": "Mysql80",
            "typeInfra": "single",
            "creationDate": "555 Freeman Street, Winesburg, New Jersey, 8986",
            "action": "NoAction"

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



    <table id="table2" border="1">
        <thead>
          <tr>
              <th>Select</th>
              <th>Select2</th>
              <th>Select2</th>
          </tr>
        </thead>
        <tbody>
           <tr> 
               <td>
                   <form name="f2" action="javascript:select();" >
                    <input id="edit" type="submit" name="edit" value="Edit" />
                   </form>
               </td>
          </tr>
       </tbody>
      </table>
