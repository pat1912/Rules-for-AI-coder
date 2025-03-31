# ULTIMATE CODE SHARING PROTOCOL (UCSP)

## FUNDAMENTAL PRINCIPLE: CONFIRMATION-BASED SEQUENTIAL SPLITTING

### PREPARATION PHASE
1. **ARTIFACT INITIALIZATION**: Create ONLY the first artifact (e.g., "script-js-part1") and attempt to include the ENTIRE file content.
2. **CONTENT SOURCE VERIFICATION**: Always maintain the complete source file separately for reference to ensure no content is lost in the splitting process.

### EXECUTION PHASE
3. **MAXIMUM CAPACITY MANDATE**: For every artifact, you MUST attempt to include ALL remaining code before considering splitting.
4. **EXPLICIT CAPACITY TESTING**:
   - Before creating any new part, state: "ATTEMPTING FULL CONTENT INSERTION"
   - When a character limit error occurs, specify: "CAPACITY LIMIT REACHED AT APPROXIMATELY [X] CHARACTERS - SPLITTING REQUIRED"

5. **MANDATORY USER CONFIRMATION**:
   - After reporting the capacity limit, STOP and WAIT for the user's "continue" command
   - Do NOT create the next part until explicitly instructed by the user
   - After receiving the "continue" command, acknowledge with: "CONTINUING WITH PART [N] AS REQUESTED"

6. **SPLITTING DECISION DOCUMENTATION**:
   - Document the exact error message received
   - Identify the precise line number or character position where splitting occurred
   - Reference this information when creating the next part

7. **RIGOROUS CONTINUATION PROCEDURE**:
   - Each new part MUST begin with exact copy of the LAST 10 LINES from previous part
   - Include a "CONTINUATION MARKER" comment: `// CONTINUATION FROM PART X - LINE: "last line from previous part"`
   - Number parts strictly sequentially (part1, part2, etc.) with no gaps, variations, or alphabetic additions

### VERIFICATION PHASE
8. **MANDATORY CONTENT CHECKS**:
   - Before submitting each part, verify that:
     * No code has been omitted or modified
     * Line breaks and spacing remain intact
     * All syntax elements are properly closed
   - After each part, track approximately what percentage of the total file has been shared

9. **PROGRESS TRACKING**:
   - Maintain a running count of parts created
   - Estimate remaining parts based on content size
   - Example format: "PROGRESS: PART 2/~4 COMPLETE (APPROXIMATELY 48% OF TOTAL)"

### ANTI-ERROR MECHANISMS
10. **STRICT SEQUENTIAL CREATION**: 
    - NEVER create part N+1 before part N has been confirmed to reach maximum capacity
    - NEVER create part N+1 without explicit user command to continue
    - Issue explicit confirmation: "PART X MAXIMUM CAPACITY CONFIRMED - WAITING FOR CONTINUE COMMAND"

11. **FORBIDDEN PRACTICES**:
    - NO premature artifact creation
    - NO manually predetermined split points
    - NO content reformatting or compression to fit more in a part
    - NO creation of multiple artifacts simultaneously
    - NO proceeding to next part without user confirmation

12. **ERROR RECOVERY PROTOCOL**:
    - If an error occurs in the sharing process, immediately state: "ERROR IN SHARING PROTOCOL"
    - Identify the nature of the error and how it will be corrected
    - Resume from the last correctly shared part with 20 lines of overlap instead of 10

### COMPLETION CONFIRMATION
13. **FINAL VERIFICATION**:
    - After all parts are shared, provide a summary: "SHARING COMPLETE: X PARTS TOTAL"
    - Confirm the first and last 5 lines of the original file were included
    - State: "ALL CONTENT SUCCESSFULLY TRANSMITTED ACCORDING TO UCSP STANDARDS"

### EXECUTION CHECKLIST
- [ ] Attempt to share entire file in first artifact
- [ ] Document exact capacity limit encountered
- [ ] WAIT for user's "continue" command before proceeding
- [ ] Create next part only after receiving explicit continuation instruction
- [ ] Include proper continuation marker with last 10 lines
- [ ] Verify content integrity before submitting each part
- [ ] Track and report progress after each part
- [ ] Confirm complete transmission upon finishing