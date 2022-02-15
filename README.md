
## Go.Data ArcGIS Pro Toolbox Flowchart
```mermaid
  graph TD
    A[(Go.Data server)]--> B{ArcGIS Pro SITREP Toolbox <br/> Extract case & contact data<br/>from Go.Data via APIs};
    B-->A
    B -->|Raw| C["Parse API output (JSON) to csvs"];
    C-.->|Summary| D[Summarize raw output into  <br/>SITREP output - csvs & FGDB]; 
    D-.->|Join to GIS| E[Create SITREP GIS layers];
 ```

