| Ordered | Objective Title                   | EST Total Min | Mode of Delivery          | Day |
| ------- | --------------------------------- | ------------- | ------------------------- | --- |
| 0       | Course Start                      | 50            | Instruction (Resident)    | 1   |
| 1       | Identifying Misinformation and Disinformation | 130           | Guest Instructor          | 1   |
| 2       | Countering Misinformation and Disinformation | 130           | Instruction (Resident)    | 1   |
| 3       | Identifying Rival Influence       | 130           | Instruction (Resident)    | 2   |
| 4       | Mitigating Rival Influence        | 130           | Instruction (Resident)    | 2   |
| 5       | Recognizing AI Generated Content  | 70            | Instruction (Resident)    | 3   |
| 6       | Reporting Malign Influence        | 70            | Instruction (Resident)    | 3   |
| END     | Capstone                          | 50            | Assessment                | 4   |
| END     | Closing                           | 20            | -                         | 4   |
| END     | TOTAL TIME                        | 750           | 15.0                      | -   |
<!-- TBLFM: @>$3=sum(@I..@-1) -->
<!-- TBLFM: @>$4=(@>$3/50) -->
### NOTE: 
The formulas require an additional plugin: [Advanced Tables](source https://github.com/tgrosinger/md-advanced-tables/blob/main/docs/formulas.md)
Below are the formulas with comments
```md
// Formula to get total minutes in the third column
<!-- TBLFM: @>$3=sum(@I..@-1) -->
// Formula to get total academic hours (50 minutes) based on the total minutes 
<!-- TBLFM: @>$4=(@>$3/50) -->
```

## Referenced Terms
Modes of Delivery:
-  Instruction (Resident)
-  Instruction (Non-Resident)
-  Distributed (Synchronos)
-  Distributed (Asynchronos)
-  Blended
