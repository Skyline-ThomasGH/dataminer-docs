---
uid: BPA_View_Recursion
---

# View Recursion

This BPA will check the *Views.xml* file to see if any loops are present.

This BPA test is available by default from DataMiner 10.1.0 [CU4]/10.1.7 onwards.

## Metadata

- Name: View Recursion BPA
- Description: Checks if there are loops in Views.xml
- Author: Skyline Communications
- Default schedule: None

## Results

### Success

`No loops detected`

No loops were found in the *Views.xml* file.

### Error

`<number_of_loops> loop(s) detected in Views.xml`

One or more loops were detected. The detailed results will contain the tree structure for each of the loops.

### Not Executed

`An error occurred running the test: <error_Message>`

An unexpected error occurred, preventing the test from running. Please check the detailed results for more info.

## Impact when issues detected

- Impact: Unexpected behavior regarding views will occur, leading to crashes
- Corrective Action: Edit Views.xml to remove the loop
